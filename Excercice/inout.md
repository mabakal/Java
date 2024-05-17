1. **Exercice : Lire et afficher un entier**

   Écrivez un programme Java qui demande à l'utilisateur de saisir un entier, puis affiche cet entier à l'écran.

2. **Exercice : Calculer la somme de deux nombres**

   Écrivez un programme Java qui demande à l'utilisateur de saisir deux nombres, puis calcule et affiche la somme de ces deux nombres.

3. **Exercice : Convertir des degrés Celsius en Fahrenheit**

   Écrivez un programme Java qui demande à l'utilisateur de saisir une température en degrés Celsius, puis convertit cette température en degrés Fahrenheit en utilisant la formule \(F = \frac{9}{5} \times C + 32\), où \(F\) est la température en Fahrenheit et \(C\) est la température en Celsius. Affichez ensuite la température convertie.

4. **Exercice : Vérifier si un nombre est pair ou impair**

   Écrivez un programme Java qui demande à l'utilisateur de saisir un nombre, puis vérifie si ce nombre est pair ou impair. Affichez un message approprié en conséquence.

5. **Exercice : Calculer l'aire d'un rectangle**

   Écrivez un programme Java qui demande à l'utilisateur de saisir la longueur et la largeur d'un rectangle, puis calcule et affiche l'aire de ce rectangle.

6. **Exercice : Vérifier si un mot est un palindrome**

   Écrivez un programme Java qui demande à l'utilisateur de saisir un mot, puis vérifie si ce mot est un palindrome (c'est-à-dire qu'il se lit de la même manière de gauche à droite et de droite à gauche). Affichez un message approprié en conséquence.

7. **Exercice : Calculer la moyenne de plusieurs nombres**

   Écrivez un programme Java qui demande à l'utilisateur de saisir plusieurs nombres (séparés par des espaces), puis calcule et affiche la moyenne de ces nombres.

8. **Exercice : Lire et afficher une ligne de texte**

   Écrivez un programme Java qui demande à l'utilisateur de saisir une ligne de texte, puis affiche cette ligne de texte à l'écran.

9. **Exercice : Vérifier si une année est bissextile**

   Écrivez un programme Java qui demande à l'utilisateur de saisir une année, puis vérifie si cette année est bissextile (c'est-à-dire si elle est divisible par 4 mais pas par 100, sauf si elle est également divisible par 400). Affichez un message approprié en conséquence.

10. **Exercice : Calculer le PGCD de deux nombres**

    Écrivez un programme Java qui demande à l'utilisateur de saisir deux nombres, puis calcule et affiche le plus grand commun diviseur (PGCD) de ces deux nombres.


Considérez le code suivant en Java :

```java
public class Example {

    public static int sum(int a, int b) {
        return a + b;
    }

    public static void main(String[] args) {
        int result = sum(3, 5);
        System.out.println("Le résultat est : " + result);
    }
}
```

Quelle est la sortie de ce programme ?

a) Le résultat est : 8 \
b) Le résultat est : 15 \
c) Le résultat est : 3 + 5 \
d) Le résultat est : 35


---

Considérez le code suivant en Java :

```java
import java.util.Scanner;

public class Example {
    
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("Entrez un nombre : ");
        int number = scanner.nextInt();
        System.out.println("Vous avez entré : " + number);
    }
}
```

Que fait ce programme ?

a) Demande à l'utilisateur d'entrer un mot et affiche le mot entré \
b) Demande à l'utilisateur d'entrer un nombre et affiche le nombre entré \
c) Affiche un message sans demander d'entrée à l'utilisateur \
d) Demande à l'utilisateur d'entrer deux nombres et affiche leur somme



---

Considérez le code suivant en Java :

```java
public class Example {
    
    public static void main(String[] args) {
        String message = "Hello world!";
        System.out.println(message.substring(0, 5));
    }
}
```

Quelle est la sortie de ce programme ?

a) Hello \
b) world \
c) Hello world! \
d) Hello world



---

Considérez le code suivant en Java :

```java
public class Example {
    
    public static void main(String[] args) {
        String text = "apple orange banana";
        String[] fruits = text.split(" ");
        System.out.println(fruits[1]);
    }
}
```

Quelle est la sortie de ce programme ?

a) apple \
b) orange \
c) banana \
d) apple orange banana



---
