1. **Calcul de l'IMC** :
   Écrivez un programme qui demande à l'utilisateur de saisir son poids en kilogrammes et sa taille en mètres, puis calcule et affiche l'Indice de Masse Corporelle (IMC) en utilisant la formule : IMC = poids / (taille * taille).

2. **Conversion de température** :
   Écrivez un programme qui demande à l'utilisateur de saisir une température en degrés Celsius, puis convertit cette température en degrés Fahrenheit en utilisant la formule : Fahrenheit = Celsius * 9/5 + 32.

3. **Calcul de l'aire d'un triangle** :
   Écrivez un programme qui demande à l'utilisateur de saisir la longueur de la base et la hauteur d'un triangle, puis calcule et affiche l'aire du triangle en utilisant la formule : Aire = (Base * Hauteur) / 2.

4. **Calcul de la moyenne** :
   Écrivez un programme qui demande à l'utilisateur de saisir trois nombres, puis calcule et affiche leur moyenne.

5. **Vérification de parité** :
   Écrivez un programme qui demande à l'utilisateur de saisir un nombre, puis détermine et affiche si ce nombre est pair ou impair.

6. **Calcul du carré et du cube** :
   Écrivez un programme qui demande à l'utilisateur de saisir un nombre, puis calcule et affiche son carré et son cube.

7. **Échange de valeurs** :
   Écrivez un programme qui demande à l'utilisateur de saisir deux nombres, puis échange les valeurs de ces deux variables et les affiche.

8. **Calcul de la distance entre deux points** :
   Écrivez un programme qui demande à l'utilisateur de saisir les coordonnées (x, y) de deux points dans un plan cartésien, puis calcule et affiche la distance entre ces deux points en utilisant la formule de la distance euclidienne : distance = √((x2 - x1)² + (y2 - y1)²).

9. **Calcul du volume d'un cylindre** :
   Écrivez un programme qui demande à l'utilisateur de saisir le rayon et la hauteur d'un cylindre, puis calcule et affiche son volume en utilisant la formule : Volume = π * rayon² * hauteur.

10. **Comparaison de chaînes de caractères** :
    Écrivez un programme qui demande à l'utilisateur de saisir deux chaînes de caractères, puis compare ces deux chaînes et affiche si elles sont égales ou non.


##### Analyser et donner la bonne reponse


1. Quel est le résultat de l'exécution de ce code Java ?

```java
public class Exercice1 {
    public static void main(String[] args) {
        int a = 5;
        int b = 2;
        int resultat = a / b;
        System.out.println(resultat);
    }
}
```

a) 2.5 \
b) 2 \
c) 2.5 (avec une erreur de compilation) \
d) Une erreur de division par zéro

2. Quel est le résultat de l'exécution de ce code Java ?

```java
public class Exercice2 {
    public static void main(String[] args) {
        int x = 5;
        int y = 2;
        int resultat = x % y;
        System.out.println(resultat);
    }
}
```

a) 2.5 \
b) 2 \
c) 1 \
d) Une erreur de compilation

3. Quel est le résultat de l'exécution de ce code Java ?

```java
public class Exercice3 {
    public static void main(String[] args) {
        int x = 10;
        int y = 3;
        double resultat = x / y;
        System.out.println(resultat);
    }
}
```

a) 3.3333... \
b) 3 \
c) 3.0 \
d) Une erreur de compilation

4. Quel est le résultat de l'exécution de ce code Java ?

```java
public class Exercice4 {
    public static void main(String[] args) {
        double x = 5.0;
        double y = 2.0;
        double resultat = x / y;
        System.out.println(resultat);
    }
}
```

a) 2.5 \
b) 2 \
c) 2.5 (avec une erreur de compilation) \
d) 2.0

5. Quel est le résultat de l'exécution de ce code Java ?

```java
public class Exercice5 {
    public static void main(String[] args) {
        int a = 7;
        int b = 3;
        int c = 2;
        int resultat = a - b / c;
        System.out.println(resultat);
    }
}
```

a) 5 \
b) 3 \
c) 6 \
d) 2



1. Quel est le résultat de l'exécution de ce code Java ?

```java
public class Exercice1 {
    public static void main(String[] args) {
        int x = 5;
        int y = 3;
        boolean resultat = x <= y;
        System.out.println(resultat);
    }
}
```

