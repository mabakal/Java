1. **Exercice : Gestion des exceptions**

   Écrivez une méthode `divide(int a, int b)` qui prend deux entiers en entrée et retourne le résultat de la division de `a` par `b`. Gérez l'exception `ArithmeticException` qui se produit lorsque `b` est égal à zéro, en affichant un message d'erreur approprié et en renvoyant `-1`.

2. **Exercice : Utilisation de try-catch**

   Écrivez un programme qui demande à l'utilisateur de saisir un nombre entier. Utilisez un bloc `try-catch` pour capturer l'exception `InputMismatchException` qui se produit si l'utilisateur entre autre chose qu'un entier. Affichez un message d'erreur approprié et demandez à l'utilisateur de saisir à nouveau un entier.

3. **Exercice : Lecture de fichier**

   Écrivez une méthode `readFile(String filename)` qui prend en entrée le nom d'un fichier et affiche le contenu de ce fichier. Gérez l'exception `FileNotFoundException` qui se produit si le fichier spécifié n'existe pas, en affichant un message d'erreur approprié.

4. **Exercice : Fermeture de ressources**

   Modifiez la méthode `readFile(String filename)` de l'exercice précédent pour utiliser un bloc `try-with-resources` afin de garantir que le fichier est fermé correctement même en cas d'erreur lors de sa lecture.

5. **Exercice : Création de fichier**

   Écrivez une méthode `createFile(String filename)` qui prend en entrée le nom d'un fichier et crée ce fichier. Gérez l'exception `IOException` qui se produit si une erreur se produit lors de la création du fichier, en affichant un message d'erreur approprié.

6. **Exercice : Utilisation de throws**

   Modifiez la méthode `divide(int a, int b)` de l'exercice 1 pour qu'elle lance une exception `IllegalArgumentException` si `b` est égal à zéro. Modifiez également le code appelant `divide()` pour gérer cette exception en utilisant un bloc `try-catch`.

7. **Exercice : Gestion personnalisée des exceptions**

   Écrivez une classe `AgeValidator` avec une méthode `validateAge(int age)` qui prend en entrée l'âge d'une personne et lève une exception `InvalidAgeException` si l'âge est inférieur à 0 ou supérieur à 150. Créez une classe `InvalidAgeException` personnalisée qui étend la classe `Exception`. Utilisez cette classe dans un programme pour valider l'âge saisi par l'utilisateur.

8. **Exercice : Gestion des chaînes de caractères nulles**

   Écrivez une méthode `toUpperCase(String str)` qui prend une chaîne de caractères en entrée et la convertit en majuscules. Gérez le cas où la chaîne de caractères est nulle en lançant une exception `NullPointerException`.


### 

**Exercice : Gestion complète des erreurs**

Vous devez écrire un programme qui prend en entrée le nom d'un fichier, lit son contenu, effectue un traitement sur ce contenu, puis écrit le résultat dans un autre fichier. Le programme doit gérer les erreurs suivantes :

1. Si le fichier d'entrée n'existe pas, affichez un message d'erreur et quittez le programme.
2. Si une erreur se produit lors de la lecture du fichier d'entrée, affichez un message d'erreur et quittez le programme.
3. Si une erreur se produit lors du traitement du contenu du fichier d'entrée, affichez un message d'erreur et quittez le programme.
4. Si une erreur se produit lors de l'écriture du résultat dans le fichier de sortie, affichez un message d'erreur et quittez le programme.

Voici les étapes à suivre :

1. Demandez à l'utilisateur de saisir le nom du fichier d'entrée.
2. Ouvrez le fichier d'entrée en lecture.
3. Lisez le contenu du fichier d'entrée.
4. Effectuez un traitement sur le contenu lu (par exemple, convertissez-le en majuscules).
5. Demandez à l'utilisateur de saisir le nom du fichier de sortie.
6. Ouvrez le fichier de sortie en écriture.
7. Écrivez le résultat du traitement dans le fichier de sortie.
8. Fermez les flux d'entrée et de sortie.
9. Gérez les erreurs selon les points énumérés ci-dessus.


