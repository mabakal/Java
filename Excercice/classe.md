### Classes

### Exercice 1 : Création d'une classe Personne
Créez une classe `Personne` avec les attributs `nom`, `âge` et `ville`. Ajoutez des méthodes pour initialiser ces attributs, les récupérer et afficher les détails de la personne.

### Exercice 2 : Création d'une classe Livre
Créez une classe `Livre` avec les attributs `titre`, `auteur` et `année de publication`. Ajoutez des méthodes pour initialiser ces attributs, les récupérer et afficher les détails du livre.

### Exercice 3 : Création d'une classe Animal
Créez une classe `Animal` avec les attributs `nom` et `type`. Ajoutez des méthodes pour initialiser ces attributs, les récupérer et afficher les détails de l'animal.

### Exercice 4 : Création d'une classe CompteBancaire
Créez une classe `CompteBancaire` avec les attributs `solde` et `titulaire`. Ajoutez des méthodes pour créditer et débiter le compte, ainsi que pour afficher le solde.

### Exercice 5 : Création d'une classe Voiture
Créez une classe `Voiture` avec les attributs `marque`, `modèle`, `année de fabrication` et `prix`. Ajoutez des méthodes pour initialiser ces attributs, les récupérer et afficher les détails de la voiture.

### Exercice 6 : Création d'une classe Rectangle
Créez une classe `Rectangle` avec les attributs `longueur` et `largeur`. Ajoutez des méthodes pour calculer le périmètre et la surface du rectangle.

### Exercice 7 : Création d'une classe Étudiant
Créez une classe `Étudiant` avec les attributs `nom`, `âge`, `niveau` et `moyenne`. Ajoutez des méthodes pour initialiser ces attributs, les récupérer et afficher les détails de l'étudiant.

### Exercice 8 : Création d'une classe Cercle
Créez une classe `Cercle` avec l'attribut `rayon`. Ajoutez des méthodes pour calculer la circonférence et la surface du cercle.

### Exercice 9 : Création d'une classe Produit
Créez une classe `Produit` avec les attributs `nom`, `prix` et `quantité`. Ajoutez des méthodes pour initialiser ces attributs, les récupérer et afficher les détails du produit.

### Exercice 10 : Création d'une classe Triangle
Créez une classe `Triangle` avec les attributs `côté1`, `côté2` et `côté3`. Ajoutez des méthodes pour calculer le périmètre et la surface du triangle.

Bien sûr ! Voici quelques exercices sur les classes abstraites en Java :

### Exercice 1 : Formes géométriques
Définissez une classe abstraite `Forme` avec une méthode abstraite `calculerSurface()` et une méthode concrète `afficherDetails()`. Créez ensuite des classes dérivées `Cercle`, `Rectangle` et `Triangle` qui étendent la classe `Forme` et fournissent des implémentations pour la méthode `calculerSurface()`. Testez vos classes en calculant et en affichant la surface de différentes formes.

### Exercice 2 : Employés
Définissez une classe abstraite `Employé` avec des champs `nom`, `salaire` et des méthodes `calculerSalaire()` et `afficherDetails()`. Créez ensuite des classes dérivées `Manager`, `Vendeur` et `Technicien` qui étendent la classe `Employé` et fournissent des implémentations pour la méthode `calculerSalaire()`. Testez vos classes en calculant et en affichant le salaire de différents employés.

### Exercice 3 : Animaux
Définissez une classe abstraite `Animal` avec des méthodes abstraites `crier()` et `manger()`. Créez ensuite des classes dérivées `Chien`, `Chat` et `Oiseau` qui étendent la classe `Animal` et fournissent des implémentations pour les méthodes abstraites. Testez vos classes en faisant crier et manger différents animaux.

### Exercice 4 : Compte bancaire
Définissez une classe abstraite `CompteBancaire` avec des champs `solde`, `numéro de compte` et des méthodes `déposer()` et `retirer()`. Créez ensuite des classes dérivées `CompteCourant` et `CompteÉpargne` qui étendent la classe `CompteBancaire` et fournissent des implémentations pour les méthodes `déposer()` et `retirer()`. Testez vos classes en effectuant des opérations de dépôt et de retrait sur différents types de comptes.

