### Les structure de données

Les structures de données sont des méthodes organisées et efficaces pour stocker, gérer et manipuler des données dans un programme informatique. Elles fournissent un moyen de structurer et d'organiser les données afin de faciliter leur accès, leur traitement et leur gestion.


Voici quelques-unes des structures de données les plus couramment utilisées :

1. **Tableaux :** Une collection ordonnée d'éléments de données du même type, accessibles via un index numérique.

2. **Listes chaînées :** Une séquence d'éléments où chaque élément est lié au suivant par un pointeur, permettant une insertion et une suppression efficaces à n'importe quel point de la liste.

3. **Piles :** Une structure de données linéaire de type LIFO (Last In, First Out), où les éléments sont ajoutés et supprimés uniquement à une extrémité, généralement appelée le sommet.

4. **File d'attente :** Une structure de données linéaire de type FIFO (First In, First Out), où les éléments sont ajoutés à l'arrière et supprimés à l'avant.

5. **Arbres :** Une structure de données hiérarchique composée de nœuds, où chaque nœud a un parent et zéro ou plusieurs enfants.

6. **Graphes :** Une structure de données non linéaire composée de nœuds (ou sommets) connectés par des arêtes, permettant de représenter des relations arbitraires entre les éléments.

7. **Ensembles :** Une collection d'éléments uniques, sans ordre spécifique, où chaque élément n'apparaît qu'une seule fois.

8. **Dictionnaires (ou Maps) :** Une collection associant des clés à des valeurs, permettant un accès rapide et efficace aux données à l'aide de la clé.

#### Structure de données en Java

En Java, les structures de données peuvent être implémentées à l'aide des classes fournies par la bibliothèque standard de Java (java.util). Voici quelques-unes des structures de données les plus couramment utilisées en Java :

1. **Tableaux :** Les tableaux sont des structures de données simples et fondamentales en Java. Ils peuvent être déclarés de la forme `type[] nomDuTableau = new type[taille];` et permettent de stocker des éléments de données du même type dans un conteneur linéaire.

2. **Listes :** Les listes sont des collections ordonnées d'éléments qui permettent l'insertion, la suppression et l'accès séquentiel aux données. Les classes de liste les plus couramment utilisées en Java sont ArrayList et LinkedList.

    ```java
    ArrayList<Integer> arrayList = new ArrayList<>();
    LinkedList<String> linkedList = new LinkedList<>();
    ```

3. **Ensembles :** Les ensembles sont des collections qui ne contiennent pas d'éléments dupliqués. HashSet, TreeSet et LinkedHashSet sont les implémentations d'ensembles les plus couramment utilisées en Java.

    ```java
    HashSet<String> hashSet = new HashSet<>();
    TreeSet<Integer> treeSet = new TreeSet<>();
    ```

4. **Cartes (ou Maps) :** Les cartes associent des clés à des valeurs uniques. HashMap, TreeMap et LinkedHashMap sont les implémentations de cartes les plus couramment utilisées en Java.

    ```java
    HashMap<String, Integer> hashMap = new HashMap<>();
    TreeMap<Integer, String> treeMap = new TreeMap<>();
    ```

5. **Piles et Files :** Bien qu'il n'y ait pas de classes spécifiques pour les piles et les files dans la bibliothèque standard de Java, vous pouvez les implémenter à l'aide de LinkedList en respectant les principes LIFO (Last In, First Out) pour les piles et FIFO (First In, First Out) pour les files.

6. **Autres structures de données :** Java propose également d'autres structures de données telles que les files de priorité (PriorityQueue), les listes de double pointage (Deque), les piles de double pointage (ArrayDeque) et plus encore.

En utilisant ces classes de structures de données prédéfinies, vous pouvez facilement manipuler et gérer des données dans vos programmes Java de manière efficace et pratique.

#### Les collections

En Java, le terme "collections" fait référence à un ensemble de classes et d'interfaces fournies dans le package `java.util` qui permettent de stocker, de manipuler et de gérer des groupes d'objets. Les collections offrent une manière flexible et dynamique de travailler avec des données, en permettant d'ajouter, de supprimer et de rechercher des éléments de manière efficace.

