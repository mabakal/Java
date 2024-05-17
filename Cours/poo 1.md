#### Programmation orienté object

La programmation orientée objet (POO) est un paradigme de programmation qui repose sur le concept d'objets. Dans ce paradigme, un programme est conçu comme une collection d'objets qui interagissent entre eux pour accomplir des tâches. Chaque objet est une instance d'une classe, qui définit sa structure et son comportement.

#### C'est quoi un objet?

Un objet fait référence à une entité matérielle ou conceptuelle distincte et définie, généralement caractérisée par ses propriétés, ses attributs ou ses relations avec d'autres entités.

Par exemple :

1. **Objet matériel :** Dans le monde physique, un objet peut être un objet tangible tel qu'une chaise, une voiture, un livre ou un animal. Chaque objet physique possède des caractéristiques spécifiques telles que sa taille, sa forme, sa couleur, son poids, etc.

2. **Objet conceptuel :** Dans le domaine des idées, des concepts ou des disciplines, un objet peut être une entité abstraite telle qu'un concept philosophique, une théorie scientifique, un modèle mathématique ou un projet artistique. Ces objets conceptuels sont définis par leurs caractéristiques intrinsèques et leurs relations avec d'autres concepts ou entités.

En dehors du contexte de la programmation, le terme "objet" est utilisé pour désigner une vaste gamme d'entités, qu'elles soient matérielles ou immatérielles, concrètes ou abstraites. Il est souvent utilisé pour décrire quelque chose de spécifique et identifiable, avec ses propres caractéristiques distinctives.

#### Une classe

En programmation orientée objet (POO), une classe est un modèle ou un plan à partir duquel sont créés les objets. Une classe définit la structure et le comportement d'un type d'objet. Elle agit essentiellement comme un modèle pour créer des instances d'objets qui partagent les mêmes caractéristiques et comportements.

Une classe contient généralement les éléments suivants :

1. **Attributs (variables) :** Ce sont les données membres de la classe qui décrivent l'état de l'objet. Les attributs représentent les propriétés ou les caractéristiques de l'objet.

2. **Méthodes (fonctions) :** Ce sont les actions ou les comportements que l'objet peut effectuer. Les méthodes définissent les opérations que les objets de la classe peuvent effectuer.

3. **Constructeurs :** Ce sont des méthodes spéciales utilisées pour initialiser les objets lors de leur création. Ils permettent de définir comment les objets doivent être initialisés avec des valeurs spécifiques pour leurs attributs.

4. **Destructeurs (dans certains langages) :** Ce sont des méthodes spéciales utilisées pour libérer les ressources allouées par un objet avant sa destruction.

Voici un exemple simple de définition d'une classe en Java :

```java
public class Voiture {
    // Attributs
    String marque;
    String modele;
    int annee;

    // Constructeur
    public Voiture(String marque, String modele, int annee) {
        this.marque = marque;
        this.modele = modele;
        this.annee = annee;
    }

    // Méthode
    public void afficherDetails() {
        System.out.println("Marque : " + marque);
        System.out.println("Modèle : " + modele);
        System.out.println("Année : " + annee);
    }
}
```

### Création d'une class

Pour créer une classe en Java, vous devez suivre quelques étapes simples :

1. **Déclaration de la classe :** Vous déclarez une classe en utilisant le mot-clé `class`, suivi du nom de la classe. Par exemple :
   ```java
   public class MaClasse {
       // Corps de la classe
   }
   ```

2. **Définition des attributs :** À l'intérieur de la classe, vous définissez les attributs (variables) qui représentent l'état de l'objet. Par exemple :
   ```java
   public class MaClasse {
       // Attributs
       int attribut1;
       String attribut2;
       // Autres attributs...
   }
   ```

3. **Définition des méthodes :** Vous définissez les méthodes (fonctions) qui définissent le comportement de l'objet. Par exemple :
   ```java
   public class MaClasse {
       // Attributs
       int attribut1;
       String attribut2;

       // Méthodes
       public void methode1() {
           // Corps de la méthode
       }

       public int methode2() {
           // Corps de la méthode
           return 0;
       }
       // Autres méthodes...
   }
   ```

