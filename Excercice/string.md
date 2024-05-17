1. **Palindrome** :
   Écrivez une fonction qui prend une chaîne de caractères en entrée et vérifie si elle est un palindrome (lue de la même manière de gauche à droite et de droite à gauche).

2. **Comptage des voyelles** :
   Écrivez une fonction qui prend une chaîne de caractères en entrée et compte le nombre de voyelles qu'elle contient.

3. **Inversion des mots** :
   Écrivez une fonction qui prend une phrase en entrée et inverse l'ordre des mots. Par exemple, "Bonjour tout le monde" devrait devenir "monde le tout Bonjour".

4. **Compression de chaîne** :
   Écrivez une fonction qui prend une chaîne de caractères en entrée et la compresse en remplaçant les séquences consécutives de caractères identiques par le caractère suivi du nombre de répétitions. Par exemple, "aaabbbcccc" devrait devenir "a3b3c4".

5. **Occurrence de sous-chaîne** :
   Écrivez une fonction qui prend deux chaînes de caractères en entrée et compte le nombre d'occurrences de la deuxième chaîne dans la première.

6. **Validation de mot de passe** :
   Écrivez une fonction qui prend un mot de passe en entrée et vérifie s'il répond aux critères de complexité spécifiés (par exemple, longueur minimale, présence de caractères spéciaux, de chiffres, etc.).

7. **Conversion en majuscules/minuscules** :
   Écrivez une fonction qui prend une chaîne de caractères en entrée et la convertit en majuscules ou en minuscules, selon une spécification donnée.

8. **Comptage des mots** :
   Écrivez une fonction qui prend une phrase en entrée et compte le nombre de mots qu'elle contient.

9. **Rotation de chaîne** :
   Écrivez une fonction qui prend une chaîne de caractères en entrée et effectue une rotation des caractères vers la gauche ou vers la droite d'un nombre donné de positions.

10. **Comparaison de chaînes** :
    Écrivez une fonction qui compare deux chaînes de caractères et renvoie si elles sont égales, ou laquelle est plus grande ou plus petite selon l'ordre lexicographique.


####


1. **Recherche de sous-chaîne palindromique la plus longue** :
   Écrivez une fonction qui prend une chaîne de caractères en entrée et renvoie la sous-chaîne palindromique la plus longue qu'elle contient.

2. **Manipulation de gros fichiers texte** :
   Écrivez un programme qui traite de gros fichiers texte, en comptant le nombre de mots, en identifiant les mots les plus fréquents, ou en effectuant d'autres opérations de traitement de texte tout en conservant une utilisation minimale de la mémoire.

3. **Recherche de motifs avec des expressions régulières** :
   Écrivez une fonction qui utilise des expressions régulières pour rechercher des motifs complexes dans une chaîne de caractères, tels que des adresses email valides, des URL, ou des numéros de téléphone.

4. **Analyse syntaxique de code source** :
   Écrivez un programme qui analyse syntaxiquement un fichier source dans un langage de programmation donné, identifiant les fonctions, les variables, les instructions, etc., et génère un rapport structuré.

5. **Cryptographie** :
   Écrivez un programme qui implémente un algorithme de chiffrement ou de hachage, tel que AES, RSA, SHA-256, etc., pour chiffrer ou hacher des chaînes de caractères.

6. **Comparaison de chaînes avec distance de Levenshtein** :
   Écrivez une fonction qui calcule la distance de Levenshtein entre deux chaînes de caractères, c'est-à-dire le nombre minimum d'opérations (insertions, suppressions ou substitutions) nécessaires pour transformer une chaîne en une autre.

7. **Analyseur de logs** :
   Écrivez un programme qui analyse des fichiers de logs de serveur, extrait des informations pertinentes telles que les adresses IP, les codes de statut HTTP, les horodatages, etc., et génère des rapports ou des statistiques.

8. **Compression de texte avancée** :
   Écrivez un programme qui utilise des techniques de compression avancées telles que l'algorithme de compression de Lempel-Ziv-Welch pour compresser de gros fichiers texte de manière efficace.


#### Qu'est ce que je fais?


Considérez le code suivant en Java :