Les collections en Java sont hautement paramétrables grâce à l'utilisation de génériques, ce qui signifie qu'elles peuvent stocker des éléments de n'importe quel type spécifié lors de leur utilisation.

Voici quelques-unes des principales interfaces de collection en Java :

1. **List :** Une collection ordonnée qui permet des éléments dupliqués. Les implémentations les plus courantes sont ArrayList et LinkedList.

2. **Set :** Une collection qui ne permet pas d'éléments dupliqués. Les implémentations les plus courantes sont HashSet, TreeSet et LinkedHashSet.

3. **Map :** Une collection d'associations clé-valeur, où chaque élément est stocké en tant que paire clé-valeur unique. Les implémentations les plus courantes sont HashMap, TreeMap et LinkedHashMap.

4. **Queue :** Une collection qui représente une file d'attente, où les éléments sont insérés à la fin et retirés du début. Les implémentations les plus courantes sont PriorityQueue et LinkedList.

5. **Deque :** Une double-ended queue qui prend en charge l'ajout et la suppression d'éléments des deux extrémités de la file. L'implémentation la plus courante est ArrayDeque.


#### Parcourir les collections


1. **Boucle for-each :** La boucle for-each, également connue sous le nom de boucle for each, est une méthode simple et élégante pour parcourir les collections en Java. Elle est particulièrement utile lorsque vous voulez simplement accéder à chaque élément de la collection sans avoir besoin d'indices. Cette méthode est disponible pour toutes les collections qui implémentent l'interface Iterable.

    Exemple :
    ```java
    List<String> liste = new ArrayList<>();
    // Ajouter des éléments à la liste...
    
    for (String element : liste) {
        System.out.println(element);
    }
    ```

2. **Iterator :** L'interface Iterator permet de parcourir les éléments d'une collection de manière itérative. Elle offre des méthodes telles que `hasNext()` pour vérifier s'il y a un élément suivant et `next()` pour récupérer l'élément suivant.

    Exemple :
    ```java
    List<Integer> liste = new ArrayList<>();
    // Ajouter des éléments à la liste...
    
    Iterator<Integer> iterator = liste.iterator();
    while (iterator.hasNext()) {
        Integer element = iterator.next();
        System.out.println(element);
    }
    ```

3. **Boucle for :** Vous pouvez utiliser une boucle for standard avec un indice pour parcourir les collections qui prennent en charge l'accès par indice, comme les listes. Cependant, cette méthode est moins recommandée car elle nécessite plus de code et est moins lisible que les autres méthodes mentionnées ci-dessus.

    Exemple :
    ```java
    List<String> liste = new ArrayList<>();
    // Ajouter des éléments à la liste...
    
    for (int i = 0; i < liste.size(); i++) {
        String element = liste.get(i);
        System.out.println(element);
    }
    ```

#### Les listes

En Java, les listes sont des structures de données très utilisées qui permettent de stocker une collection ordonnée d'éléments. Java offre plusieurs implémentations de listes dans sa bibliothèque standard, notamment `ArrayList`, `LinkedList` et `Vector`. Voici un aperçu de ces implémentations :

1. **ArrayList :** Cette classe implémente l'interface `List` et utilise un tableau dynamique pour stocker les éléments. Les `ArrayList` offrent un accès rapide aux éléments par indice, mais les opérations d'insertion et de suppression peuvent être coûteuses en temps si elles modifient la taille interne du tableau.

2. **LinkedList :** Cette classe implémente également l'interface `List`, mais utilise une structure de liste chaînée pour stocker les éléments. Les `LinkedList` offrent un accès rapide aux éléments en début et en fin de liste, ainsi que des opérations d'insertion et de suppression efficaces, mais elles sont moins performantes pour l'accès aléatoire par indice.

3. **Vector :** Cette classe est similaire à `ArrayList`, mais elle est synchronisée, ce qui signifie qu'elle est thread-safe. Cependant, cette synchronisation peut entraîner des performances légèrement inférieures par rapport à `ArrayList`.

Voici un exemple d'utilisation d'une `ArrayList` en Java :