4. **Définition des constructeurs :** Vous pouvez définir un ou plusieurs constructeurs pour initialiser les objets de la classe. Par exemple :
   ```java
   public class MaClasse {
       // Attributs
       int attribut1;
       String attribut2;
       
       // Constructeur par défaut
       public MaClasse() {
           // Corps du constructeur
       }
       
       // Constructeur avec paramètres
       public MaClasse(int valeur1, String valeur2) {
           this.attribut1 = valeur1;
           this.attribut2 = valeur2;
       }
       // Autres constructeurs...
   }
   ```

5. **Définition des autres éléments de la classe :** Selon les besoins, vous pouvez ajouter d'autres éléments tels que des méthodes statiques, des méthodes de classe, des classes internes, etc.

Voici un exemple complet de création d'une classe en Java avec des attributs, des méthodes et des constructeurs :

```java
public class MaClasse {
    // Attributs
    int attribut1;
    String attribut2;
    
    // Constructeur par défaut
    public MaClasse() {
        // Corps du constructeur
    }
    
    // Constructeur avec paramètres
    public MaClasse(int valeur1, String valeur2) {
        this.attribut1 = valeur1;
        this.attribut2 = valeur2;
    }
    
    // Méthode
    public void afficherDetails() {
        System.out.println("Attribut 1 : " + attribut1);
        System.out.println("Attribut 2 : " + attribut2);
    }
}
```

#### Créer un object

Pour créer un objet à partir d'une classe en Java, vous devez suivre ces étapes :

1. **Déclarez une classe :** Vous avez déjà créé une classe dans l'étape précédente. Assurez-vous que la classe est correctement déclarée avec ses attributs, ses méthodes et ses constructeurs.

2. **Utilisez le mot-clé `new` pour créer un objet :** Vous pouvez utiliser le mot-clé `new` suivi du nom de la classe et de ses arguments de constructeur (le cas échéant) pour créer un nouvel objet de cette classe. Par exemple :
   ```java
   MaClasse monObjet = new MaClasse();
   ```
   ou avec un constructeur prenant des paramètres :
   ```java
   MaClasse monObjet = new MaClasse(valeur1, valeur2);
   ```


#### Les types d'attribue

Les types d'attributs d'une classe en Java peuvent être classés en plusieurs catégories en fonction de leur visibilité, de leur utilisation et de leur portée. Voici les principaux types d'attributs que l'on retrouve dans une classe :

1. **Attributs d'instance :** Ce sont des attributs qui sont associés à chaque instance (objet) de la classe. Chaque objet a sa propre copie des attributs d'instance. Ils sont déclarés à l'intérieur de la classe mais à l'extérieur de toute méthode, et sont accessibles via des méthodes d'instance. Par exemple :
   ```java
   public class MaClasse {
       // Attribut d'instance
       private int attributInstance;
       
       // Méthode d'instance pour accéder à l'attribut d'instance
       public int getAttributInstance() {
           return attributInstance;
       }
   }
   ```

2. **Attributs statiques (ou attributs de classe) :** Ce sont des attributs qui sont partagés par toutes les instances de la classe. Ils sont déclarés avec le mot-clé `static` et sont associés à la classe elle-même plutôt qu'à des instances individuelles. Par conséquent, ils sont accessibles sans avoir besoin de créer une instance de la classe. Par exemple :
   ```java
   public class MaClasse {
       // Attribut statique
       private static int attributStatique;

       // Méthode statique pour accéder à l'attribut statique
       public static int getAttributStatique() {
           return attributStatique;
       }
   }
   ```

3. **Attributs de visibilité :** Les attributs peuvent avoir différentes visibilités, contrôlant ainsi leur accessibilité depuis d'autres classes. Les principales visibilités sont `public`, `protected`, `private` et la visibilité par défaut (si aucun modificateur n'est spécifié). Par exemple :
   ```java
   public class MaClasse {
       public int attributPublic; // Visible depuis n'importe quelle classe
       protected int attributProtected; // Visible dans la même classe, les sous-classes et le même paquetage
       private int attributPrivate; // Visible uniquement dans la même classe
       int attributParDefaut; // Visible uniquement dans le même paquetage
   }
   ```

