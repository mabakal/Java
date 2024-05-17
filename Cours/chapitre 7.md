#### Générécité

La généricité, également connue sous le nom de programmation générique, est une fonctionnalité introduite dans Java 5 qui permet aux développeurs de créer des classes, des interfaces et des méthodes qui peuvent fonctionner avec différents types de données sans compromettre la sécurité du type à la compilation.

#### Avantages de la généricité

La généricité, ou la programmation générique, présente plusieurs avantages dans le développement logiciel en Java :

1. **Sécurité du type à la compilation :** La généricité permet de détecter les erreurs de type dès la phase de compilation plutôt qu'à l'exécution. Cela garantit que les types utilisés dans le code sont cohérents et appropriés, ce qui réduit les risques d'erreurs à l'exécution.

2. **Réutilisabilité du code :** Les classes et les méthodes génériques peuvent être utilisées avec différents types de données sans modification du code source. Cela permet de réutiliser le même code dans différentes situations, ce qui favorise la modularité et la maintenabilité du code.

3. **Abstraction des algorithmes :** En utilisant la généricité, il est possible de créer des algorithmes et des structures de données qui sont indépendants des types spécifiques de données avec lesquels ils travaillent. Cela permet de créer des solutions algorithmiques plus génériques et flexibles.

4. **Élimination des castings inutiles :** Les types génériques permettent d'éviter les castings (conversions de type) inutiles dans le code, ce qui rend le code plus clair, plus concis et plus sûr.

5. **Performance :** Bien que la généricité ait un léger coût en termes de performance en raison de l'utilisation de types de données paramétrés, elle offre généralement une performance comparable à celle des approches non génériques, tout en offrant des avantages en termes de sécurité et de maintenabilité.

6. **Compatibilité avec les types primitifs et les objets :** La généricité peut être utilisée avec des types primitifs (int, double, etc.) ainsi qu'avec des types d'objets (String, Integer, etc.), ce qui permet une utilisation flexible dans divers contextes.

#### Création d'un Type générique

Pour créer un type générique en Java, utiliser les paramètres du types générique.


#### Les methodes générique

Les méthodes génériques sont des méthodes qui peuvent accepter des arguments de type générique et/ou retourner des valeurs de type générique. Elles sont déclarées de manière similaire aux classes génériques, en utilisant des paramètres de type générique entre les chevrons ("< >"). Voici quelques caractéristiques et exemples de méthodes génériques en Java :

1. **Déclaration d'une méthode générique :** Pour déclarer une méthode générique, utilisez des paramètres de type générique entre les chevrons ("< >") avant le type de retour de la méthode. Par exemple :

    ```java
    public <T> void afficher(T element) {
        System.out.println(element);
    }
    ```

    Dans cet exemple, "<T>" est le paramètre de type générique de la méthode "afficher".

2. **Utilisation d'un type générique comme type de retour :** Vous pouvez également utiliser un type générique comme type de retour de la méthode. Par exemple :

    ```java
    public <T> T obtenirPremier(List<T> liste) {
        return liste.get(0);
    }
    ```

    Dans cet exemple, la méthode "obtenirPremier" retourne un élément de type générique "T" à partir d'une liste.

3. **Contraintes de type :** Vous pouvez imposer des contraintes sur les types génériques utilisés dans une méthode en utilisant le mot-clé "extends". Par exemple :

    ```java
    public <T extends Comparable<T>> T trouverMax(T a, T b) {
        return a.compareTo(b) > 0 ? a : b;
    }
    ```

    Dans cet exemple, la méthode "trouverMax" accepte deux arguments de type générique "T" qui doivent être des sous-types de "Comparable<T>".

4. **Utilisation de plusieurs paramètres de type générique :** Vous pouvez déclarer plusieurs paramètres de type générique pour une méthode. Par exemple :

    ```java
    public <T, U> void afficherPair(T premier, U deuxieme) {
        System.out.println("Premier élément : " + premier);
        System.out.println("Deuxième élément : " + deuxieme);
    }
    ```
#### Généricité et l'héritage


#### Types générique et implementation


#### Les symboles utilse

***Wildcards***

Les wildcards, ou caractères génériques en français, sont des symboles utilisés en Java dans le contexte des types génériques pour représenter des types inconnus ou non spécifiés. Ils sont utilisés pour fournir une certaine flexibilité lors de l'utilisation de types génériques. Il existe deux types de wildcards : les wildcards avec une borne supérieure (upper bounded wildcards) et les wildcards avec une borne inférieure (lower bounded wildcards).

