#### Les exceptions

Une exception est une condition anormale ou une situation d'erreur qui se produit pendant l'exécution d'un programme et qui peut perturber son fonctionnement normal. En Java, une exception est représentée par un objet de classe héritant de la classe `java.lang.Throwable`.

Les exceptions sont utilisées pour signaler et gérer différents types de problèmes qui peuvent survenir pendant l'exécution d'un programme, tels que :

1. Des erreurs de manipulation de fichiers, comme l'ouverture d'un fichier inexistant.
2. Des erreurs de manipulation de chaînes, comme la conversion d'une chaîne en un type de données incompatible.
3. Des erreurs de calcul, comme une division par zéro.
4. Des problèmes de mémoire, comme l'épuisement de la mémoire disponible.
5. Des erreurs de formatage, comme l'utilisation d'un format incorrect pour la date ou l'heure.
6. Des exceptions d'accès réseau, comme une connexion perdue lors de l'accès à une ressource distante.


#### Une erreur

En programmation, une erreur (ou une exception) est une condition anormale ou une situation inattendue qui se produit pendant l'exécution d'un programme et qui peut entraîner une interruption ou un dysfonctionnement du programme. Les erreurs sont généralement causées par des conditions imprévues ou des circonstances qui ne peuvent pas être gérées ou résolues par le programme lui-même.

Voici quelques exemples d'erreurs courantes en programmation :

1. **Erreur de syntaxe :** Une erreur de syntaxe se produit lorsque le code source ne respecte pas les règles de syntaxe du langage de programmation. Par exemple, une accolade manquante, une virgule incorrecte ou une faute de frappe dans un mot-clé peuvent entraîner une erreur de syntaxe.

2. **Erreur de logique :** Une erreur de logique se produit lorsque le code ne fonctionne pas comme prévu en raison d'un algorithme incorrect ou d'une mauvaise compréhension du problème à résoudre. Ces erreurs ne sont pas détectées par le compilateur et peuvent être difficiles à déboguer.

3. **Erreur d'exécution :** Une erreur d'exécution se produit pendant l'exécution du programme en raison de conditions anormales telles que la division par zéro, l'accès à une mémoire non allouée ou le dépassement de capacité d'un tableau.

4. **Erreur de concurrence :** Une erreur de concurrence se produit lorsque plusieurs threads accèdent simultanément à des ressources partagées sans synchronisation appropriée, ce qui peut entraîner des conditions de course ou des incohérences de données.

5. **Erreur de mémoire :** Une erreur de mémoire se produit lorsque le programme utilise incorrectement la mémoire disponible, comme une fuite de mémoire (memory leak) ou un dépassement de capacité du tas (heap overflow).

#### Gestion d'éxception

En Java, les exceptions sont gérées à l'aide de blocs `try`, `catch` et `finally`. Voici les étapes pour gérer les exceptions en Java :

1. **Encadrez le code susceptible de générer une exception dans un bloc `try` :** Placez le code qui pourrait générer une exception à l'intérieur d'un bloc `try`.

    ```java
    try {
        // Code susceptible de générer une exception
    } 
    ```

2. **Capturez et traitez les exceptions dans des blocs `catch` :** Ajoutez des blocs `catch` pour attraper les exceptions qui se produisent dans le bloc `try`. Chaque bloc `catch` spécifie le type d'exception qu'il peut attraper et le code à exécuter en cas de capture de cette exception.

    ```java
    catch (TypeDeLException e) {
        // Code de gestion de l'exception
    }
    ```

3. **Utilisez plusieurs blocs `catch` pour gérer différents types d'exceptions :** Vous pouvez avoir plusieurs blocs `catch` pour gérer différents types d'exceptions.

    ```java
    catch (TypeDeLException1 e) {
        // Code de gestion de l'exception 1
    }
    catch (TypeDeLException2 e) {
        // Code de gestion de l'exception 2
    }
    ```

4. **Ajoutez un bloc `finally` facultatif pour exécuter un code de nettoyage :** Le bloc `finally` est facultatif et est utilisé pour spécifier un code qui doit être exécuté après l'exécution du bloc `try` et de tous les blocs `catch`, qu'une exception ait été levée ou non. Il est couramment utilisé pour le nettoyage des ressources, telles que la fermeture de fichiers ou de connexions.

    ```java
    finally {
        // Code de nettoyage
    }
    ```

Voici un exemple complet illustrant la gestion des exceptions en Java :