4. **Attributs finals :** Les attributs finals sont des attributs dont la valeur ne peut pas être modifiée une fois qu'elle a été initialisée. Ils peuvent être initialisés lors de leur déclaration ou dans le constructeur de la classe. Par exemple :
   ```java
   public class MaClasse {
       private final int attributFinal = 10; // Attribut final avec initialisation immédiate
       
       // Attribut final avec initialisation dans le constructeur
       private final String autreAttributFinal;
       
       public MaClasse(String valeur) {
           this.autreAttributFinal = valeur;
       }
   }
   ```

En utilisant ces différents types d'attributs, vous pouvez modéliser différentes caractéristiques et comportements dans vos classes Java en fonction des besoins de votre application.


#### Les types de methodes

Dans une classe Java, les méthodes (ou fonctions) peuvent être classées en plusieurs catégories en fonction de leur utilité et de leur portée. Voici les principaux types de méthodes que l'on retrouve dans une classe :

1. **Méthodes d'instance :** Ce sont des méthodes qui agissent sur les données spécifiques d'une instance (objet) de la classe. Elles sont déclarées sans le mot-clé `static` et peuvent accéder aux attributs d'instance de la classe. Ces méthodes sont appelées sur des objets particuliers de la classe. Par exemple :
   ```java
   public class MaClasse {
       // Attribut d'instance
       private int attributInstance;
       
       // Méthode d'instance
       public void methodeInstance() {
           // Corps de la méthode
           System.out.println("La valeur de l'attribut d'instance est : " + attributInstance);
       }
   }
   ```

2. **Méthodes statiques :** Ce sont des méthodes qui sont associées à la classe elle-même plutôt qu'à des instances individuelles. Elles sont déclarées avec le mot-clé `static` et peuvent accéder uniquement aux attributs statiques de la classe. Ces méthodes sont appelées sur la classe elle-même, sans avoir besoin de créer une instance de la classe. Par exemple :
   ```java
   public class MaClasse {
       // Attribut statique
       private static int attributStatique;
       
       // Méthode statique
       public static void methodeStatique() {
           // Corps de la méthode
           System.out.println("La valeur de l'attribut statique est : " + attributStatique);
       }
   }
   ```

3. **Constructeurs :** Ce sont des méthodes spéciales utilisées pour initialiser les objets lors de leur création. Les constructeurs ont le même nom que la classe et peuvent prendre des paramètres pour initialiser les attributs de l'objet. Par exemple :
   ```java
   public class MaClasse {
       // Constructeur par défaut
       public MaClasse() {
           // Corps du constructeur
       }
       
       // Constructeur avec paramètres
       public MaClasse(int valeur) {
           // Initialisation des attributs avec les valeurs passées en paramètre
       }
   }
   ```

4. **Méthodes de classe (ou méthodes utilitaires) :** Ce sont des méthodes qui effectuent des opérations indépendantes des attributs spécifiques d'une instance. Elles sont généralement utilisées pour effectuer des opérations de traitement de données ou d'assistance. Par exemple :
   ```java
   public class MaClasse {
       // Méthode de classe
       public static int additionner(int a, int b) {
           return a + b;
       }
   }
   ```

5. **Méthodes d'assistance :** Ce sont des méthodes privées utilisées à l'intérieur de la classe pour effectuer des tâches spécifiques. Elles sont souvent utilisées pour réduire la duplication de code et améliorer la lisibilité du code en regroupant des opérations communes. Ces méthodes ne sont pas accessibles en dehors de la classe. Par exemple :
   ```java
   public class MaClasse {
       // Méthode d'assistance privée
       private void faireQuelqueChose() {
           // Corps de la méthode
       }
   }
   ```

#### Les modificateurs

