1. **Somme des éléments** :
   Écrivez une fonction qui prend un tableau d'entiers en entrée et retourne la somme de tous ses éléments.

2. **Maximum et minimum** :
   Écrivez une fonction qui prend un tableau d'entiers en entrée et retourne à la fois le plus grand et le plus petit élément de ce tableau.

3. **Recherche d'un élément** :
   Écrivez une fonction qui prend un tableau d'entiers et une valeur cible en entrée, et retourne true si la valeur cible est présente dans le tableau, sinon retourne false.

4. **Inversion d'un tableau** :
   Écrivez une fonction qui prend un tableau en entrée et inverse l'ordre de ses éléments. Par exemple, [1, 2, 3] devrait devenir [3, 2, 1].

5. **Moyenne des éléments** :
   Écrivez une fonction qui prend un tableau de nombres en entrée et retourne la moyenne de ses éléments.

6. **Comptage des éléments pairs** :
   Écrivez une fonction qui prend un tableau d'entiers en entrée et retourne le nombre d'éléments pairs dans ce tableau.

7. **Suppression des doublons** :
   Écrivez une fonction qui prend un tableau en entrée et supprime tous les éléments doublons, en ne conservant qu'une seule occurrence de chaque élément.

8. **Rotation d'un tableau** :
   Écrivez une fonction qui prend un tableau et un entier k en entrée, et effectue une rotation à droite du tableau de k positions. Par exemple, si le tableau est [1, 2, 3, 4, 5] et k est 2, le tableau devrait devenir [4, 5, 1, 2, 3].

9. **Concaténation de tableaux** :
   Écrivez une fonction qui prend deux tableaux en entrée et les concatène pour former un seul tableau résultant.

10. **Tri d'un tableau** :
    Écrivez une fonction qui prend un tableau d'entiers en entrée et le trie par ordre croissant.


#### Les tries


1. **Tri par insertion (Insertion sort)** :
   - Il parcourt la liste à trier, en insérant chaque élément à sa place appropriée.
   - Convient aux petites listes ou lorsque la liste est presque triée.
   - Complexité temporelle moyenne : O(n²).

2. **Tri par sélection (Selection sort)** :
   - Il trouve l'élément le plus petit et l'échange avec le premier élément, puis trouve le deuxième plus petit et l'échange avec le deuxième élément, et ainsi de suite.
   - Simple à implémenter mais inefficace pour les grandes listes.
   - Complexité temporelle moyenne : O(n²).

3. **Tri à bulles (Bubble sort)** :
   - Il parcourt la liste plusieurs fois, en comparant et en échangeant les éléments adjacents s'ils sont dans le mauvais ordre.
   - Simple à implémenter mais inefficace, surtout pour les grandes listes.
   - Complexité temporelle moyenne : O(n²).

4. **Tri par fusion (Merge sort)** :
   - Il divise récursivement la liste en deux moitiés, trie chaque moitié, puis fusionne les deux moitiés triées pour former une liste triée.
   - Très efficace, même pour de grandes listes.
   - Complexité temporelle moyenne : O(n log n).

5. **Tri rapide (Quick sort)** :
   - Il choisit un élément pivot, partitionne la liste autour du pivot en plaçant les éléments plus petits à sa gauche et les éléments plus grands à sa droite, puis trie récursivement les sous-listes.
   - Très efficace en pratique et utilisé largement.
   - Complexité temporelle moyenne : O(n log n).

6. **Tri par tas (Heap sort)** :
   - Il crée un tas à partir de la liste à trier, puis extrait successivement l'élément maximum du tas et le place à la fin du tableau.
   - Moins utilisé en pratique mais offre une complexité temporelle garantie de O(n log n).
   
7. **Tri par comptage (Counting sort)** :
   - Convient aux listes dont les éléments sont dans un petit intervalle connu.
   - Il compte le nombre d'occurrences de chaque élément et utilise ces informations pour placer chaque élément à sa position correcte dans la liste triée.
   - Complexité temporelle moyenne : O(n + k), où k est la plage d'éléments.

8. **Tri par base (Radix sort)** :
   - Il trie les éléments en traitant les chiffres individuellement en commençant par le chiffre le moins significatif et en se déplaçant vers le chiffre le plus significatif.
   - Utilisé pour trier les entiers ou les chaînes de caractères en fonction de leur représentation dans une base donnée.



### Recherche

1. **Recherche linéaire (Sequential Search)** :
   - Il parcourt la liste élément par élément jusqu'à ce qu'il trouve l'élément recherché.
   - Convient aux listes non triées et de petite taille.
   - Complexité temporelle moyenne : O(n).

2. **Recherche binaire (Binary Search)** :
   - Il nécessite que la liste soit triée au préalable.
   - Il divise récursivement la liste en deux parties et recherche dans la moitié appropriée en fonction de la comparaison avec l'élément au milieu de la liste.
   - Très efficace pour les listes triées.
   - Complexité temporelle moyenne : O(log n).

3. **Recherche par interpolation (Interpolation Search)** :
   - Il est similaire à la recherche binaire mais utilise une estimation plus intelligente de la position de l'élément recherché en fonction de sa valeur.
   - Fonctionne mieux sur des données uniformément distribuées.
   - Complexité temporelle moyenne : O(log log n) dans le meilleur des cas, O(n) dans le pire des cas.

