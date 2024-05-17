#### Les fonctions

En programmation, une fonction est un bloc de code qui effectue une tâche spécifique et peut être appelé (ou invoqué) à partir d'autres parties du programme pour exécuter cette tâche. Les fonctions permettent de regrouper du code en unités logiques et réutilisables, ce qui facilite la gestion et la maintenance du code.

Voici quelques points importants à retenir sur les fonctions :

### 1. Encapsulation :
Les fonctions encapsulent du code en le regroupant dans un seul bloc, ce qui permet de le réutiliser à plusieurs endroits sans avoir à le réécrire.

### 2. Modularité :
Les fonctions favorisent la modularité du code en le divisant en petites unités logiques, ce qui rend le code plus facile à comprendre, à maintenir et à déboguer.

### 3. Réutilisabilité :
Les fonctions peuvent être appelées à partir de différentes parties du programme, ce qui permet de réutiliser le même code pour effectuer des tâches similaires dans différentes parties du programme.

### 4. Paramètres et valeurs de retour :
Les fonctions peuvent accepter des paramètres en entrée, qui sont des valeurs fournies lors de l'appel de la fonction, et elles peuvent également renvoyer une valeur en sortie, qui est le résultat de l'exécution de la fonction.

### 5. Signature de la fonction :
La signature d'une fonction comprend son nom, ses paramètres et son type de retour. Deux fonctions peuvent avoir le même nom tant que leur signature est différente, ce qui permet de surcharger les fonctions (avoir plusieurs fonctions avec le même nom mais des paramètres différents).

### Exemple :
```java
// Définition d'une fonction qui ajoute deux nombres et renvoie le résultat
int additionner(int a, int b) {
    return a + b;
}

// Appel de la fonction et stockage du résultat dans une variable
int resultat = additionner(5, 3);

// Affichage du résultat
System.out.println("Résultat de l'addition : " + resultat);
```

#### La signauture d'une fonction

La signature d'une fonction, également appelée prototype de fonction, comprend plusieurs éléments qui définissent sa structure et son comportement. Voici les principaux éléments de la signature d'une fonction en Java :

1. **Nom de la fonction :** Il s'agit du nom utilisé pour appeler la fonction lors de son utilisation dans le code.

2. **Paramètres de la fonction :** Ce sont les valeurs que la fonction accepte en entrée pour effectuer son travail. Chaque paramètre est composé d'un type et d'un nom. Les paramètres sont placés entre les parenthèses après le nom de la fonction.

3. **Type de retour :** C'est le type de données que la fonction renvoie après son exécution. Si une fonction ne renvoie aucune valeur, son type de retour est déclaré comme `void`.

Voici un exemple de signature de fonction en Java :

```java
public int additionner(int a, int b) {
    // Corps de la fonction
    return a + b;
}
```

Dans cet exemple :

- Le nom de la fonction est `additionner`.
- Les paramètres de la fonction sont `a` et `b`, de type `int`.
- Le type de retour de la fonction est `int`.

#### Les paramètres de fonctions

Les paramètres de fonction sont des variables déclarées dans la déclaration d'une fonction pour recevoir des valeurs lorsqu'elle est appelée. Ces valeurs, appelées arguments, sont passées à la fonction lors de son appel et sont utilisées à l'intérieur de la fonction pour effectuer des opérations.

Voici quelques points importants à retenir sur les paramètres de fonction en Java :

1. **Déclaration :** Les paramètres de fonction sont déclarés entre parenthèses après le nom de la fonction. Chaque paramètre est composé d'un type suivi de son nom.

2. **Types de données :** Les paramètres peuvent être de n'importe quel type de données valide en Java, y compris les types primitifs (comme `int`, `double`, `boolean`, etc.) et les types de référence (comme les objets, les tableaux, etc.).

3. **Passage de paramètres :** Lorsqu'une fonction est appelée, les valeurs des arguments fournis sont passées aux paramètres correspondants dans la déclaration de la fonction. Ces valeurs sont ensuite accessibles à l'intérieur de la fonction via les paramètres.