En Java, les modificateurs sont des mots-clés utilisés pour spécifier la portée, le comportement et d'autres caractéristiques des classes, des méthodes, des attributs et d'autres éléments du code. Voici une liste des principaux modificateurs en Java :

### Modificateurs d'accès :

1. **public :** L'élément est accessible partout, à la fois à l'intérieur et à l'extérieur de la classe, du package et du projet.
   
2. **protected :** L'élément est accessible dans la classe elle-même, dans les sous-classes (même si elles sont dans un package différent) et dans le même package.

3. **private :** L'élément est accessible uniquement dans la classe elle-même.

4. **default (ou package-private) :** L'élément est accessible uniquement dans le même package. Si aucun modificateur d'accès n'est spécifié, il est par défaut package-private.

### Modificateurs de non-accessibilité :

1. **final :** Le mot-clé final est utilisé pour indiquer que l'élément ne peut pas être redéfini (pour les méthodes et les classes) ou réassigné (pour les variables).

2. **abstract :** Le mot-clé abstract est utilisé pour indiquer que la méthode ou la classe est déclarée mais n'est pas implémentée dans la classe actuelle et doit être implémentée dans les sous-classes (pour les méthodes) ou ne peut pas être instanciée directement (pour les classes).

3. **static :** Le mot-clé static est utilisé pour déclarer des éléments qui appartiennent à la classe plutôt qu'à une instance spécifique de la classe. Les éléments statiques sont partagés par toutes les instances de la classe.

#### L'héritage


L'héritage est l'un des concepts fondamentaux de la programmation orientée objet (POO). Il permet à une classe (appelée sous-classe ou classe dérivée) de hériter des propriétés et des comportements d'une autre classe (appelée superclasse ou classe de base). En Java, l'héritage est réalisé à l'aide du mot-clé `extends`.

Voici quelques points clés sur l'héritage en Java :

1. **Classe de base (Superclasse) :** La classe dont une autre classe hérite est appelée classe de base ou superclasse. Elle définit les propriétés et les comportements de base que les classes dérivées peuvent utiliser.

2. **Classe dérivée (Sous-classe) :** La classe qui hérite d'une autre classe est appelée classe dérivée ou sous-classe. Elle hérite des propriétés et des comportements de la classe de base et peut également ajouter de nouvelles fonctionnalités ou modifier le comportement existant.

3. **Mot-clé `extends` :** En Java, pour hériter d'une classe, vous utilisez le mot-clé `extends` suivi du nom de la classe de base. Par exemple :
   ```java
   class SousClasse extends SuperClasse {
       // Corps de la classe dérivée
   }
   ```

4. **Héritage simple :** En Java, seule l'héritage simple est pris en charge, ce qui signifie qu'une classe ne peut hériter que d'une seule classe de base.

5. **Constructeurs et méthodes hérités :** Les constructeurs et les méthodes publics de la classe de base sont hérités par la classe dérivée et peuvent être utilisés comme s'ils appartenaient à la classe dérivée. Cependant, les constructeurs de la classe de base ne sont pas hérités.

6. **Redéfinition (ou surcharge) de méthodes :** Une classe dérivée peut redéfinir (ou surcharger) les méthodes de la classe de base pour fournir une implémentation spécifique à la classe dérivée. Cela permet la personnalisation du comportement dans les sous-classes.

Voici un exemple simple d'héritage en Java :

```java
// Classe de base
class Animal {
    void crier() {
        System.out.println("L'animal crie !");
    }
}

// Classe dérivée
class Chien extends Animal {
    void crier() {
        System.out.println("Le chien aboie !");
    }
}

// Classe dérivée
class Chat extends Animal {
    void crier() {
        System.out.println("Le chat miaule !");
    }
}

public class Main {
    public static void main(String[] args) {
        Animal animal1 = new Chien();
        Animal animal2 = new Chat();
        
        animal1.crier(); // Le chien aboie !
        animal2.crier(); // Le chat miaule !
    }
}
```