4. **Recherche par saut (Jump Search)** :
   - Il fonctionne sur une liste triée et saute d'indices en indices à l'intérieur de la liste jusqu'à ce que l'élément recherché soit trouvé ou qu'une valeur plus grande soit rencontrée.
   - Convient aux listes triées et relativement grandes.
   - Complexité temporelle moyenne : O(√n).

5. **Recherche exponentielle (Exponential Search)** :
   - Il double la taille de l'intervalle de recherche à chaque étape jusqu'à ce qu'une valeur plus grande soit trouvée, puis effectue une recherche binaire dans cet intervalle.
   - Efficace pour les listes de taille inconnue ou non bornée.
   - Complexité temporelle moyenne : O(log n).

6. **Recherche de motif (Pattern Matching)** :
   - Il recherche un motif (sous-chaîne) dans une chaîne de caractères.
   - Il existe différentes approches pour le pattern matching, y compris la recherche naïve, les algorithmes basés sur les automates finis ou sur les expressions régulières, et les algorithmes basés sur la programmation dynamique.


#### Recursivité


1. **Calcul de la factorielle** :
   Écrivez une fonction récursive qui prend un entier positif n en entrée et renvoie n! (factorielle de n), définie comme le produit de tous les entiers de 1 à n.

2. **Calcul de la somme des chiffres** :
   Écrivez une fonction récursive qui prend un entier positif n en entrée et renvoie la somme de ses chiffres.

3. **Calcul de la puissance** :
   Écrivez une fonction récursive qui prend deux entiers x et y en entrée et renvoie x^y (x élevé à la puissance y).

4. **Recherche dans un tableau** :
   Écrivez une fonction récursive qui prend un tableau d'entiers, une valeur cible et un indice de départ en entrée, et recherche la valeur cible dans le tableau en utilisant la récursivité.

5. **Calcul de la suite de Fibonacci** :
   Écrivez une fonction récursive qui prend un entier n en entrée et renvoie le n-ième terme de la suite de Fibonacci, définie comme F(0) = 0, F(1) = 1 et F(n) = F(n-1) + F(n-2) pour n > 1.

6. **Calcul du nombre de chemins dans un réseau** :
   Écrivez une fonction récursive qui prend deux entiers m et n en entrée, représentant les dimensions d'un réseau, et renvoie le nombre total de chemins possibles pour aller du coin supérieur gauche au coin inférieur droit, en se déplaçant uniquement vers la droite ou vers le bas à chaque étape.

7. **Calcul du pgcd (Plus Grand Commun Diviseur)** :
   Écrivez une fonction récursive qui prend deux entiers a et b en entrée et renvoie leur PGCD en utilisant l'algorithme d'Euclide : si b est égal à 0, le PGCD est a, sinon le PGCD est le PGCD de b et a modulo b.

8. **Tri d'un tableau avec le tri fusion** :
   Écrivez une fonction récursive qui prend un tableau d'entiers en entrée et le trie en utilisant l'algorithme de tri fusion.

9. **Calcul de la somme des nombres premiers inférieurs à n** :
   Écrivez une fonction récursive qui prend un entier positif n en entrée et renvoie la somme de tous les nombres premiers inférieurs à n.

10. **Tours de Hanoï** :
    Écrivez une fonction récursive qui résout le problème des Tours de Hanoï, prenant en entrée le nombre de disques et les trois poteaux, et affichant les mouvements nécessaires pour déplacer tous les disques du premier poteau au dernier.

Le problème de "First In, First Out" (FIFO) est souvent associé à la gestion des files d'attente, où les éléments sont traités dans l'ordre où ils ont été ajoutés à la file. Voici un exemple de problème qui utilise le principe FIFO :

**Problème : Gestion d'une file d'attente dans une banque**

Supposons qu'une banque utilise une file d'attente FIFO pour gérer les clients qui attendent d'être servis par un guichet. Les clients entrent dans la file dans l'ordre où ils arrivent et sont servis par les guichets dans le même ordre. Écrire un programme Java qui simule la gestion de cette file d'attente. Le programme devrait permettre les opérations suivantes :

1. Ajouter un client à la file d'attente.
2. Servir le prochain client dans la file d'attente.
3. Afficher le nombre de clients dans la file d'attente.


Le problème de "First In, Last Out" (FILO), également connu sous le nom de "Last In, First Out" (LIFO), est généralement associé à la gestion de piles. Dans une structure de données de type pile, le dernier élément ajouté est le premier à être retiré. Voici un exemple de problème qui utilise le principe FILO :

**Problème : Gestion d'une pile de livres**

Supposons que vous avez une pile de livres sur votre bureau. Vous voulez ajouter des livres à la pile et retirer le dernier livre ajouté. Écrire un programme Java qui simule la gestion de cette pile de livres. Le programme devrait permettre les opérations suivantes :

1. Ajouter un livre à la pile.
2. Retirer le dernier livre ajouté à la pile.
3. Afficher le nombre de livres dans la pile.
