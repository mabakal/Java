### Énoncé de l'exercice :
Écrire un programme Java qui permet de résoudre une équation du second degré de la forme ax^2 + bx + c = 0, en demandant à l'utilisateur de saisir les valeurs des coefficients a, b et c, puis en affichant les solutions réelles de l'équation.

### Instructions :
1. Demandez à l'utilisateur de saisir les valeurs des coefficients a, b et c de l'équation.
2. Utilisez la formule quadratique pour calculer les solutions de l'équation :
   - Si le discriminant (b^2 - 4ac) est positif, il existe deux solutions réelles distinctes.
   - Si le discriminant est égal à zéro, il existe une solution réelle double.
   - Si le discriminant est négatif, il n'y a pas de solution réelle.
3. Affichez les solutions réelles de l'équation.

Voici un exemple de sortie attendue :

```
Entrez le coefficient a : 1
Entrez le coefficient b : -3
Entrez le coefficient c : 2
Les solutions de l'équation sont x1 = 2.0 et x2 = 1.0
```

### Conseils :
- Utilisez la formule quadratique : x = (-b ± √(b^2 - 4ac)) / (2a) pour calculer les solutions.
- Utilisez des structures conditionnelles pour gérer les différents cas en fonction du discriminant.


***matrice***

Écrire une fonction qui permet de faire la somme de deux matrices. Cette fonction prend en argument deux matrices de même taille, leur dimension ; elle renvoie une matrice.

***tableau***


Écrire une fonction qui permet de fusionner deux tableaux triés, c'est-à-dire qu'elle retourne le tableau trié contenant les éléments des deux tableaux en entrée. Elle prend en entrée un tableau, sa longueur, un autre tableau, sa longueur ; elle renvoie un tableau.

Cette nouvelle fonction doit avoir une complexité algorithmique aussi faible que possible.

***Transposé***

Ecrire une fonction qui fait la transposé d'une matrice, cette fonction prend en paramètre une matrice et renvoi son transposé


1. **Calcul de la moyenne :**
   Écrire une fonction qui prend en entrée un tableau de nombres réels et renvoie leur moyenne.

2. **Calcul de la médiane :**
   Écrire une fonction qui prend en entrée un tableau de nombres réels et renvoie leur médiane.

3. **Calcul de la variance :**
   Écrire une fonction qui prend en entrée un tableau de nombres réels et renvoie leur variance.

4. **Calcul de l'écart-type :**
   Écrire une fonction qui prend en entrée un tableau de nombres réels et renvoie leur écart-type.

5. **Calcul de la corrélation :**
   Écrire une fonction qui prend en entrée deux tableaux de nombres réels et renvoie leur coefficient de corrélation.


1. **Compter le nombre de caractères dans une chaîne :**
   Écrire une fonction qui prend en entrée une chaîne de caractères et renvoie le nombre total de caractères qu'elle contient.

2. **Inverser une chaîne de caractères :**
   Écrire une fonction qui prend en entrée une chaîne de caractères et renvoie une nouvelle chaîne contenant les mêmes caractères mais dans l'ordre inverse.

3. **Vérifier si une chaîne est un palindrome :**
   Écrire une fonction qui prend en entrée une chaîne de caractères et renvoie vrai si elle est un palindrome (c'est-à-dire qu'elle se lit de la même manière de gauche à droite et de droite à gauche), faux sinon.

4. **Convertir une chaîne en majuscules ou en minuscules :**
   Écrire une fonction qui prend en entrée une chaîne de caractères et renvoie une nouvelle chaîne où tous les caractères sont convertis en majuscules ou en minuscules, selon le choix de l'utilisateur.

5. **Extraire une sous-chaîne :**
   Écrire une fonction qui prend en entrée une chaîne de caractères et deux indices (début et fin) et renvoie la sous-chaîne comprise entre ces indices.

6. **Remplacer un sous-chaîne par une autre :**
   Écrire une fonction qui prend en entrée une chaîne de caractères, une sous-chaîne à rechercher et une chaîne de remplacement, et renvoie une nouvelle chaîne où toutes les occurrences de la sous-chaîne sont remplacées par la chaîne de remplacement.

7. **Découper une chaîne en tokens :**
   Écrire une fonction qui prend en entrée une chaîne de caractères et un délimiteur, et renvoie un tableau contenant les tokens (mots ou sous-chaînes) obtenus en découpant la chaîne en fonction du délimiteur.

8. **Vérifier si une chaîne commence ou se termine par une certaine sous-chaîne :**
   Écrire une fonction qui prend en entrée une chaîne de caractères et une sous-chaîne, et renvoie vrai si la chaîne commence ou se termine par cette sous-chaîne, faux sinon.