Dans cet exemple, les classes `Chien` et `Chat` héritent de la classe `Animal` et redéfinissent la méthode `crier()` pour fournir des implémentations spécifiques. Lorsque nous créons des objets de type `Animal`, nous pouvons les utiliser pour appeler la méthode `crier()` qui sera exécutée selon le type réel de l'objet.

#### Encapculation

L'encapsulation est l'un des principes fondamentaux de la programmation orientée objet (POO) et fait partie des concepts clés qui contribuent à la création de code robuste et modulaire. L'encapsulation consiste à regrouper les données (attributs) et les méthodes qui les manipulent au sein d'une même entité, appelée classe. Les données sont cachées et ne sont pas accessibles directement depuis l'extérieur de la classe. Au lieu de cela, l'accès et la manipulation des données se font via des méthodes spéciales appelées "getters" et "setters".

Voici les principaux objectifs de l'encapsulation :

### 1. Protection des données :
Les données d'une classe sont déclarées comme privées, ce qui signifie qu'elles ne peuvent être accédées ou modifiées directement depuis l'extérieur de la classe. Cela protège les données contre les modifications non autorisées et garantit leur intégrité.

### 2. Contrôle d'accès :
L'encapsulation permet de définir des méthodes spéciales, appelées "getters" et "setters", pour accéder et modifier les données d'une classe. Ces méthodes permettent de contrôler l'accès aux données et d'appliquer des règles de validation avant toute modification.

### 3. Modularité :
En regroupant les données et les méthodes qui les manipulent au sein d'une même classe, l'encapsulation favorise la modularité du code. Cela permet de diviser le code en petites unités autonomes, ce qui facilite la maintenance, la réutilisation et l'extension du code.

### 4. Abstraction :
L'encapsulation permet de masquer les détails d'implémentation des données derrière une interface publique. Cela permet aux utilisateurs de la classe de se concentrer sur ce que la classe fait plutôt que sur la manière dont elle le fait, ce qui favorise une meilleure compréhension du code et une plus grande facilité d'utilisation.


#### Les getters et les setters

Les getters et les setters sont des méthodes utilisées pour accéder et modifier les valeurs des attributs (ou des propriétés) d'une classe en Java. Ils sont utilisés pour implémenter le principe d'encapsulation, qui consiste à protéger les attributs d'une classe en les rendant privés et en fournissant des méthodes publiques pour y accéder et les modifier de manière contrôlée.

Voici comment vous pouvez définir des getters et des setters dans une classe Java :

### Exemple de classe avec getters et setters :
```java
public class Personne {
    // Attributs privés
    private String nom;
    private int age;
    
    // Getter pour l'attribut nom
    public String getNom() {
        return nom;
    }
    
    // Setter pour l'attribut nom
    public void setNom(String nom) {
        this.nom = nom;
    }
    
    // Getter pour l'attribut age
    public int getAge() {
        return age;
    }
    
    // Setter pour l'attribut age
    public void setAge(int age) {
        this.age = age;
    }
}
```

Dans cet exemple, la classe `Personne` a deux attributs privés : `nom` et `age`. Pour permettre l'accès à ces attributs depuis l'extérieur de la classe, nous avons défini des getters et des setters correspondants.

- Le getter `getNom()` renvoie la valeur de l'attribut `nom`.
- Le setter `setNom(String nom)` prend un argument de type `String` et met à jour la valeur de l'attribut `nom`.

De manière similaire, nous avons défini des getters et des setters pour l'attribut `age`.

### Utilisation des getters et setters :
```java
public class Main {
    public static void main(String[] args) {
        // Création d'un objet Personne
        Personne personne = new Personne();
        
        // Utilisation des setters pour définir les valeurs des attributs
        personne.setNom("Alice");
        personne.setAge(30);
        
        // Utilisation des getters pour récupérer les valeurs des attributs
        System.out.println("Nom : " + personne.getNom());
        System.out.println("Age : " + personne.getAge());
    }
}
```

Les getters et setters permettent un accès contrôlé aux attributs d'une classe, ce qui permet de garantir l'encapsulation et de maintenir l'intégrité des données.