```java
try {
    // Code susceptible de générer une exception
    int resultat = 10 / 0; // Division par zéro
} catch (ArithmeticException e) {
    // Gestion de l'exception d'arithmétique
    System.out.println("Division par zéro !");
} finally {
    // Code de nettoyage (facultatif)
    System.out.println("Fin du traitement.");
}
```

##### Lever une exception

Lever une exception, également appelé "jeter une exception" ou "générer une exception", fait référence au processus de signaler une condition anormale ou une situation d'erreur qui se produit pendant l'exécution d'un programme. Lorsqu'une exception est levée, elle interrompt normalement le flux d'exécution normal du programme et transfère le contrôle à un gestionnaire d'exceptions qui peut gérer la condition exceptionnelle.

Le processus de levée d'une exception se fait généralement à l'aide du mot-clé `throw` en Java. Voici comment cela fonctionne :

1. **Identification de la condition exceptionnelle :** Le programme détecte une condition anormale ou une situation d'erreur pendant son exécution. Cela peut être dû à une erreur de logique, une entrée incorrecte de l'utilisateur, un problème de système, etc.

2. **Création de l'objet d'exception :** Une fois la condition exceptionnelle détectée, un objet d'exception approprié est créé. En Java, les exceptions sont généralement des objets qui héritent de la classe `Throwable`.

3. **Lever l'exception :** L'objet d'exception est "levé" à l'aide du mot-clé `throw`. Cela signifie que l'exception est signalée et que le contrôle est transféré au gestionnaire d'exceptions le plus proche capable de la gérer.

4. **Propagation de l'exception :** Une fois l'exception levée, elle est propagée dans la pile d'appels jusqu'à ce qu'elle soit capturée et traitée par un bloc `catch` approprié.

Voici un exemple simple en Java illustrant comment lever une exception avec le mot-clé `throw` :

```java
public class Main {
    public static void main(String[] args) {
        int age = -5;
        
        if (age < 0) {
            throw new IllegalArgumentException("L'âge ne peut pas être négatif");
        }
    }
}
```

#### Signer une exception

Lorsque vous signez une exception, vous la déclarez dans la signature d'une méthode ou d'une déclaration de méthode en utilisant le mot-clé `throws`. Cela signifie que vous indiquez explicitement dans la signature de la méthode que cette méthode peut potentiellement lever une exception de ce type, mais vous ne la traitez pas à l'intérieur de la méthode elle-même.

La signature d'une méthode inclut généralement le nom de la méthode, ses paramètres, le type de valeur de retour (le cas échéant) et la liste des exceptions pouvant être levées par cette méthode. Voici un exemple simple :

```java
public void méthode() throws MonException {
    // Code de la méthode
}
```

#### Personalisation d'exception

Pour personnaliser une exception en Java, vous pouvez créer votre propre classe d'exception en étendant l'une des classes d'exceptions prédéfinies de Java, telles que `Exception` ou l'une de ses sous-classes comme `RuntimeException`. Voici les étapes pour personnaliser une exception :

1. **Créez une classe pour votre exception :** Créez une nouvelle classe qui étend une classe d'exception appropriée. Vous pouvez ajouter des champs et des méthodes supplémentaires à cette classe pour personnaliser davantage votre exception.

2. **Définissez un constructeur :** Définissez au moins un constructeur dans votre classe d'exception. Ce constructeur peut accepter des paramètres pour initialiser les champs de l'exception, comme un message d'erreur.

3. **Optionnel : Ajoutez des méthodes supplémentaires :** Selon vos besoins, vous pouvez ajouter des méthodes supplémentaires à votre classe d'exception pour fournir des fonctionnalités supplémentaires. Par exemple, vous pouvez ajouter des méthodes pour récupérer des informations spécifiques sur l'erreur.

Voici un exemple simple de personnalisation d'une exception en Java :

```java
public class MonException extends Exception {
    private String message;
    
    public MonException(String message) {
        this.message = message;
    }
    
    public String getMessage() {
        return message;
    }
}
```


Vous pouvez maintenant utiliser cette classe d'exception personnalisée dans votre code comme n'importe quelle autre exception Java. Par exemple :

```java
public class Main {
    public static void main(String[] args) {
        try {
            throw new MonException("Une erreur personnalisée s'est produite");
        } catch (MonException e) {
            System.out.println("Erreur : " + e.getMessage());
        }
    }
}
```