1. **Exercice 1 : Gestion d'une exception d'index hors limites**
   
   Écrivez un programme Java qui demande à l'utilisateur de saisir un indice et affiche l'élément correspondant d'un tableau prérempli. Si l'indice saisi est en dehors des limites du tableau, le programme doit lever et gérer une exception appropriée.

2. **Exercice 2 : Gestion d'une exception de division par zéro**
   
   Écrivez une méthode Java `diviser(int a, int b)` qui divise deux nombres entiers `a` et `b` et affiche le résultat. Si `b` est égal à zéro, le programme doit lever et gérer une exception appropriée.

3. **Exercice 3 : Gestion d'une exception de fichier inexistant**
   
   Écrivez un programme Java qui tente de lire un fichier texte spécifié par l'utilisateur. Si le fichier n'existe pas, le programme doit lever et gérer une exception appropriée.

4. **Exercice 4 : Gestion d'une exception d'entrée incorrecte**
   
   Écrivez un programme Java qui demande à l'utilisateur de saisir un nombre entier. Si l'utilisateur saisit une valeur incorrecte (par exemple, une chaîne de caractères au lieu d'un entier), le programme doit lever et gérer une exception appropriée.

5. **Exercice 5 : Gestion d'une exception personnalisée**
   
   Créez une exception personnalisée `ValeurNegativeException` qui est levée lorsque la valeur saisie par l'utilisateur est négative. Écrivez un programme Java qui demande à l'utilisateur de saisir un nombre entier et qui lève cette exception si la valeur est négative.

#### Problèmes

Bien sûr ! Voici un problème qui vous permettra de créer et de gérer une exception personnalisée en Java :

**Problème : Gestion des inscriptions à un événement**

Vous êtes en train de développer un système de gestion des inscriptions pour un événement. Chaque participant doit s'inscrire en fournissant son nom et son âge. Cependant, vous souhaitez appliquer certaines règles lors de l'inscription :

1. Le participant doit avoir au moins 18 ans pour s'inscrire à l'événement.
2. Le nom du participant ne peut pas être vide.

Pour garantir le respect de ces règles, vous décidez de créer une exception personnalisée appelée `InscriptionInvalideException` qui sera levée lorsque les règles ne sont pas respectées.

Votre tâche est de créer cette exception personnalisée et de l'intégrer dans votre programme de gestion des inscriptions. Voici les étapes à suivre :

1. Créez une classe `InscriptionInvalideException` qui étend la classe `Exception`. Cette exception devrait avoir un constructeur prenant un message en paramètre.
2. Dans votre programme de gestion des inscriptions, demandez à l'utilisateur de saisir son nom et son âge.
3. Validez les entrées de l'utilisateur :
   - Si le nom est vide, lancez une `InscriptionInvalideException` avec un message approprié.
   - Si l'âge est inférieur à 18 ans, lancez une `InscriptionInvalideException` avec un message approprié.
4. Capturez et gérez les exceptions levées en affichant un message d'erreur approprié à l'utilisateur.


Bien sûr ! Voici un autre problème qui nécessite la création et la gestion d'une exception personnalisée en Java :

**Problème : Gestion des réservations de billets**

Vous développez un système de réservation de billets en ligne pour un cinéma. Vous souhaitez appliquer certaines règles lors de la réservation :

1. Chaque utilisateur peut réserver au maximum 5 billets à la fois.
2. Le nombre de billets réservés ne peut pas être négatif.

Pour garantir le respect de ces règles, vous décidez de créer une exception personnalisée appelée `ReservationInvalideException` qui sera levée lorsque les règles ne sont pas respectées.

Votre tâche est de créer cette exception personnalisée et de l'intégrer dans votre programme de gestion des réservations. Voici les étapes à suivre :

1. Créez une classe `ReservationInvalideException` qui étend la classe `Exception`. Cette exception devrait avoir un constructeur prenant un message en paramètre.
2. Dans votre programme de gestion des réservations, demandez à l'utilisateur de saisir le nombre de billets qu'il souhaite réserver.
3. Validez le nombre de billets saisi par l'utilisateur :
   - Si le nombre de billets est négatif, lancez une `ReservationInvalideException` avec un message approprié.
   - Si le nombre de billets dépasse 5, lancez une `ReservationInvalideException` avec un message approprié.
4. Capturez et gérez les exceptions levées en affichant un message d'erreur approprié à l'utilisateur.


D'accord, voici un problème plus complexe qui implique la gestion d'exceptions personnalisées dans un contexte de gestion de transactions bancaires :

**Problème : Gestion des transactions bancaires**

Vous développez un système de gestion des transactions bancaires pour une banque en ligne. Le système doit être capable de gérer les opérations courantes telles que les dépôts, les retraits et les transferts entre comptes. Vous souhaitez appliquer certaines règles lors de la gestion des transactions :

1. Le montant d'un retrait ne peut pas être supérieur au solde disponible sur le compte.
2. Le montant d'un transfert entre comptes ne peut pas être supérieur au solde disponible sur le compte source.
3. Toute opération (dépôt, retrait, transfert) avec un montant négatif est invalide.

Pour garantir le respect de ces règles, vous décidez de créer plusieurs exceptions personnalisées :

- `SoldeInsuffisantException` : Levée lorsqu'un montant de transaction dépasse le solde disponible sur le compte.
- `MontantNegatifException` : Levée lorsqu'un montant de transaction est négatif.

Votre tâche est de créer ces exceptions personnalisées et de les intégrer dans votre programme de gestion des transactions bancaires. Voici les étapes à suivre :

1. Créez les classes `SoldeInsuffisantException` et `MontantNegatifException` qui étendent la classe `Exception`.
2. Dans votre programme de gestion des transactions, implémentez les méthodes `depot`, `retrait` et `transfert` qui gèrent les transactions entre les comptes.
3. Validez chaque transaction selon les règles énoncées ci-dessus.
4. Lancez les exceptions personnalisées appropriées si une transaction échoue en raison d'un solde insuffisant ou d'un montant négatif.
5. Capturez et gérez ces exceptions dans votre programme pour fournir des messages d'erreur informatifs aux utilisateurs.

D'accord, voici un autre problème qui implique la création et la gestion d'exceptions personnalisées en Java :

**Problème : Gestion des étudiants et de leurs notes**

Vous développez un système de gestion des étudiants pour une école. Le système doit être capable de stocker des informations sur les étudiants, y compris leur nom, leur numéro d'étudiant et leurs notes dans différentes matières. Vous souhaitez appliquer certaines règles lors de la gestion des notes des étudiants :

1. Chaque note doit être comprise entre 0 et 20 inclusivement.
2. Le nombre de notes pour chaque étudiant est limité à 5.

Pour garantir le respect de ces règles, vous décidez de créer deux exceptions personnalisées :

- `NoteInvalideException` : Levée lorsqu'une note est en dehors de la plage valide.
- `TropDeNotesException` : Levée lorsqu'un étudiant a plus de 5 notes.

Votre tâche est de créer ces exceptions personnalisées et de les intégrer dans votre programme de gestion des étudiants et de leurs notes. Voici les étapes à suivre :

1. Créez les classes `NoteInvalideException` et `TropDeNotesException` qui étendent la classe `Exception`.
2. Implémentez une classe `Etudiant` qui contient les informations sur un étudiant, y compris son nom, son numéro d'étudiant et ses notes.
3. Dans la classe `Etudiant`, implémentez une méthode pour ajouter une note à l'étudiant. Validez la note ajoutée selon les règles spécifiées et lancez les exceptions personnalisées appropriées si nécessaire.
4. Capturez et gérez ces exceptions dans votre programme pour fournir des messages d'erreur informatifs aux utilisateurs.