#### Héritage

L'héritage est l'un des concepts fondamentaux de la programmation orientée objet (POO) qui permet à une classe (appelée sous-classe ou classe dérivée) d'hériter des propriétés et des comportements d'une autre classe (appelée superclasse ou classe de base). En Java, l'héritage est réalisé à l'aide du mot-clé `extends`.

Voici les principaux points à retenir sur l'héritage en Java :

### 1. Classe de base (Superclasse) :
Une classe de base (ou superclasse) est une classe existante dont une autre classe hérite. Elle définit les propriétés et les comportements généraux que les classes dérivées peuvent utiliser.

### 2. Classe dérivée (Sous-classe) :
Une classe dérivée (ou sous-classe) est une classe qui hérite des propriétés et des comportements d'une classe de base. Elle peut également ajouter de nouvelles fonctionnalités ou modifier le comportement existant.

### 3. Mot-clé `extends` :
En Java, pour hériter d'une classe, vous utilisez le mot-clé `extends` suivi du nom de la classe de base. Par exemple :
```java
class SousClasse extends SuperClasse {
    // Corps de la classe dérivée
}
```

### 4. Héritage simple :
En Java, seul l'héritage simple est pris en charge, ce qui signifie qu'une classe ne peut hériter que d'une seule classe de base. Cependant, une classe de base peut avoir plusieurs classes dérivées.

### 5. Constructeurs et méthodes hérités :
Les constructeurs et les méthodes publics de la classe de base sont hérités par la classe dérivée et peuvent être utilisés comme s'ils appartenaient à la classe dérivée. Cependant, les constructeurs de la classe de base ne sont pas hérités.

### 6. Redéfinition (ou surcharge) de méthodes :
Une classe dérivée peut redéfinir (ou surcharger) les méthodes de la classe de base pour fournir une implémentation spécifique à la classe dérivée. Cela permet la personnalisation du comportement dans les sous-classes.

### 7. Mot-clé `super` :
Le mot-clé `super` est utilisé pour accéder aux membres de la classe parente à l'intérieur de la classe enfant. Il est principalement utilisé pour appeler le constructeur de la classe parente à partir du constructeur de la classe enfant.

L'héritage en Java permet de créer une hiérarchie de classes qui favorise la réutilisabilité du code, la modularité et la facilité de maintenance. Il permet également de partager du code commun entre les classes et d'organiser le code de manière logique et cohérente.



#### Surcharge de methode

La surcharge de méthode est un concept en programmation orientée objet qui permet à une classe d'avoir plusieurs méthodes avec le même nom mais des signatures différentes dans la même classe. La signature d'une méthode comprend son nom et le type et le nombre de ses paramètres. La surcharge de méthode permet à une classe d'avoir des méthodes similaires qui effectuent des tâches différentes en fonction des paramètres qu'elles prennent.

Voici les principaux points à retenir sur la surcharge de méthode en Java :

### 1. Signature de méthode :
La signature d'une méthode comprend son nom et le type et le nombre de ses paramètres. Deux méthodes avec le même nom mais des signatures différentes peuvent coexister dans la même classe grâce à la surcharge de méthode.

### 2. Types de paramètres différents :
Les méthodes surchargées peuvent prendre un nombre différent de paramètres ou des types de paramètres différents.

### 3. Pas de dépendance sur le type de retour :
La surcharge de méthode ne dépend pas du type de retour de la méthode. Deux méthodes peuvent avoir le même nom et la même signature, mais un type de retour différent.

### 4. Exemple de surcharge de méthode en Java :
```java
public class Calculateur {
    // Méthode surchargée pour additionner deux entiers
    public int additionner(int a, int b) {
        return a + b;
    }

    // Méthode surchargée pour additionner trois entiers
    public int additionner(int a, int b, int c) {
        return a + b + c;
    }

    // Méthode surchargée pour additionner deux doubles
    public double additionner(double a, double b) {
        return a + b;
    }
}
```

#### Redéfinition de methode