### Exercice 5 : Géométrie 3D
Définissez une classe abstraite `Forme3D` avec des méthodes abstraites `calculerVolume()` et `calculerSurface()`. Créez ensuite des classes dérivées `Cube`, `Sphere` et `Cône` qui étendent la classe `Forme3D` et fournissent des implémentations pour les méthodes abstraites. Testez vos classes en calculant et en affichant le volume et la surface de différentes formes géométriques 3D.


**Problème : Gestion d'une bibliothèque**

Vous développez un système de gestion pour une bibliothèque. Le système doit être capable de gérer les livres, les membres et les emprunts. Chaque livre a un titre, un auteur et un numéro ISBN unique. Chaque membre de la bibliothèque a un nom, un numéro de membre et peut emprunter des livres. Chaque emprunt est associé à un membre et à un livre, et comporte une date de début et une date de retour prévue.

Votre tâche est de concevoir et d'implémenter les classes Java nécessaires pour ce système de gestion de bibliothèque. Voici les exigences spécifiques :

1. **Classe Livre :**
   - Attributs : titre, auteur, ISBN
   - Méthodes :
     - Constructeur pour initialiser les attributs.
     - Méthodes getters pour chaque attribut.

2. **Classe Membre :**
   - Attributs : nom, numéro de membre
   - Méthodes :
     - Constructeur pour initialiser les attributs.
     - Méthodes getters pour chaque attribut.

3. **Classe Emprunt :**
   - Attributs : membre, livre, date de début, date de retour prévue
   - Méthodes :
     - Constructeur pour initialiser les attributs.
     - Méthodes getters pour chaque attribut.

4. **Classe Bibliotheque :**
   - Attributs : liste des livres disponibles, liste des membres, liste des emprunts en cours
   - Méthodes :
     - Méthode pour ajouter un livre à la bibliothèque.
     - Méthode pour ajouter un membre à la bibliothèque.
     - Méthode pour permettre à un membre d'emprunter un livre.
     - Méthode pour afficher les livres disponibles.
     - Méthode pour afficher les membres de la bibliothèque.
     - Méthode pour afficher les emprunts en cours.

Implémentez ces classes en Java et testez-les dans un programme principal. Assurez-vous de valider votre code en ajoutant des livres, des membres et en effectuant des emprunts. Assurez-vous également de gérer les cas où un membre essaie d'emprunter un livre déjà emprunté, ou lorsque les dates de retour sont dépassées.


**Problème : Gestion d'un système de réservation de billets d'avion**

Vous développez un système de réservation de billets d'avion pour une compagnie aérienne. Le système doit être capable de gérer les vols, les passagers et les réservations. Chaque vol a un numéro de vol, une destination et une capacité maximale de passagers. Chaque passager a un nom, un numéro de réservation et peut réserver un ou plusieurs billets pour un vol. Chaque réservation est associée à un passager et à un vol.

Votre tâche est de concevoir et d'implémenter les classes Java nécessaires pour ce système de réservation de billets d'avion. Voici les exigences spécifiques :

1. **Classe Vol :**
   - Attributs : numéro de vol, destination, capacité maximale de passagers, liste des réservations
   - Méthodes :
     - Constructeur pour initialiser les attributs.
     - Méthodes pour ajouter une réservation à un vol et vérifier la disponibilité des places.

2. **Classe Passager :**
   - Attributs : nom, numéro de réservation
   - Méthodes :
     - Constructeur pour initialiser les attributs.
     - Méthodes getters et setters pour chaque attribut.

3. **Classe Reservation :**
   - Attributs : passager, vol
   - Méthodes :
     - Constructeur pour initialiser les attributs.