```java
public class TextManipulation {
    
    public static String reverseString(String s) {
        return new StringBuilder(s).reverse().toString();
    }
    
    public static int countVowels(String s) {
        int count = 0;
        for (char c : s.toCharArray()) {
            if ("aeiouAEIOU".indexOf(c) != -1) {
                count++;
            }
        }
        return count;
    }
    
    public static String removeDuplicates(String s) {
        StringBuilder result = new StringBuilder();
        for (int i = 0; i < s.length(); i++) {
            if (result.indexOf(String.valueOf(s.charAt(i))) == -1) {
                result.append(s.charAt(i));
            }
        }
        return result.toString();
    }
    
    public static String capitalizeWords(String s) {
        StringBuilder result = new StringBuilder();
        for (String word : s.split(" ")) {
            result.append(word.substring(0, 1).toUpperCase());
            result.append(word.substring(1));
            result.append(" ");
        }
        return result.toString().trim();
    }
}
```


1. **Exercice : Compter le nombre de voyelles**

   Considérez le code suivant en Java :

   ```java
   public class CountVowels {
       
       public static int countVowels(String s) {
           int count = 0;
           String vowels = "aeiouAEIOU";
           for (int i = 0; i < s.length(); i++) {
               if (vowels.contains(String.valueOf(s.charAt(i)))) {
                   count++;
               }
           }
           return count;
       }
       
       public static void main(String[] args) {
           String input = "Bonjour le monde";
           int result = countVowels(input);
           System.out.println("Le nombre de voyelles dans la chaîne est : " + result);
       }
   }
   ```

   Que fait ce code ?

   a) Compte le nombre de caractères dans la chaîne \
   b) Compte le nombre de voyelles dans la chaîne \
   c) Supprime toutes les voyelles de la chaîne \
   d) Convertit toutes les voyelles en majuscules dans la chaîne

2. **Exercice : Inverser une chaîne de caractères**

   Considérez le code suivant en Java :

   ```java
   public class ReverseString {
       
       public static String reverseString(String s) {
           return new StringBuilder(s).reverse().toString();
       }
       
       public static void main(String[] args) {
           String input = "Hello world";
           String result = reverseString(input);
           System.out.println("La chaîne inversée est : " + result);
       }
   }
   ```

   Que fait ce code ?

   a) Trie la chaîne de caractères par ordre alphabétique \
   b) Supprime tous les espaces de la chaîne de caractères \
   c) Inverse la chaîne de caractères \
   d) Convertit tous les caractères en majuscules dans la chaîne

3. **Exercice : Conversion de température**

   Considérez le code suivant en Java :

   ```java
   public class TemperatureConverter {
       
       public static double convertCelsiusToFahrenheit(double celsius) {
           return (celsius * 9 / 5) + 32;
       }
       
       public static void main(String[] args) {
           double celsius = 25.0;
           double fahrenheit = convertCelsiusToFahrenheit(celsius);
           System.out.println("25 degrés Celsius équivalent à " + fahrenheit + " degrés Fahrenheit.");
       }
   }
   ```


1. **Recherche de motifs dans une chaîne :**
   Écrire un programme qui recherche tous les motifs d'une chaîne de caractères dans une autre chaîne. Par exemple, trouver tous les emplacements des occurrences de "abc" dans une chaîne donnée.

2. **Calcul de la distance d'édition :**
   Écrire un programme qui calcule la distance d'édition entre deux chaînes de caractères. La distance d'édition est le nombre minimum d'opérations nécessaires pour transformer une chaîne en une autre, où une opération peut être une insertion, une suppression ou une substitution d'un caractère.

3. **Recherche du plus long sous-palindrome :**
   Écrire un programme qui trouve le plus long sous-palindrome (une sous-chaîne qui est également un palindrome) dans une chaîne de caractères donnée.

4. **Compression de chaîne :**
   Écrire un programme qui compresse une chaîne de caractères en remplaçant les séquences répétées de caractères par un seul caractère suivi du nombre de répétitions. Par exemple, la chaîne "aaabbbccc" serait compressée en "a3b3c3".

5. **Génération de toutes les permutations :**
   Écrire un programme qui génère toutes les permutations d'une chaîne de caractères donnée. Une permutation est une réarrangement des caractères de la chaîne.

6. **Vérification de l'équilibre des parenthèses :**
   Écrire un programme qui vérifie si une chaîne de caractères contient des parenthèses équilibrées. Une chaîne est équilibrée si chaque parenthèse ouvrante a une parenthèse correspondante fermante et qu'elles apparaissent dans le bon ordre.

7. **Recherche de la plus longue sous-chaîne commune :**
   Écrire un programme qui trouve la plus longue sous-chaîne commune entre deux chaînes de caractères données.

8. **Génération de tous les sous-ensembles :**
   Écrire un programme qui génère tous les sous-ensembles d'une chaîne de caractères donnée. Un sous-ensemble est une collection de caractères pris dans la chaîne originale, dans n'importe quel ordre.