a) true \
b) false \
c) Une erreur de compilation \
d) true (avec une erreur de logique)

2. Quel est le résultat de l'exécution de ce code Java ?

```java
public class Exercice2 {
    public static void main(String[] args) {
        int x = 10;
        int y = 8;
        boolean resultat = x != y;
        System.out.println(resultat);
    }
}
```

a) true \
b) false \
c) Une erreur de compilation \
d) true (avec une erreur de logique)

3. Quel est le résultat de l'exécution de ce code Java ?

```java
public class Exercice3 {
    public static void main(String[] args) {
        int x = 5;
        int y = 5;
        boolean resultat = x < y;
        System.out.println(resultat);
    }
}
```

a) true \
b) false \
c) Une erreur de compilation \
d) true (avec une erreur de logique)

4. Quel est le résultat de l'exécution de ce code Java ?

```java
public class Exercice4 {
    public static void main(String[] args) {
        double x = 5.0;
        double y = 5.0;
        boolean resultat = x == y;
        System.out.println(resultat);
    }
}
```

a) true \
b) false \
c) Une erreur de compilation \
d) true (avec une erreur de logique)

5. Quel est le résultat de l'exécution de ce code Java ?

```java
public class Exercice5 {
    public static void main(String[] args) {
        int x = 5;
        int y = 5;
        boolean resultat = x <= y;
        System.out.println(resultat);
    }
}
```

a) true \
b) false \
c) Une erreur de compilation \
d) true (avec une erreur de logique)



1. Quel est le résultat de l'exécution de ce code Java ?

```java
public class Exercice1 {
    public static void main(String[] args) {
        boolean a = true;
        boolean b = false;
        boolean resultat = a && b;
        System.out.println(resultat);
    }
}
```

a) true \
b) false \
c) true (avec une erreur de compilation) \
d) false (avec une erreur de compilation)

2. Quel est le résultat de l'exécution de ce code Java ?

```java
public class Exercice2 {
    public static void main(String[] args) {
        boolean a = true;
        boolean b = false;
        boolean resultat = a || b;
        System.out.println(resultat);
    }
}
```

a) true \
b) false \
c) true (avec une erreur de compilation) \
d) false (avec une erreur de compilation)

3. Quel est le résultat de l'exécution de ce code Java ?

```java
public class Exercice3 {
    public static void main(String[] args) {
        boolean a = true;
        boolean resultat = !a;
        System.out.println(resultat);
    }
}
```

a) true \
b) false \
c) true (avec une erreur de compilation) \
d) false (avec une erreur de compilation)

4. Quel est le résultat de l'exécution de ce code Java ?

```java
public class Exercice4 {
    public static void main(String[] args) {
        boolean a = true;
        boolean b = false;
        boolean resultat = a && !b;
        System.out.println(resultat);
    }
}
```

a) true \
b) false \
c) true (avec une erreur de compilation) \
d) false (avec une erreur de compilation)

5. Quel est le résultat de l'exécution de ce code Java ?

```java
public class Exercice5 {
    public static void main(String[] args) {
        boolean a = false;
        boolean b = false;
        boolean resultat = a || !b;
        System.out.println(resultat);
    }
}
```

a) true \
b) false \
c) true (avec une erreur de compilation) \
d) false (avec une erreur de compilation)

Réponses :
1. b) false
2. a) true
3. b) false
4. a) true
5. a) true


<p>If we list all the natural numbers below $10$ that are multiples of $3$ or 5, we get 3, 5, 6 and 9. The sum of these multiples is 23.</p>
<p>Find the sum of all the multiples of $3$ or $5$ below 1000.</p>
<br/>

<p>Each new term in the Fibonacci sequence is generated by adding the previous two terms. By starting with 1 and 2, the first $10$ terms will be:
1, 2, 3, 5, 8, 13, 21, 34, 55, 89, ...</p>
<p>By considering the terms in the Fibonacci sequence whose values do not exceed four million, find the sum of the even-valued terms.</p>



1. Quelle est la sortie de ce code Java ?

```java
public class Main {
    public static void main(String[] args) {
        int x = 5;
        int y = 2;
        System.out.println(x * y);
    }
}
```

a) 7  
b) 10  
c) 5  
d) 2  

2. Quelle est la sortie de ce code Java ?

```java
public class Main {
    public static void main(String[] args) {
        int x = 10;
        int y = 3;
        System.out.println(x / y);
    }
}
```