```java
import java.util.ArrayList;
import java.util.List;

public class ExempleListe {
    public static void main(String[] args) {
        // Créer une liste
        List<String> liste = new ArrayList<>();

        // Ajouter des éléments à la liste
        liste.add("Element 1");
        liste.add("Element 2");
        liste.add("Element 3");

        // Parcourir et afficher les éléments de la liste
        for (String element : liste) {
            System.out.println(element);
        }
    }
}
```

Les listes sont des structures de données fondamentales qui offrent plusieurs caractéristiques importantes :

1. **Ordre :** Les éléments d'une liste sont organisés dans un ordre spécifique, ce qui signifie que chaque élément a une position relative par rapport aux autres éléments de la liste. Cela permet d'accéder aux éléments par leur indice ou leur position dans la liste.

2. **Accès aux éléments :** Les listes permettent un accès efficace aux éléments individuels par leur indice. Cela signifie que vous pouvez accéder rapidement à n'importe quel élément de la liste en connaissant son indice.

3. **Insertion et suppression :** Les listes permettent l'insertion et la suppression dynamiques d'éléments. Vous pouvez ajouter de nouveaux éléments à n'importe quel endroit de la liste et supprimer des éléments existants en fonction de leurs indices.

4. **Taille dynamique :** Les listes peuvent grandir ou rétrécir dynamiquement pour accommoder le nombre d'éléments qu'elles contiennent. Cela signifie que vous n'avez pas besoin de spécifier une taille fixe pour une liste à l'avance, ce qui les rend très flexibles et adaptées à une variété de situations.

5. **Itérabilité :** Les listes sont itérables, ce qui signifie que vous pouvez parcourir tous les éléments de la liste à l'aide de boucles ou d'itérateurs. Cela facilite le traitement de tous les éléments de la liste de manière séquentielle.

6. **Duplicatas :** Les listes peuvent contenir des éléments en double. Cela signifie que vous pouvez avoir plusieurs occurrences du même élément dans une liste.

7. **Mutabilité :** Dans de nombreuses implémentations de listes, les éléments peuvent être modifiés après leur insertion. Cependant, certaines implémentations de listes, comme `List.of()` dans Java 9 et versions ultérieures, créent des listes immuables, où les éléments ne peuvent pas être modifiés après leur insertion.

***Les differentes type de liste en Java***


1. **ArrayList :** Cette classe implémente l'interface `List` et utilise un tableau dynamique pour stocker les éléments. Les `ArrayList` offrent un accès rapide aux éléments par indice, mais les opérations d'insertion et de suppression peuvent être coûteuses en temps si elles modifient la taille interne du tableau.

2. **LinkedList :** Cette classe implémente également l'interface `List`, mais utilise une structure de liste chaînée pour stocker les éléments. Les `LinkedList` offrent un accès rapide aux éléments en début et en fin de liste, ainsi que des opérations d'insertion et de suppression efficaces, mais elles sont moins performantes pour l'accès aléatoire par indice.

3. **Vector :** Cette classe est similaire à `ArrayList`, mais elle est synchronisée, ce qui signifie qu'elle est thread-safe. Cependant, cette synchronisation peut entraîner des performances légèrement inférieures par rapport à `ArrayList`.

4. **Stack :** La classe `Stack` représente une pile (structure de données LIFO - Last In, First Out) en Java. Elle hérite de la classe `Vector` et fournit des méthodes pour empiler et dépiler des éléments.

5. **CopyOnWriteArrayList :** Cette classe est une variante de `ArrayList` qui est thread-safe pour la lecture. Elle garantit que les opérations de lecture sont effectuées de manière atomique sans nécessiter de synchronisation explicite. Cependant, les opérations d'écriture (comme l'ajout et la suppression d'éléments) sont plus coûteuses en temps car elles effectuent une copie complète de la liste.

6. **Listes immuables :** À partir de Java 9, des méthodes statiques `List.of()` et `List.copyOf()` ont été introduites pour créer des listes immuables. Ces listes ne peuvent pas être modifiées après leur création, ce qui les rend idéales pour les situations où l'immutabilité est souhaitée.


#### Les ensembles