4. **Classe GestionReservations :**
   - Attributs : liste des vols, liste des passagers
   - Méthodes :
     - Méthodes pour ajouter un vol et un passager.
     - Méthode pour permettre à un passager de réserver un billet pour un vol.
     - Méthodes pour afficher les vols, les passagers et les réservations.

Implémentez ces classes en Java et testez-les dans un programme principal. Assurez-vous de valider votre code en ajoutant des vols, des passagers et en effectuant des réservations. Assurez-vous également de gérer les cas où un vol est complet ou lorsque le même passager tente de réserver plusieurs fois pour le même vol.


**Problème : Système de gestion d'une chaîne de restaurants**

Vous développez un système de gestion pour une chaîne de restaurants. Le système doit être capable de gérer les succursales, les menus, les commandes et les clients. Chaque succursale a un nom, une adresse et un ensemble de menus disponibles. Chaque menu a un nom, une liste de plats et un prix. Chaque plat a un nom et un prix. Chaque client a un nom, une adresse et peut passer des commandes dans une succursale.

Votre tâche est de concevoir et d'implémenter les classes Java nécessaires pour ce système de gestion de chaîne de restaurants. Voici les exigences spécifiques :

1. **Classe Succursale :**
   - Attributs : nom, adresse, liste des menus disponibles
   - Méthodes :
     - Constructeur pour initialiser les attributs.
     - Méthode pour ajouter un menu à la liste des menus disponibles.
     - Méthode pour afficher les menus disponibles.

2. **Classe Menu :**
   - Attributs : nom, liste des plats, prix
   - Méthodes :
     - Constructeur pour initialiser les attributs.
     - Méthode pour ajouter un plat à la liste des plats.
     - Méthode pour afficher les plats du menu.

3. **Classe Plat :**
   - Attributs : nom, prix
   - Méthodes :
     - Constructeur pour initialiser les attributs.

4. **Classe Client :**
   - Attributs : nom, adresse
   - Méthodes :
     - Constructeur pour initialiser les attributs.
     - Méthode pour passer une commande dans une succursale.

5. **Classe Commande :**
   - Attributs : client, succursale, liste des plats commandés
   - Méthodes :
     - Constructeur pour initialiser les attributs.
     - Méthode pour ajouter un plat à la liste des plats commandés.
     - Méthode pour calculer le total de la commande.

6. **Classe GestionRestaurant :**
   - Attributs : liste des succursales, liste des clients
   - Méthodes :
     - Méthode pour ajouter une succursale.
     - Méthode pour ajouter un client.
     - Méthode pour permettre à un client de passer une commande dans une succursale.
     - Méthode pour afficher les succursales, les menus et les commandes.


1. **Calculatrice simple :**
   Créez une classe `Calculatrice` avec des méthodes pour effectuer des opérations arithmétiques simples telles que l'addition, la soustraction, la multiplication et la division. Les méthodes prennent deux nombres en entrée et retournent le résultat de l'opération.

2. **Gestionnaire de notes :**
   Développez une classe `Etudiant` avec des attributs pour le nom de l'étudiant et ses notes dans différentes matières. Ajoutez des méthodes pour calculer la moyenne des notes de l'étudiant et pour afficher ses informations.

3. **Conversion de devises :**
   Créez une classe `ConvertisseurDeDevises` avec des méthodes pour convertir une somme d'argent d'une devise à une autre. Les méthodes prennent le montant d'argent et les taux de change en entrée et retournent le montant converti.

4. **Gestionnaire de contacts :**
   Implémentez une classe `Contact` pour représenter les informations d'un contact, telles que le nom, l'adresse e-mail et le numéro de téléphone. Ajoutez des méthodes pour afficher les détails du contact.

5. **Jeu de dé simple :**
   Créez une classe `De` pour simuler le lancer d'un dé. La classe devrait avoir une méthode pour lancer le dé et renvoyer le résultat (un nombre aléatoire entre 1 et 6).

6. **Gestionnaire de compte bancaire :**
   Développez une classe `CompteBancaire` avec des attributs pour le nom du titulaire du compte et le solde. Ajoutez des méthodes pour effectuer des dépôts, des retraits et pour afficher le solde actuel.