a) 3  
b) 3.3333  
c) 3.0  
d) 4  


3. Quelle est la sortie de ce code Java ?

```java
public class Main {
    public static void main(String[] args) {
        int x = 7;
        int y = 2;
        System.out.println(x % y);
    }
}
```

a) 3.5  
b) 1  
c) 3  
d) 2  


4. Quelle est la sortie de ce code Java ?

```java
public class Main {
    public static void main(String[] args) {
        String str1 = "Hello";
        String str2 = "World";
        System.out.println(str1 + " " + str2);
    }
}
```

a) HelloWorld  
b) Hello World  
c) Helloworld  
d) Compilation error  


5. Quelle est la sortie de ce code Java ?

```java
public class Main {
    public static void main(String[] args) {
        int x = 5;
        x++;
        System.out.println(x);
    }
}
```

a) 5  
b) 6  
c) 4  
d) 10  


6. Quelle est la sortie de ce code Java ?

```java
public class Main {
    public static void main(String[] args) {
        int x = 10;
        int y = 3;
        System.out.println(x += y);
    }
}
```

a) 7  
b) 10  
c) 13  
d) 30  


7. Quelle est la sortie de ce code Java ?

```java
public class Main {
    public static void main(String[] args) {
        int x = 7;
        int y = 2;
        System.out.println(x == y);
    }
}
```

a) true  
b) false  
c) 3  
d) Compilation error  


8. Quelle est la sortie de ce code Java ?

```java
public class Main {
    public static void main(String[] args) {
        int x = 5;
        int y = 5;
        System.out.println(x != y);
    }
}
```

a) true  
b) false  
c) 5  
d) Compilation error  


9. Quelle est la sortie de ce code Java ?

```java
public class Main {
    public static void main(String[] args) {
        int x = 10;
        int y = 3;
        System.out.println(x > y);
    }
}
```

a) true  
b) false  
c) 7  
d) Compilation error  


10. Quelle est la sortie de ce code Java ?

```java
public class Main {
    public static void main(String[] args) {
        int x = 5;
        int y = 10;
        System.out.println(x < y);
    }
}
```

a) true  
b) false  
c) 5  
d) Compilation error  


Voici quelques questions à choix multiples (QCM) sur les bases de la programmation en se concentrant sur les variables, les tableaux, les structures de décision, les conditions et les chaînes de caractères :

1. Quel est le type de données utilisé pour stocker des nombres entiers en Java ?
   a) int
   b) float
   c) char
   d) String

2. Quelle est la syntaxe correcte pour déclarer une variable en Java ?
   a) variable x;
   b) var x;
   c) int x;
   d) x = int;

3. Quelle est la valeur initiale d'une variable int en Java si aucune valeur n'est attribuée ?
   a) 0
   b) 1
   c) null
   d) -1

4. Comment accéder au premier élément d'un tableau en Java ?
   a) tableau[0]
   b) tableau[1]
   c) tableau.first()
   d) tableau.get(0)

5. Quelle est la syntaxe pour une condition "si" en Java ?
   a) if(condition) { }
   b) case(condition) { }
   c) when(condition) { }
   d) for(condition) { }

6. Quelle est la différence entre "==" et "=" en Java ?
   a) "==" est utilisé pour assigner une valeur, "=" est utilisé pour comparer des valeurs
   b) "==" est utilisé pour comparer des valeurs, "=" est utilisé pour assigner une valeur
   c) Ils sont utilisés de la même manière en Java
   d) Aucune des réponses ci-dessus

7. Quelle est la méthode pour concaténer des chaînes de caractères en Java ?
   a) concat()
   b) append()
   c) add()
   d) merge()

8. Comment déclarer et initialiser un tableau en Java ?
   a) int[] tableau = new int[];
   b) tableau<int> = new tableau[];
   c) int[] tableau = new int[10];
   d) int tableau = new int[];

9. Quelle est la syntaxe correcte pour une boucle "for" en Java ?
   a) for(i = 0; i < 10; i++) { }
   b) for(int i = 0; i < 10; i++) { }
   c) for(int i = 0; i < 10) { }
   d) for(int i = 10; i > 0; i--) { }

10. Comment comparer deux chaînes de caractères en Java ?
    a) str1.compare(str2)
    b) str1.equals(str2)
    c) str1 == str2
    d) compare(str1, str2)
