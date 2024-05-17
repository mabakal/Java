**Exercice 1 : Multiples de 3 et 5**
Écrivez un programme Java qui calcule la somme de tous les multiples de 3 ou 5 en dessous d'un nombre donné.

**Exercice 2 : Table de multiplication**
Écrivez un programme Java qui affiche la table de multiplication d'un nombre donné jusqu'à 10.

**Exercice 3 : Factorielle**
Écrivez une méthode Java qui calcule la factorielle d'un nombre donné à l'aide d'une boucle.

**Exercice 4 : Nombre premier**
Écrivez un programme Java qui vérifie si un nombre donné est premier.

**Exercice 5 : Suite de Fibonacci**
Écrivez un programme Java qui génère les premiers n termes de la suite de Fibonacci.

**Exercice 6 : Calcul de la moyenne**
Écrivez un programme Java qui calcule la moyenne des nombres donnés par l'utilisateur. Le programme doit demander à l'utilisateur combien de nombres il souhaite entrer, puis lire ces nombres et calculer leur moyenne.

**Exercice 7 : Triangle de Pascal**
Écrivez un programme Java qui affiche les n premières lignes du triangle de Pascal.

**Exercice 8 : Conversion de température**
Écrivez un programme Java qui convertit les températures de Fahrenheit en Celsius et vice versa. Le programme doit demander à l'utilisateur le type de conversion qu'il souhaite effectuer, puis lire la température et afficher le résultat.

**Exercice 9 : Vérification de palindrome**
Écrivez un programme Java qui vérifie si un mot donné par l'utilisateur est un palindrome.

**Exercice 10 : Calcul de la somme des chiffres**
Écrivez un programme Java qui calcule la somme des chiffres d'un nombre donné par l'utilisateur.



**Question 1 :**
Considérez le code suivant :

```java
int sum = 0;
for (int i = 1; i <= 5; i++) {
    sum += i;
}
System.out.println("La somme est : " + sum);
```

Quelle est la sortie de ce code ?

a) La somme est : 15
b) La somme est : 10
c) La somme est : 5
d) La somme est : 25

**Question 2 :**
Considérez le code suivant :

```java
int i = 0;
while (i < 5) {
    System.out.print(i + " ");
    i += 2;
}
```

Quelle est la sortie de ce code ?

a) 0 1 2 3 4 
b) 0 2 4 
c) 0 1 2 3 
d) 0 2 4 6 

**Question 3 :**
Considérez le code suivant :

```java
int i = 5;
do {
    System.out.print(i + " ");
    i -= 2;
} while (i > 0);
```

Quelle est la sortie de ce code ?

a) 5 3 1 
b) 5 3 
c) 5 2 
d) 5 2 0 

**Question 4 :**
Considérez le code suivant :

```java
for (int i = 0; i < 10; i++) {
    if (i % 2 == 0) {
        continue;
    }
    System.out.print(i + " ");
}
```

Quelle est la sortie de ce code ?

a) 0 1 2 3 4 5 6 7 8 9 
b) 0 2 4 6 8 
c) 1 3 5 7 9 
d) Aucune des réponses ci-dessus

**Question 5 :**
Considérez le code suivant :

```java
int i = 10;
while (i > 0) {
    System.out.print(i + " ");
    i--;
    if (i == 5) {
        break;
    }
}
```

Quelle est la sortie de ce code ?

a) 10 9 8 7 6 5 
b) 10 9 8 7 
c) 10 9 8 
d) Aucune des réponses ci-dessus


**Question 1 :**
Considérez le code suivant :

```java
int num = 6;
for (int i = 1; i <= num; i++) {
    for (int j = 1; j <= i; j++) {
        System.out.print(j + " ");
    }
    System.out.println();
}
```

Quelle est la sortie de ce code ?

a) 1 2 3 4 5 6 
   1 2 3 4 5 
   1 2 3 4 
   1 2 3 
   1 2 
   1 

b) 1 
   1 2 
   1 2 3 
   1 2 3 4 
   1 2 3 4 5 
   1 2 3 4 5 6 

c) 1 
   1 2 
   1 2 3 
   1 2 3 4 
   1 2 3 4 5 
   1 2 3 4 5 6 

d) Aucune des réponses ci-dessus

**Question 2 :**
Considérez le code suivant :

```java
int n = 5;
int sum = 0;
int i = 1;
do {
    sum += i * i;
    i++;
} while (i <= n);
System.out.println("La somme des carrés des " + n + " premiers nombres est : " + sum);
```

Quelle est la sortie de ce code ?

a) La somme des carrés des 5 premiers nombres est : 55
b) La somme des carrés des 5 premiers nombres est : 30
c) La somme des carrés des 5 premiers nombres est : 15
d) La somme des carrés des 5 premiers nombres est : 5