La redéfinition de méthode (ou overriding en anglais) est un concept clé de la programmation orientée objet qui permet à une classe fille (ou sous-classe) de fournir une implémentation spécifique d'une méthode déjà définie dans sa classe parente (ou superclasse). En d'autres termes, une classe enfant peut remplacer (ou redéfinir) le comportement d'une méthode de sa classe parente pour fournir une implémentation adaptée à ses besoins spécifiques.

Voici les principaux points à retenir sur la redéfinition de méthode en Java :

### 1. Méthodes héritées :
Une classe fille hérite de toutes les méthodes publiques et protégées de sa classe parente. Cela inclut également les méthodes déclarées comme `public` dans l'interface implémentée par la classe parente.

### 2. Redéfinition de méthode :
Une classe fille peut redéfinir une méthode héritée en fournissant une implémentation spécifique dans sa propre classe. Pour ce faire, la signature de la méthode redéfinie (son nom, ses paramètres et son type de retour) doit être identique à celle de la méthode dans la classe parente.

### 3. Annotation `@Override` :
En Java, il est recommandé d'utiliser l'annotation `@Override` lors de la redéfinition d'une méthode pour indiquer explicitement au compilateur que vous avez l'intention de redéfinir une méthode héritée. Cela aide à détecter les erreurs de signature ou de nom de méthode lors de la compilation.

### 4. Utilisation du mot-clé `super` :
Dans la classe fille, vous pouvez utiliser le mot-clé `super` pour appeler la méthode redéfinie de la classe parente. Cela permet à la classe fille d'exécuter le comportement de la méthode de la classe parente avant ou après sa propre implémentation.

Voici un exemple simple de redéfinition de méthode en Java :

```java
class Animal {
    public void faireDuBruit() {
        System.out.println("L'animal fait un bruit");
    }
}

class Chien extends Animal {
    @Override
    public void faireDuBruit() {
        System.out.println("Le chien aboie");
    }
}

public class Main {
    public static void main(String[] args) {
        Animal animal = new Animal();
        animal.faireDuBruit();  // Affiche: L'animal fait un bruit

        Animal chien = new Chien();
        chien.faireDuBruit();   // Affiche: Le chien aboie
    }
}
```



#### Classe abstraite

Une classe abstraite est une classe en Java qui ne peut pas être instanciée directement, ce qui signifie que vous ne pouvez pas créer d'objets à partir d'une classe abstraite. Au lieu de cela, elle sert de modèle pour d'autres classes qui en héritent (ou en étendent), appelées classes concrètes.

Voici les principaux points à retenir sur les classes abstraites en Java :

### 1. Déclaration :
Une classe abstraite est déclarée à l'aide du mot-clé `abstract`. Elle peut avoir des méthodes abstraites (méthodes sans implémentation) ainsi que des méthodes concrètes (méthodes avec implémentation).

### 2. Méthodes abstraites :
Une méthode abstraite est déclarée sans corps, c'est-à-dire sans implémentation. Elle est destinée à être redéfinie (ou implémentée) dans les classes filles. Une classe abstraite peut avoir zéro ou plusieurs méthodes abstraites.

### 3. Méthodes concrètes :
Une classe abstraite peut également contenir des méthodes concrètes (méthodes avec implémentation) qui sont partagées par toutes les classes filles.

### 4. Instanciation interdite :
Comme une classe abstraite ne peut pas être instanciée directement, elle ne peut être utilisée que comme classe parente pour créer d'autres classes. Une classe abstraite peut contenir des constructeurs, mais ils ne peuvent pas être utilisés pour instancier la classe abstraite elle-même.

### 5. Héritage :
Une classe fille (ou sous-classe) d'une classe abstraite doit fournir des implémentations pour toutes les méthodes abstraites héritées de la classe abstraite parente. Sinon, la classe fille doit également être déclarée comme abstraite.