4. **Nombre de paramètres :** Une fonction peut avoir zéro ou plusieurs paramètres. Les paramètres sont séparés par des virgules dans la liste des paramètres de la fonction.

5. **Nom des paramètres :** Les noms des paramètres sont des identificateurs qui sont utilisés à l'intérieur de la fonction pour faire référence aux valeurs des arguments passés lors de l'appel de la fonction.

Voici un exemple de déclaration de fonction avec des paramètres en Java :

```java
public void afficherMessage(String message, int nombre) {
    System.out.println("Message : " + message);
    System.out.println("Nombre : " + nombre);
}
```

#### Les packages

En Java, un package est un mécanisme permettant d'organiser et de regrouper un ensemble de classes et d'interfaces connexes. Les packages aident à structurer les projets Java en fournissant une hiérarchie de répertoires pour les fichiers source et les fichiers compilés (.class).

Voici quelques points importants à retenir sur les packages en Java :

1. **Organisation des classes :** Les packages permettent d'organiser les classes en groupes logiques selon leur fonctionnalité ou leur domaine d'application. Cela facilite la gestion des classes et améliore la lisibilité du code.

2. **Déclaration :** Pour déclarer une classe ou une interface dans un package, vous devez inclure une directive `package` au début du fichier source. Par exemple, `package com.example.mypackage;`.

3. **Importation :** Pour utiliser une classe ou une interface définie dans un autre package, vous devez importer le package en utilisant la directive `import`. Par exemple, `import com.example.otherpackage.MyClass;`.

4. **Hiérarchie :** Les packages peuvent être organisés hiérarchiquement, avec des packages parentaux contenant des sous-packages et des classes. Par exemple, `com.example` peut être un package parent de `com.example.subpackage`.

5. **Nommage :** Les conventions de nommage recommandent d'utiliser des noms de packages en minuscules et en utilisant des noms de domaine inversés. Par exemple, `com.example.mypackage`.

6. **Visibilité :** Les membres d'un package ont une visibilité par défaut entre les classes du même package. Cela signifie que les classes du même package peuvent accéder aux membres (champs, méthodes) sans avoir besoin de spécifier d'importations.

7. **Accessibilité :** Certains membres peuvent être déclarés `public` pour être accessibles en dehors du package, tandis que d'autres peuvent être déclarés `protected`, `private` ou ne pas avoir de modificateur d'accès pour restreindre leur visibilité.

#### Création et utilisation de packages

Pour utiliser un package en Java, vous devez suivre quelques étapes simples :

1. **Importation du package :** Si vous avez déjà créé un package avec des classes, vous devez l'importer dans le fichier Java où vous souhaitez utiliser ces classes. Pour ce faire, utilisez la directive `import` au début du fichier Java.

2. **Création d'objets :** Une fois le package importé, vous pouvez créer des objets des classes qui s'y trouvent et utiliser ces objets dans votre programme.

Voici un exemple concret pour illustrer l'utilisation d'un package :

Supposons que vous avez un package appelé `com.example.mypackage`, qui contient une classe appelée `MaClasse`. Voici comment vous pouvez l'utiliser :

1. Créez une structure de répertoires comme suit :

```
myproject/
└── src/
    ├── com/
    │   └── example/
    │       └── mypackage/
    │           └── MaClasse.java
    └── MonProgramme.java
```

2. Contenu du fichier `MaClasse.java` :

```java
package com.example.mypackage;

public class MaClasse {
    public void afficherMessage() {
        System.out.println("Bonjour depuis MaClasse !");
    }
}
```

3. Contenu du fichier `MonProgramme.java` :

```java
import com.example.mypackage.MaClasse;

public class MonProgramme {
    public static void main(String[] args) {
        // Créer un objet de la classe MaClasse
        MaClasse objet = new MaClasse();
        
        // Appeler la méthode afficherMessage() de MaClasse
        objet.afficherMessage();
    }
}
```
