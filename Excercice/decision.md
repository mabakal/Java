**Exercice 1 : Maximum de deux nombres**
Écrivez un programme Java qui prend deux nombres entiers en entrée et affiche le plus grand des deux.

**Exercice 2 : Jour de la semaine**
Écrivez un programme Java qui prend un numéro de jour de la semaine (entre 1 et 7) en entrée et affiche le nom du jour correspondant (par exemple, 1 pour "Lundi", 2 pour "Mardi", etc.).

**Exercice 3 : Équation du second degré**
Écrivez un programme Java qui résout une équation du second degré de la forme ax^2 + bx + c = 0 en demandant à l'utilisateur d'entrer les coefficients a, b et c, puis en affichant les solutions réelles de l'équation.

**Exercice 4 : Parité d'un nombre**
Écrivez un programme Java qui vérifie si un nombre donné par l'utilisateur est pair ou impair, et affiche un message approprié.

**Exercice 5 : Classement des étudiants**
Écrivez un programme Java qui prend la note d'un étudiant en entrée et affiche un message indiquant s'il a réussi ou échoué. Un étudiant réussit s'il a obtenu une note supérieure ou égale à 50.

**Exercice 6 : Conversion de notes**
Écrivez un programme Java qui prend une note d'un étudiant en entrée et affiche sa note sous forme de lettre en utilisant la notation américaine (A, B, C, D, F). Utilisez les règles de notation suivantes :
- A : 90-100
- B : 80-89
- C : 70-79
- D : 60-69
- F : 0-59

**Exercice 7 : Détermination de l'âge**
Écrivez un programme Java qui prend l'année de naissance d'une personne en entrée et affiche son âge en fonction de l'année actuelle.

**Exercice 8 : Calcul du périmètre d'un rectangle**
Écrivez un programme Java qui prend la longueur et la largeur d'un rectangle en entrée et affiche son périmètre.

**Exercice 9 : Vérification de l'éligibilité à voter**
Écrivez un programme Java qui prend l'âge d'une personne en entrée et vérifie si elle est éligible à voter (âge >= 18 ans) ou non.

**Exercice 10 : Calcul de l'indice de masse corporelle (IMC)**
Écrivez un programme Java qui prend le poids (en kilogrammes) et la taille (en mètres) d'une personne en entrée et calcule son indice de masse corporelle (IMC), puis affiche une catégorie correspondant à l'IMC (par exemple, "Poids insuffisant", "Poids normal", "Surpoids", etc.).

**break :** Le mot-clé `break` est utilisé pour interrompre l'exécution d'une boucle et sortir de celle-ci immédiatement. Il est généralement utilisé pour sortir prématurément d'une boucle lorsque certaines conditions sont rencontrées.

**Exemple :**
```java
for (int i = 0; i < 10; i++) {
    if (i == 5) {
        break; // Sort de la boucle lorsque i vaut 5
    }
    System.out.println(i);
}
```
Dans cet exemple, la boucle `for` s'arrête lorsque `i` atteint la valeur 5. Sans le `break`, la boucle continuerait jusqu'à ce que `i` atteigne 10.

**continue :** Le mot-clé `continue` est utilisé pour passer à l'itération suivante d'une boucle, en sautant le reste du code à l'intérieur de la boucle pour l'itération actuelle. Il est généralement utilisé pour éviter l'exécution d'une partie du code dans certaines conditions.

**Exemple :**
```java
for (int i = 0; i < 10; i++) {
    if (i % 2 == 0) {
        continue; // Passe à l'itération suivante si i est pair
    }
    System.out.println(i);
}
```
Dans cet exemple, la boucle `for` affiche uniquement les nombres impairs. Lorsque `i` est pair, le `continue` est exécuté, sautant l'affichage du nombre pair.

**Exercice 1 :**
Écrivez un programme Java qui utilise une boucle `for` pour afficher les nombres de 1 à 10, mais arrêtez-vous et quittez la boucle dès que vous rencontrez le nombre 5 en utilisant `break`.

**Exercice 2 :**
Écrivez un programme Java qui utilise une boucle `while` pour afficher les nombres de 1 à 10, en sautant l'affichage des nombres pairs en utilisant `continue`.