En programmation, un ensemble (ou "set" en anglais) est une structure de données qui représente une collection non ordonnée d'éléments uniques. Contrairement aux listes où l'ordre des éléments est important et où les éléments peuvent être répétés, un ensemble ne conserve pas l'ordre des éléments et garantit que chaque élément est unique.

Les ensembles sont utilisés lorsque vous avez besoin de stocker un groupe d'éléments sans vous soucier de l'ordre dans lequel ils ont été ajoutés et sans permettre de doublons. Les opérations principales sur les ensembles comprennent l'ajout d'éléments, la suppression d'éléments et la vérification de l'appartenance d'un élément à l'ensemble.

En Java, l'interface principale pour représenter un ensemble est `Set`, qui est implémentée par plusieurs classes dans la bibliothèque standard Java. Les implémentations les plus courantes incluent :

1. **HashSet :** Cette classe utilise une table de hachage pour stocker les éléments, ce qui offre des performances constantes (en moyenne) pour les opérations d'ajout, de suppression et de recherche. Les éléments ne sont pas conservés dans un ordre spécifique.

2. **TreeSet :** Cette classe utilise un arbre binaire de recherche pour stocker les éléments, ce qui garantit un ordre naturel des éléments (par exemple, triés par ordre croissant). Les opérations d'ajout, de suppression et de recherche ont une complexité logarithmique, ce qui peut être plus lent que HashSet pour les ensembles de grande taille, mais garantit un ordre spécifique des éléments.

3. **LinkedHashSet :** Cette classe est similaire à HashSet, mais elle conserve l'ordre d'insertion des éléments. Cela signifie que lorsque vous parcourez un LinkedHashSet, les éléments sont renvoyés dans l'ordre dans lequel ils ont été ajoutés.

#### Avantages des ensembles


Les ensembles présentent plusieurs avantages qui les rendent utiles dans de nombreuses situations en programmation :

1. **Unicité des éléments :** Les ensembles garantissent que chaque élément est unique. Cela signifie qu'un élément ne peut apparaître qu'une seule fois dans un ensemble, ce qui simplifie la manipulation des données et évite les doublons.

2. **Absence d'ordre :** Contrairement aux listes ou aux tableaux où l'ordre des éléments est important, les ensembles ne conservent pas d'ordre spécifique des éléments. Cela permet une manipulation plus flexible des données sans se soucier de leur position dans l'ensemble.

3. **Recherche efficace :** Les ensembles offrent généralement des opérations de recherche efficaces. Selon l'implémentation, la recherche d'un élément dans un ensemble peut avoir une complexité de temps constante (en moyenne) ou logarithmique, ce qui est beaucoup plus rapide que parcourir une liste ou un tableau pour effectuer une recherche.

4. **Opérations ensemblistes :** Les ensembles supportent des opérations ensemblistes telles que l'union, l'intersection, la différence et la différence symétrique. Ces opérations sont souvent utilisées pour combiner, comparer ou filtrer des ensembles de données.

5. **Simplicité d'utilisation :** Les ensembles offrent une interface simple et intuitive pour ajouter, supprimer et vérifier l'appartenance d'éléments. Cela facilite leur utilisation dans de nombreuses situations sans nécessiter de connaissances complexes sur la structure interne de l'ensemble.

6. **Utilisation dans les algorithmes :** Les ensembles sont largement utilisés dans la conception d'algorithmes pour résoudre des problèmes tels que la recherche de motifs, la déduplication de données, la validation d'unicité et bien d'autres. Leur unicité et leur efficacité de recherche en font des structures de données précieuses dans de nombreux contextes.


#### Les Maps

Une map (ou tableau associatif) est une structure de données qui associe des paires clé-valeur, où chaque clé est unique et est utilisée pour accéder à sa valeur correspondante. Contrairement aux listes ou aux ensembles, où les éléments sont simplement stockés dans un ordre séquentiel ou sans ordre, les maps fournissent une correspondance explicite entre les clés et les valeurs.

En Java, l'interface principale pour représenter une map est `Map`, qui est implémentée par plusieurs classes dans la bibliothèque standard Java. Les implémentations les plus couramment utilisées incluent :