1. **Wildcard avec une borne supérieure (`? extends Type`) :** Ce type de wildcard permet de spécifier que le type générique peut être n'importe quel sous-type d'un certain type spécifié. Par exemple, `List<? extends Number>` signifie que la liste peut contenir n'importe quel sous-type de `Number`. Cela permet de rendre le code plus flexible en acceptant une variété de types, tout en garantissant que ces types sont des sous-types de la borne supérieure spécifiée.

2. **Wildcard avec une borne inférieure (`? super Type`) :** Ce type de wildcard permet de spécifier que le type générique peut être n'importe quel supertype (ou type parent) d'un certain type spécifié. Par exemple, `List<? super Integer>` signifie que la liste peut contenir n'importe quel type qui est un supertype de `Integer`. Cela permet d'accepter une variété de types qui sont des super-types du type spécifié.


#### Heritage

En Java, les types génériques peuvent hériter des classes, mais il y a certaines limitations et règles à suivre pour garantir la sécurité et la cohérence du code. Voici les principales règles à respecter lors de l'héritage de classes avec des types génériques :

1. **Héritage de classes génériques :** Une classe générique peut hériter d'une autre classe générique. Par exemple :

    ```java
    public class MaClasseGenerique<T> extends ClasseParente<T> {
        // ...
    }
    ```

    Ici, `MaClasseGenerique<T>` est une classe générique qui hérite de `ClasseParente<T>`, une autre classe générique.

2. **Utilisation de types génériques dans la hiérarchie d'héritage :** Lorsque vous utilisez des types génériques dans la hiérarchie d'héritage, assurez-vous de spécifier les mêmes types de paramètres génériques pour toutes les classes impliquées. Par exemple :

    ```java
    public class MaClasseGenerique<T> extends ClasseParente<T> {
        // ...
    }

    public class ClasseParente<T> {
        // ...
    }
    ```

    Dans cet exemple, `T` est utilisé de manière cohérente dans `MaClasseGenerique` et `ClasseParente`.

3. **Héritage de classes non génériques avec des classes génériques :** Une classe non générique peut hériter d'une classe générique. Dans ce cas, le type générique doit être spécifié avec des arguments de type concrets dans la déclaration de la classe héritée. Par exemple :

    ```java
    public class MaClasseGenerique<T> {
        // ...
    }

    public class MaClasseNonGenerique extends MaClasseGenerique<String> {
        // ...
    }
    ```

    Ici, `MaClasseNonGenerique` hérite de `MaClasseGenerique`, mais le type générique `T` est spécifié comme `String`.

4. **Héritage de classes génériques avec des types sauvages ("wildcards") :** Lorsque vous héritez d'une classe générique avec des types sauvages, utilisez les mêmes types sauvages dans la sous-classe ou spécifiez un type générique concret. Par exemple :

    ```java
    public class MaClasseGenerique<T> {
        // ...
    }

    public class MaClasseSousClasse extends MaClasseGenerique<?> {
        // Utilisation de wildcard (?)
        // ...
    }
    ```

    Ou :

    ```java
    public class MaClasseGenerique<T> {
        // ...
    }

    public class MaClasseSousClasse<T> extends MaClasseGenerique<T> {
        // Spécification d'un type générique concret
        // ...
    }
    ```

    Dans ces exemples, `?` est un wildcard qui représente un type inconnu.


#### Création de classe générique

Pour créer un type générique en Java, vous pouvez utiliser la syntaxe suivante :

```java
public class NomDeClasse<T> {
    // Code de la classe avec l'utilisation du type générique T
}
```

Dans cet exemple, `T` est un paramètre de type générique. Vous pouvez utiliser n'importe quel nom pour ce paramètre, mais `T` est communément utilisé pour représenter un type générique. Vous pouvez également avoir plusieurs paramètres de type générique en utilisant une virgule pour les séparer, par exemple `NomDeClasse<T, U>`.

Voici un exemple simple d'une classe générique en Java :

```java
public class Boite<T> {
    private T contenu;

    public Boite(T contenu) {
        this.contenu = contenu;
    }

    public T getContenu() {
        return contenu;
    }

    public void setContenu(T contenu) {
        this.contenu = contenu;
    }
}
```

Dans cet exemple, `Boite` est une classe générique qui peut contenir n'importe quel type d'objet. Le type de l'objet est spécifié lors de la création d'une instance de la classe `Boite`. Par exemple :

```java
Boite<String> boiteString = new Boite<>("Contenu de la boîte");
System.out.println(boiteString.getContenu()); // Affiche : Contenu de la boîte

Boite<Integer> boiteInteger = new Boite<>(42);
System.out.println(boiteInteger.getContenu()); // Affiche : 42
```