**Exercice 3 :**
Écrivez un programme Java qui utilise une boucle `do-while` pour demander à l'utilisateur de deviner un nombre entre 1 et 10. Si l'utilisateur devine le nombre correctement, affichez "Bravo !" et sortez de la boucle en utilisant `break`. Si la devinette est incorrecte, continuez la boucle en demandant à nouveau une nouvelle devinette.

Ces exercices vous aideront à comprendre comment utiliser les mots-clés `break` et `continue` pour contrôler le flux d'exécution dans les boucles en Java.


### QCM



1. Quelle structure est utilisée pour exécuter une action si une condition est vraie et une autre action si la condition est fausse ?
   a) La boucle
   b) La fonction
   c) La condition
   d) L'itération

2. Quel opérateur est utilisé pour vérifier si deux valeurs sont égales en Java ?
   a) ==
   b) !=
   c) =
   d) <>

3. Quel mot-clé est utilisé pour démarrer une structure de décision "if" en Java ?
   a) else
   b) then
   c) do
   d) if

4. Quelle est la syntaxe correcte pour une structure de décision "if" en Java ?
   a) if (condition) { }
   b) { if condition }
   c) condition { if }
   d) { } if condition

5. Quelle est la valeur de vérité de l'expression suivante en Java : `(5 > 3 && 7 < 10)` ?
   a) true
   b) false
   c) Il y a une erreur de syntaxe
   d) Cette expression est invalide

6. Quel mot-clé est utilisé pour exécuter un bloc de code si aucune des conditions précédentes n'est vraie ?
   a) else
   b) elseif
   c) other
   d) otherwise

7. Quelle structure est utilisée pour vérifier plusieurs conditions et exécuter différentes actions en fonction de la condition vérifiée ?
   a) La boucle
   b) L'itération
   c) Le switch
   d) Le if-else-if

8. Dans une structure "switch", quelle est l'action effectuée si aucune des valeurs de cas correspond ?
   a) Une erreur est renvoyée
   b) Le programme se termine
   c) Le bloc "default" est exécuté
   d) La première valeur de cas est utilisée

9. Quelle est la syntaxe correcte pour une structure "switch" en Java ?
   a) switch (expression) { }
   b) { switch expression }
   c) expression { switch }
   d) { } switch expression

10. Quelle est la valeur de vérité de l'expression suivante en Java : `(8 >= 8 || 5 < 3)` ?
    a) true
    b) false
    c) Il y a une erreur de syntaxe
    d) Cette expression est invalide

### QCM

1. Considérez le code suivant :

```java
int x = 10;
int y = 5;
int z;

if (x > y) {
    z = x - y;
} else {
    z = y - x;
}

System.out.println(z);
```

Quelle est la valeur imprimée par ce code ?
   a) 5
   b) 10
   c) 15
   d) -5

2. Considérez le code suivant :

```java
int heure = 14;
String message;

if (heure < 12) {
    message = "Bonjour";
} else if (heure < 18) {
    message = "Bon après-midi";
} else {
    message = "Bonne soirée";
}

System.out.println(message);
```

Quel message est imprimé si `heure = 14` ?
   a) "Bonjour"
   b) "Bon après-midi"
   c) "Bonne soirée"
   d) Aucune des réponses ci-dessus

3. Considérez le code suivant :

```java
int nombre = 25;
String resultat;

resultat = (nombre % 2 == 0) ? "Pair" : "Impair";

System.out.println(resultat);
```

Quel est le résultat imprimé par ce code ?
   a) "Pair"
   b) "Impair"
   c) 0
   d) 1

4. Considérez le code suivant :

```java
int x = 5;
int y = 3;
int z = 0;

z = (x > y) ? x : y;

System.out.println(z);
```

Quelle est la valeur de `z` après l'exécution de ce code ?
   a) 5
   b) 3
   c) 8
   d) 0

5. Considérez le code suivant :

```java
int nombre = 7;

if (nombre % 2 == 0) {
    System.out.println("Le nombre est pair");
} else {
    System.out.println("Le nombre est impair");
}
```

Quel est le résultat imprimé si `nombre = 7` ?
   a) "Le nombre est pair"
   b) "Le nombre est impair"
   c) Aucune sortie
   d) Une erreur se produit