1. **HashMap :** Cette classe utilise une table de hachage pour stocker les paires clé-valeur, offrant des opérations d'insertion, de suppression et de recherche efficaces avec une complexité de temps moyenne constante (O(1)). Les clés ne sont pas conservées dans un ordre spécifique.

2. **TreeMap :** Cette classe utilise une structure d'arbre binaire de recherche pour stocker les paires clé-valeur, ce qui garantit un ordre naturel des clés (par exemple, triées par ordre croissant). Les opérations d'insertion, de suppression et de recherche ont une complexité de temps logarithmique (O(log n)).

3. **LinkedHashMap :** Cette classe est similaire à HashMap, mais elle conserve l'ordre d'insertion des paires clé-valeur. Cela signifie que lorsque vous parcourez un LinkedHashMap, les paires clé-valeur sont renvoyées dans l'ordre dans lequel elles ont été insérées.

4. **EnumMap :** Cette classe est une implémentation spéciale de Map conçue pour les clés de type énumération. Elle est optimisée pour une utilisation avec des énumérations, offrant de meilleures performances et une utilisation plus sûre des types.

#### Les avantages des Maps

Les maps offrent plusieurs avantages qui les rendent indispensables dans de nombreux scénarios de programmation :

1. **Association clé-valeur :** Les maps permettent d'associer des valeurs à des clés uniques, ce qui facilite la recherche, l'accès et la manipulation des données en fonction de leurs clés.

2. **Recherche rapide :** Grâce à leurs structures internes optimisées (comme les tables de hachage ou les arbres binaires de recherche), les maps offrent des performances de recherche efficaces, souvent en temps constant (O(1)) ou logarithmique (O(log n)).

3. **Flexibilité :** Les maps peuvent stocker une grande variété de types de données comme valeurs, ce qui permet de représenter des associations diverses et complexes entre les clés et les valeurs.

4. **Gestion des données structurées :** Les maps permettent de gérer des données structurées de manière claire et organisée, en associant des informations pertinentes avec des clés significatives.

5. **Évolutivité :** Les maps peuvent être étendues pour contenir un nombre variable d'éléments, ce qui les rend adaptées à une large gamme de scénarios, des petites collections aux ensembles de données volumineux.

6. **Facilité d'utilisation :** Les méthodes et les opérations fournies par les interfaces Map et ses implémentations rendent l'utilisation des maps simple et intuitive dans le code Java.

7. **Gestion des clés uniques :** Les maps garantissent l'unicité des clés, ce qui facilite la manipulation des données et évite les conflits ou les doublons.

8. **Structure de données polyvalente :** Les maps peuvent être utilisées dans de nombreux contextes de programmation, notamment pour la gestion de caches, la représentation de données relationnelles, la résolution de problèmes algorithmiques, etc.

#### Les itérateurs

Les itérateurs sont des objets permettant de parcourir séquentiellement les éléments d'une collection de données, tels que des listes, des ensembles ou des maps, sans exposer la structure interne de la collection. Ils offrent une manière standardisée de parcourir les éléments d'une collection, indépendamment de sa mise en œuvre spécifique.

En Java, l'interface principale pour les itérateurs est `Iterator`, qui définit plusieurs méthodes permettant de parcourir une collection. Les collections Java telles que les listes (`List`), les ensembles (`Set`) et les maps (`Map`) implémentent souvent l'interface `Iterable`, qui permet de récupérer un itérateur pour parcourir leurs éléments.

Les méthodes principales de l'interface `Iterator` incluent :

1. **`boolean hasNext()`:** Cette méthode retourne vrai si la collection contient plus d'éléments à parcourir, sinon elle retourne faux.

2. **`E next()`:** Cette méthode renvoie le prochain élément de la collection et fait avancer l'itérateur. Si aucun élément suivant n'est disponible, elle lève une exception de type `NoSuchElementException`.

3. **`void remove()`:** Cette méthode permet de supprimer l'élément actuellement pointé par l'itérateur. Elle peut être appelée après un appel à la méthode `next()`, mais elle n'est pas supportée par tous les types d'itérateurs.