**Question 3 :**
Considérez le code suivant :

```java
int num = 5;
for (int i = 1; i <= num; i++) {
    for (int j = 1; j <= num - i; j++) {
        System.out.print(" ");
    }
    for (int k = 1; k <= i; k++) {
        System.out.print("* ");
    }
    System.out.println();
}
```

Quelle est la sortie de ce code ?

a) 
     * 
    * * 
   * * * 
  * * * * 
 * * * * * 

b) 
 * * * * * 
  * * * * 
   * * * 
    * * 
     * 

c) 
 * 
 * * 
 * * * 
 * * * * 
 * * * * * 

d) Aucune des réponses ci-dessus


### QCM


1. Quelle est la structure répétitive qui exécute un bloc de code tant qu'une condition est vraie ?
   a) La boucle for
   b) La boucle while
   c) La boucle do-while
   d) L'instruction break

2. Quelle est la différence principale entre la boucle "while" et la boucle "do-while" en Java ?
   a) La boucle "while" est exécutée au moins une fois, tandis que la boucle "do-while" peut ne pas être exécutée du tout.
   b) La boucle "do-while" est exécutée au moins une fois, tandis que la boucle "while" peut ne pas être exécutée du tout.
   c) La boucle "while" peut avoir une condition d'arrêt, tandis que la boucle "do-while" ne peut pas.
   d) Il n'y a pas de différence entre les deux.

3. Quelle boucle est recommandée lorsque le nombre d'itérations est connu à l'avance ?
   a) La boucle for
   b) La boucle while
   c) La boucle do-while
   d) L'instruction break

4. Quelle est la structure utilisée pour interrompre l'exécution d'une boucle de manière anticipée ?
   a) L'instruction continue
   b) L'instruction break
   c) L'instruction return
   d) L'instruction exit

5. Comment s'appelle le processus consistant à répéter une série d'instructions un nombre fixe de fois ?
   a) Itération
   b) Incrémentation
   c) Bouclage
   d) Looping

6. Quelle est la syntaxe correcte d'une boucle "for" en Java ?
   a) for (initialisation; condition; mise à jour) { }
   b) for (initialisation; condition) { }
   c) for (condition; mise à jour) { }
   d) for (initialisation) { }

7. Quelle est la syntaxe correcte d'une boucle "while" en Java ?
   a) while (condition) { }
   b) while (initialisation; condition; mise à jour) { }
   c) while (initialisation) { }
   d) while { }

8. Quelle est la syntaxe correcte d'une boucle "do-while" en Java ?
   a) do { } while (condition);
   b) do (condition) { } while;
   c) do while (condition) { };
   d) do while { } (condition);

9. Quelle boucle est la plus appropriée lorsque le bloc de code doit être exécuté au moins une fois ?
   a) La boucle for
   b) La boucle while
   c) La boucle do-while
   d) L'instruction break

10. Quel est l'opérateur utilisé pour augmenter la valeur d'une variable de 1 dans une boucle ?
    a) ++
    b) --
    c) +=
    d) *=

### QCM


Considérez le code suivant :

```java
int[] tableau = {1, 2, 3, 4, 5};
int somme = 0;

for (int i = 0; i < tableau.length; i++) {
    somme += tableau[i];
}

System.out.println("La somme des éléments du tableau est : " + somme);
```

Quelle est la sortie de ce code ?

a) "La somme des éléments du tableau est : 15"
b) "La somme des éléments du tableau est : 10"
c) "La somme des éléments du tableau est : 5"
d) "La somme des éléments du tableau est : 0"


Question 1:
```java
int[] tableau = {1, 2, 3, 4, 5};
int somme = 0;

for (int i = 0; i < tableau.length; i++) {
    somme += tableau[i];
}

System.out.println("La somme des éléments du tableau est : " + somme);
```
Quelle est la sortie de ce code ?

a) "La somme des éléments du tableau est : 15"
b) "La somme des éléments du tableau est : 10"
c) "La somme des éléments du tableau est : 5"
d) "La somme des éléments du tableau est : 0"



---

Question 2:
```java
int i = 5;
while (i > 0) {
    System.out.print(i + " ");
    i--;
}
```
Quelle est la sortie de ce code ?

a) 5 4 3 2 1
b) 1 2 3 4 5
c) 5 4 3 2
d) 1 2 3 4


---

Question 3:
```java
int somme = 0;
do {
    somme += 2;
} while (somme < 10);
System.out.println(somme);
```
Quelle est la sortie de ce code ?

a) 8
b) 10
c) 12
d) 14


---

Question 4:
```java
int[] nombres = {1, 2, 3, 4, 5};
int somme = 0;
for (int nombre : nombres) {
    somme += nombre;
}
System.out.println(somme);
```
Quelle est la sortie de ce code ?

a) 15
b) 5
c) 10
d) 25