### QCM

1. Quelle est la syntaxe pour définir une fonction (méthode) en Java ?
   a) method nomFonction() { }
   b) def nomFonction() { }
   c) fonction nomFonction() { }
   d) returnType nomFonction() { }

2. Comment appeler une fonction définie dans une autre classe en Java ?
   a) functionName();
   b) otherClass.functionName();
   c) functionName(otherClass);
   d) new otherClass.functionName();

3. Quelle est la différence entre une fonction et une méthode en Java ?
   a) Aucune, les deux termes sont interchangeables en Java
   b) Une fonction est définie à l'intérieur d'une classe, tandis qu'une méthode est définie en dehors d'une classe
   c) Une fonction retourne toujours une valeur, tandis qu'une méthode peut ne pas retourner de valeur
   d) Une méthode est définie à l'intérieur d'une classe, tandis qu'une fonction est définie en dehors d'une classe

4. Qu'est-ce qu'un package en Java ?
   a) Une fonctionnalité supplémentaire que vous pouvez ajouter à Java pour étendre ses fonctionnalités
   b) Un ensemble de fichiers contenant des classes connexes
   c) Une méthode pour encapsuler des données et des fonctions
   d) Une collection de méthodes prédéfinies dans Java

5. Quelle est la syntaxe pour importer un package en Java ?
   a) import package.name;
   b) package.import name;
   c) include package.name;
   d) using package.name;

6. Quel est l'avantage d'utiliser des packages en Java ?
   a) Ils permettent de mieux organiser le code en le regroupant par fonctionnalité
   b) Ils rendent le code plus difficile à lire et à comprendre
   c) Ils permettent de limiter l'accès aux classes et aux méthodes
   d) Ils accélèrent l'exécution du programme en regroupant les classes similaires

7. Comment importer toutes les classes d'un package en Java ?
   a) import package.*;
   b) import package.all;
   c) import package.allClasses;
   d) import package.classes.*;

8. Quelle est la différence entre un package et un répertoire (dossier) en Java ?
   a) Il n'y a pas de différence, les deux termes sont interchangeables
   b) Un package est une collection de classes Java, tandis qu'un répertoire est une structure de stockage sur le système de fichiers
   c) Un package est utilisé pour stocker des fichiers HTML, tandis qu'un répertoire est utilisé pour stocker des fichiers Java
   d) Un package est créé avec l'instruction "package", tandis qu'un répertoire est créé avec l'instruction "directory"


### QCM

Bien sûr, voici quelques questions avec des fonctions un peu plus complexes :

1. Considérez la fonction suivante :

```java
public int e(int n) {
    if (n == 0) {
        return 1;
    } else {
        return n * e(n - 1);
    }
}
```

Quelle est la valeur renvoyée par cette fonction lorsque `n = 5` ?
   a) 5
   b) 20
   c) 120
   d) 125

2. Considérez la fonction suivante :

```java
public boolean d(String mot) {
    int debut = 0;
    int fin = mot.length() - 1;
    while (debut < fin) {
        if (mot.charAt(debut) != mot.charAt(fin)) {
            return false;
        }
        debut++;
        fin--;
    }
    return true;
}
```

Quelle est la valeur renvoyée par cette fonction lorsque `mot = "radar"` ?
   a) true
   b) false
   c) Une erreur se produit
   d) "rr"

3. Considérez la fonction suivante :

```java
public int[] c(int[] tableau) {
    Arrays.sort(tableau);
    return tableau;
}
```

Quelle est la valeur renvoyée par cette fonction lorsque `tableau = {3, 1, 4, 1, 5, 9, 2}` ?
   a) {1, 1, 2, 3, 4, 5, 9}
   b) {9, 5, 4, 3, 2, 1, 1}
   c) {3, 1, 4, 1, 5, 9, 2}
   d) Une erreur se produit

4. Considérez la fonction suivante :

```java
public int b(List<Integer> liste) {
    int somme = 0;
    for (int element : liste) {
        somme += element;
    }
    return somme;
}
```

Quelle est la valeur renvoyée par cette fonction lorsque `liste = {2, 4, 6, 8, 10}` ?
   a) 30
   b) 15
   c) 5
   d) Une erreur se produit

5. Considérez la fonction suivante :

```java
public String a(String chaine) {
    StringBuilder resultat = new StringBuilder();
    for (int i = chaine.length() - 1; i >= 0; i--) {
        resultat.append(chaine.charAt(i));
    }
    return resultat.toString();
}
```

Quelle est la valeur renvoyée par cette fonction lorsque `chaine = "Java"` ?
   a) "avaJ"
   b) "Java"
   c) "aavJ"
   d) "avaJva"