### Exemple :
```java
abstract class Forme {
    // Méthode abstraite pour calculer l'aire de la forme
    abstract double calculerAire();
    
    // Méthode concrète pour afficher le type de forme
    void afficherType() {
        System.out.println("Je suis une forme.");
    }
}

class Rectangle extends Forme {
    double longueur, largeur;
    
    Rectangle(double longueur, double largeur) {
        this.longueur = longueur;
        this.largeur = largeur;
    }
    
    @Override
    double calculerAire() {
        return longueur * largeur;
    }
}
```
#### Le polymorphisme

Le polymorphisme est un concept clé de la programmation orientée objet (POO) qui permet à un même nom de méthode ou d'opérateur d'être utilisé pour effectuer différentes actions en fonction du contexte d'utilisation. En d'autres termes, le polymorphisme permet à un objet de prendre différentes formes.

Il existe deux types principaux de polymorphisme en Java :

1. **Polymorphisme statique (lié à la surcharge de méthodes) :** Il s'agit du polymorphisme qui se produit au moment de la compilation. Il est associé à la surcharge de méthodes, où plusieurs méthodes portent le même nom mais ont des listes de paramètres différentes. Le compilateur détermine quelle méthode appeler en fonction des types des arguments fournis lors de l'appel de la méthode.

2. **Polymorphisme dynamique (lié à l'héritage et à la liaison dynamique) :** Il s'agit du polymorphisme qui se produit au moment de l'exécution. Il est associé à l'héritage et à la substitution de méthodes. Lorsqu'une méthode d'un objet est appelée, Java détermine quelle méthode exécuter en fonction du type réel de l'objet au moment de l'exécution, plutôt que du type déclaré de la référence utilisée pour accéder à l'objet. Cela permet aux méthodes héritées d'être redéfinies dans les classes dérivées, et chaque classe peut fournir son propre comportement pour ces méthodes.

#### Les interfaces

Une interface en Java est une collection de méthodes abstraites et de constantes. Elle fournit un moyen de spécifier un ensemble de méthodes que les classes doivent implémenter. Les interfaces sont similaires aux classes abstraites, mais elles ne peuvent contenir que des méthodes abstraites (méthodes sans corps) et des constantes.

Voici les principaux points à retenir sur les interfaces en Java :

### 1. Déclaration :
Une interface est déclarée à l'aide du mot-clé `interface`. Elle peut contenir des méthodes abstraites, des constantes et, à partir de Java 8, des méthodes par défaut et des méthodes statiques.

### 2. Méthodes abstraites :
Toutes les méthodes d'une interface sont implicitement abstraites, ce qui signifie qu'elles n'ont pas de corps et sont destinées à être redéfinies (ou implémentées) dans les classes qui les implémentent.

### 3. Constantes :
Les constantes dans une interface sont implicitement `public`, `static` et `final`, ce qui signifie qu'elles sont des valeurs constantes qui ne peuvent pas être modifiées.

### 4. Implémentation :
Pour implémenter une interface, une classe doit utiliser le mot-clé `implements` et fournir une implémentation pour toutes les méthodes abstraites de l'interface. Une classe peut implémenter plusieurs interfaces.

### 5. Héritage :
Les interfaces peuvent hériter d'autres interfaces à l'aide du mot-clé `extends`. Une interface peut étendre une ou plusieurs autres interfaces.

### 6. Utilisation :
Les interfaces sont utilisées pour définir des contrats (ou des spécifications) que les classes doivent respecter. Elles sont couramment utilisées pour définir des API (interfaces de programmation d'applications) et des modèles de conception (comme le modèle de conception stratégie).

### Exemple :
```java
// Définition d'une interface
interface Animal {
    void faireDuBruit();
}

// Implémentation de l'interface
class Chien implements Animal {
    @Override
    public void faireDuBruit() {
        System.out.println("Le chien aboie.");
    }
}

class Chat implements Animal {
    @Override
    public void faireDuBruit() {
        System.out.println("Le chat miaule.");
    }
}

public class Main {
    public static void main(String[] args) {
        Animal chien = new Chien();
        chien.faireDuBruit();  // Affiche: Le chien aboie.

        Animal chat = new Chat();
        chat.faireDuBruit();   // Affiche: Le chat miaule.
    }
}
```