7. **Chronomètre :**
   Implémentez une classe `Chronomètre` pour mesurer le temps écoulé. La classe devrait avoir des méthodes pour démarrer, arrêter et réinitialiser le chronomètre, ainsi qu'une méthode pour obtenir le temps écoulé.


#### Héritage


1. **Véhicules :**
   Créez une classe `Vehicule` avec des attributs tels que la marque, le modèle et l'année. Ensuite, créez des sous-classes telles que `Voiture`, `Moto`, et `Vélo` qui héritent de la classe `Vehicule`. Chaque sous-classe devrait avoir des attributs spécifiques et des méthodes pour les actions liées au type de véhicule.

2. **Formes géométriques :**
   Définissez une classe abstraite `Forme` avec des méthodes pour calculer l'aire et le périmètre. Ensuite, créez des sous-classes telles que `Cercle`, `Rectangle`, et `Triangle` qui héritent de la classe `Forme`. Chaque sous-classe devrait implémenter les méthodes pour calculer l'aire et le périmètre selon sa forme spécifique.

3. **Employés :**
   Développez une classe `Employe` avec des attributs tels que le nom, le numéro d'identification et le salaire de base. Ensuite, créez des sous-classes telles que `Manager`, `Vendeur`, et `Technicien` qui héritent de la classe `Employe`. Chaque sous-classe devrait avoir des attributs et des méthodes spécifiques à son rôle dans l'entreprise.

4. **Animaux :**
   Créez une classe `Animal` avec des attributs tels que le nom, l'âge et l'espèce. Ensuite, créez des sous-classes telles que `Chien`, `Chat`, et `Oiseau` qui héritent de la classe `Animal`. Chaque sous-classe devrait avoir des méthodes pour des actions spécifiques à l'animal, telles que `miauler()` pour un chat ou `aboyer()` pour un chien.

5. **Produits :**
   Implémentez une classe `Produit` avec des attributs tels que le nom, le prix et la quantité en stock. Ensuite, créez des sous-classes telles que `Aliment`, `Vêtement`, et `Électronique` qui héritent de la classe `Produit`. Chaque sous-classe devrait avoir des attributs spécifiques à son type de produit.


#### Le polymorphisme


1. **Exercice 1 - Formes géométriques :**
   Définissez une classe abstraite `Forme` avec une méthode abstraite `calculerSurface()`. Ensuite, créez des sous-classes telles que `Cercle`, `Rectangle` et `Triangle`, qui étendent la classe `Forme` et implémentent la méthode `calculerSurface()` pour calculer la surface de leur forme respective.

2. **Exercice 2 - Animaux :**
   Déclarez une classe abstraite `Animal` avec une méthode abstraite `crier()`. Ensuite, créez des sous-classes telles que `Chien`, `Chat` et `Oiseau`, qui étendent la classe `Animal` et implémentent la méthode `crier()` pour représenter leur cri respectif.

3. **Exercice 3 - Employés :**
   Créez une classe abstraite `Employe` avec une méthode abstraite `calculerSalaire()`. Ensuite, créez des sous-classes telles que `Manager`, `Vendeur` et `Technicien`, qui étendent la classe `Employe` et implémentent la méthode `calculerSalaire()` pour calculer le salaire en fonction de leur type de travail.

4. **Exercice 4 - Figurines :**
   Définissez une classe abstraite `Figurine` avec une méthode abstraite `attaquer()`. Ensuite, créez des sous-classes telles que `Guerrier`, `Mage` et `Archer`, qui étendent la classe `Figurine` et implémentent la méthode `attaquer()` avec leur propre style d'attaque.

5. **Exercice 5 - Instruments de musique :**
   Créez une classe abstraite `Instrument` avec une méthode abstraite `jouer()`. Ensuite, créez des sous-classes telles que `Piano`, `Guitare` et `Trompette`, qui étendent la classe `Instrument` et implémentent la méthode `jouer()` pour jouer leur son respectif.


