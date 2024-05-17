#### Les fichiers

Un fichier est une unité de stockage sur un ordinateur qui contient des données, telles que du texte, des images, des vidéos, des programmes, etc. Les fichiers sont organisés de manière hiérarchique dans un système de fichiers, où ils sont souvent regroupés dans des répertoires ou des dossiers.

Chaque fichier possède un nom unique qui permet de l'identifier dans le système de fichiers. Les fichiers peuvent avoir différentes extensions de nom de fichier, qui indiquent souvent le type de contenu qu'ils contiennent ou le programme associé à leur traitement.

Les fichiers peuvent être ouverts, lus, écrits, modifiés, déplacés, copiés ou supprimés par des programmes informatiques, selon les autorisations et les capacités du système d'exploitation sur lequel ils sont stockés.

#### Les operations sur les fichiers


1. **Création de fichier :** Vous pouvez créer un nouveau fichier vide dans le système de fichiers.

2. **Lecture de fichier :** Vous pouvez lire le contenu d'un fichier existant à partir du système de fichiers. Cela peut inclure la lecture de texte, de données binaires, d'images, de vidéos, etc.

3. **Écriture dans un fichier :** Vous pouvez écrire des données dans un fichier existant ou créer un nouveau fichier et y écrire des données. Cela peut inclure l'écriture de texte, de données binaires, la création de documents, etc.

4. **Mise à jour de fichier :** Vous pouvez modifier le contenu d'un fichier existant en y apportant des modifications. Cela peut inclure l'ajout, la suppression ou la modification de données dans le fichier.

5. **Suppression de fichier :** Vous pouvez supprimer un fichier du système de fichiers. Cette opération est permanente et supprime définitivement le fichier du système.

6. **Déplacement de fichier :** Vous pouvez déplacer un fichier d'un emplacement à un autre dans le système de fichiers. Cela peut inclure le renommage du fichier ou le déplacement vers un répertoire différent.

7. **Copie de fichier :** Vous pouvez créer une copie d'un fichier existant dans un autre emplacement ou avec un nom de fichier différent.

8. **Vérification de l'existence de fichier :** Vous pouvez vérifier si un fichier existe dans le système de fichiers sans avoir à l'ouvrir ou à le manipuler.

9. **Changement des autorisations de fichier :** Vous pouvez modifier les autorisations d'accès à un fichier, telles que les autorisations de lecture, d'écriture et d'exécution.

10. **Obtention d'informations sur le fichier :** Vous pouvez obtenir des informations sur un fichier telles que sa taille, sa date de création, sa date de modification, etc.

#### Chemin

En informatique, un chemin (path) fait référence à l'adresse ou à l'emplacement d'un fichier ou d'un répertoire dans un système de fichiers. Il s'agit d'une chaîne de caractères qui spécifie l'emplacement exact d'un fichier ou d'un répertoire dans la hiérarchie du système de fichiers.

Le chemin peut être absolu ou relatif :

1. **Chemin absolu :** Un chemin absolu spécifie l'emplacement complet d'un fichier ou d'un répertoire à partir de la racine du système de fichiers. Par exemple, sur un système de fichiers Unix, `/usr/local/bin` est un chemin absolu qui spécifie le répertoire `bin` situé dans `local`, qui lui-même est situé dans `usr`. Sur un système Windows, `C:\Program Files\Java` est un exemple de chemin absolu.

2. **Chemin relatif :** Un chemin relatif spécifie l'emplacement d'un fichier ou d'un répertoire par rapport à un répertoire de référence. Par exemple, `../../images/photo.jpg` est un chemin relatif qui spécifie le fichier `photo.jpg` situé deux niveaux au-dessus du répertoire courant.

***Path***
En Java, la classe `Path` fait partie du package `java.nio.file`, et elle est utilisée pour représenter un chemin de fichier ou de répertoire dans le système de fichiers. La classe `Path` fournit des méthodes pour manipuler les chemins, effectuer des opérations de fichiers et de répertoires, et travailler avec des chemins relatifs et absolus.

Voici quelques-unes des fonctionnalités fournies par la classe `Path` en Java :

1. **Création de chemins :** Vous pouvez créer un objet `Path` en utilisant les méthodes statiques de la classe `Paths`. Par exemple :

    ```java
    Path chemin = Paths.get("chemin/vers/fichier.txt");
    ```

2. **Conversion de chemins :** Vous pouvez convertir un `Path` en une chaîne de caractères représentant le chemin en utilisant la méthode `toString()`. Par exemple :

    ```java
    String cheminStr = chemin.toString();
    ```

3. **Résolution de chemins :** Vous pouvez résoudre un chemin relatif par rapport à un autre chemin en utilisant la méthode `resolve()`. Par exemple :

    ```java
    Path cheminRelatif = Paths.get("sous-repertoire");
    Path cheminComplet = chemin.resolve(cheminRelatif);
    ```

4. **Obtention d'informations sur le chemin :** Vous pouvez obtenir des informations sur le chemin, telles que le nom de fichier, l'extension, le répertoire parent, etc., en utilisant les différentes méthodes fournies par la classe `Path`.

5. **Navigation dans le système de fichiers :** Vous pouvez naviguer entre les répertoires, vérifier l'existence des fichiers et répertoires, créer des répertoires, lire et écrire des fichiers, etc., en utilisant les méthodes fournies par la classe `Files` en combinaison avec les objets `Path`.

```java
import java.nio.file.*;

public class ExemplePath {
    public static void main(String[] args) {
        Path chemin = Paths.get("chemin/vers/fichier.txt");
        System.out.println("Chemin: " + chemin.toString());
        System.out.println("Nom de fichier: " + chemin.getFileName());
        System.out.println("Répertoire parent: " + chemin.getParent());
        
        Path cheminRelatif = Paths.get("sous-repertoire");
        Path cheminComplet = chemin.resolve(cheminRelatif);
        System.out.println("Chemin résolu: " + cheminComplet.toString());
    }
}
```


*** Les options d'ouvertures des fichiers**

En Java, la classe principale pour ouvrir et manipuler des fichiers est la classe `File`. Lorsque vous ouvrez un fichier en Java, vous spécifiez un mode d'ouverture pour indiquer comment le fichier doit être manipulé. Les options d'ouverture courantes sont les suivantes :

1. **Lecture (Read) :** Cette option permet d'ouvrir un fichier en mode lecture seule. Vous pouvez lire le contenu du fichier, mais vous ne pouvez pas le modifier.

2. **Écriture (Write) :** Cette option permet d'ouvrir un fichier en mode écriture seule. Vous pouvez écrire de nouvelles données dans le fichier, écrasant son contenu existant. Si le fichier n'existe pas, il sera créé.

3. **Création (Create) :** Cette option permet de créer un nouveau fichier s'il n'existe pas déjà. Si le fichier existe déjà, cette option est ignorée.

4. **Création ou Écriture (Create or Write) :** Cette option combine les options de création et d'écriture. Si le fichier n'existe pas, il est créé. Sinon, son contenu est écrasé et vous pouvez écrire de nouvelles données.

5. **Ajout (Append) :** Cette option permet d'ouvrir un fichier en mode ajout, ce qui signifie que de nouvelles données peuvent être ajoutées à la fin du fichier sans écraser son contenu existant. Si le fichier n'existe pas, il est créé.

6. **Lecture et Écriture (Read and Write) :** Cette option permet d'ouvrir un fichier en mode lecture et écriture. Vous pouvez lire et modifier le contenu du fichier.

Voici comment spécifier ces options d'ouverture lors de l'ouverture d'un fichier en Java :

```java
// Exemple d'ouverture d'un fichier en mode lecture
File file = new File("exemple.txt");
FileInputStream fis = new FileInputStream(file);

// Exemple d'ouverture d'un fichier en mode écriture
FileOutputStream fos = new FileOutputStream("exemple.txt");

// Exemple d'ouverture d'un fichier en mode création ou écriture
FileOutputStream fos = new FileOutputStream("exemple.txt", true);

// Exemple d'ouverture d'un fichier en mode ajout
FileOutputStream fos = new FileOutputStream("exemple.txt", true);
```

#### Les cycles de vie d'un fichier

Le cycle de vie d'un fichier dans un système informatique peut être généralement divisé en plusieurs étapes, notamment :

1. **Création :** Le fichier est créé par un utilisateur ou un programme. Cela peut se produire lors de la création d'un nouveau document, de la génération de fichiers temporaires par un programme, ou de toute autre opération qui crée un fichier sur le système de fichiers.

2. **Ouverture :** Le fichier est ouvert par un programme pour être lu, écrit ou manipulé de toute autre manière. L'ouverture d'un fichier implique généralement l'obtention d'un descripteur de fichier ou d'un pointeur vers le fichier, qui sera utilisé pour accéder aux données du fichier.

3. **Lecture/Écriture :** Pendant cette étape, le programme lit des données à partir du fichier ou écrit des données dans le fichier. Cela peut inclure la lecture de données pour les afficher à l'utilisateur, la modification du contenu du fichier, l'ajout de nouvelles données, etc.

4. **Fermeture :** Une fois que le programme a terminé de travailler avec le fichier, il le ferme. Cela libère les ressources système associées au fichier, telles que les descripteurs de fichier, et garantit que toutes les données en attente sont correctement écrites sur le disque.

5. **Suppression :** À un moment donné, le fichier peut être supprimé par l'utilisateur ou par un programme. La suppression d'un fichier entraîne généralement la libération de l'espace disque occupé par le fichier et la suppression de toutes les entrées de métadonnées associées.

6. **Archivage :** Dans certains cas, un fichier peut être archivé, c'est-à-dire qu'il est déplacé dans un emplacement spécial pour le stockage à long terme. Cela peut être fait pour des raisons de sauvegarde, d'archivage de données historiques, etc.

7. **Accès :** Les utilisateurs ou les programmes peuvent accéder au fichier à tout moment pendant son cycle de vie pour effectuer des opérations de lecture, d'écriture, de modification ou de suppression, en fonction des autorisations et des restrictions de sécurité associées au fichier.


#### Les fichiers de caractères

Un fichier de caractères est un type de fichier qui stocke des données sous forme de séquence de caractères. Contrairement aux fichiers binaires qui stockent des données sous forme binaire, les fichiers de caractères stockent les données sous une forme lisible par les humains, généralement en utilisant un encodage spécifique tel que ASCII, UTF-8, UTF-16, etc.

Dans un fichier de caractères, chaque caractère est représenté par un code numérique correspondant à sa position dans une table de caractères, comme ASCII ou Unicode. Les fichiers de caractères sont utilisés pour stocker des données textuelles telles que du texte brut, des documents, des scripts, des programmes source, etc.

Les fichiers de caractères peuvent être ouverts et lus par des programmes qui comprennent l'encodage utilisé pour stocker les données. Cela permet aux programmes de lire et de manipuler le contenu textuel des fichiers de manière appropriée, en interprétant correctement les caractères et en affichant le texte dans le format approprié.

En Java, les fichiers de caractères peuvent être lus et écrits à l'aide de classes comme `FileReader`, `FileWriter`, `BufferedReader`, `BufferedWriter`, etc., qui permettent de manipuler le contenu des fichiers texte en utilisant différents encodages.

#### Ecrire dans un fichier de caractère

Pour écrire dans un fichier de caractères en Java, vous pouvez utiliser la classe `FileWriter` ou `BufferedWriter`. Voici un exemple d'utilisation de `BufferedWriter` :

```java
import java.io.BufferedWriter;
import java.io.FileWriter;
import java.io.IOException;

public class Main {
    public static void main(String[] args) {
        String filename = "exemple.txt";

        try (BufferedWriter writer = new BufferedWriter(new FileWriter(filename))) {
            // Écriture dans le fichier
            writer.write("Bonjour le monde !");
            writer.newLine(); // Ajoute une nouvelle ligne
            writer.write("C'est un exemple d'écriture dans un fichier de caractères.");

            System.out.println("Le contenu a été écrit dans le fichier avec succès !");
        } catch (IOException e) {
            System.err.println("Une erreur s'est produite lors de l'écriture dans le fichier : " + e.getMessage());
        }
    }
}
```

Dans cet exemple, nous utilisons `BufferedWriter` pour écrire dans le fichier "exemple.txt". Nous écrivons deux lignes de texte, en utilisant la méthode `write()` pour écrire du texte brut dans le fichier, et la méthode `newLine()` pour ajouter une nouvelle ligne entre les lignes.

#### Lire dans un fichier de caractère


Pour lire à partir d'un fichier de caractères en Java, vous pouvez utiliser la classe `FileReader` ou `BufferedReader`. Voici un exemple d'utilisation de `BufferedReader` :

```java
import java.io.BufferedReader;
import java.io.FileReader;
import java.io.IOException;

public class Main {
    public static void main(String[] args) {
        String filename = "exemple.txt";

        try (BufferedReader reader = new BufferedReader(new FileReader(filename))) {
            String line;
            while ((line = reader.readLine()) != null) {
                System.out.println(line);
            }
        } catch (IOException e) {
            System.err.println("Une erreur s'est produite lors de la lecture du fichier : " + e.getMessage());
        }
    }
}
```

Dans cet exemple, nous utilisons `BufferedReader` pour lire à partir du fichier "exemple.txt". La méthode `readLine()` lit une ligne de texte du fichier et renvoie `null` lorsque la fin du fichier est atteinte. Nous lisons chaque ligne de texte dans une boucle `while` jusqu'à ce que nous atteignions la fin du fichier.

#### Les fichiers binaire

Un fichier binaire est un type de fichier qui stocke des données sous forme binaire, c'est-à-dire sous forme de séquence de bits. Contrairement aux fichiers de texte, qui stockent les données sous forme de caractères lisibles par l'homme, les fichiers binaires stockent les données dans un format qui est généralement destiné à être utilisé par des programmes informatiques plutôt que par des humains.

Les fichiers binaires peuvent contenir n'importe quel type de données, y compris des images, des vidéos, des fichiers audio, des exécutables, des bases de données, des documents compressés, etc. Ils sont utilisés pour stocker des données de manière compacte et efficace, en préservant la structure interne des données telle qu'elle est utilisée par les programmes.

Les fichiers binaires ne sont pas destinés à être lus ou modifiés directement par des utilisateurs humains, car leur contenu est généralement incompréhensible sans le programme approprié pour l'interpréter. Cependant, les programmes informatiques peuvent lire, écrire et manipuler des fichiers binaires pour effectuer une grande variété de tâches, telles que le traitement d'images, la lecture de fichiers audio, la gestion de bases de données, etc.

En Java, vous pouvez lire et écrire des données à partir de fichiers binaires à l'aide de classes comme `FileInputStream`, `FileOutputStream`, `DataInputStream`, `DataOutputStream`, etc. Ces classes vous permettent de manipuler les données binaires de manière efficace et sécurisée, en veillant à ce qu'elles soient correctement formatées et interprétées par les programmes.

#### Ecrir dans un fichier binaire

Pour écrire dans un fichier binaire en Java, vous pouvez utiliser la classe `FileOutputStream` ou `DataOutputStream`. Voici un exemple d'utilisation de `DataOutputStream` pour écrire des données binaires dans un fichier :

```java
import java.io.DataOutputStream;
import java.io.FileOutputStream;
import java.io.IOException;

public class Main {
    public static void main(String[] args) {
        String filename = "donnees.bin";

        try (DataOutputStream outputStream = new DataOutputStream(new FileOutputStream(filename))) {
            // Écriture de données binaires dans le fichier
            outputStream.writeInt(42);  // Écrit un entier
            outputStream.writeDouble(3.14);  // Écrit un double
            outputStream.writeUTF("Hello");  // Écrit une chaîne de caractères UTF-8

            System.out.println("Les données binaires ont été écrites dans le fichier avec succès !");
        } catch (IOException e) {
            System.err.println("Une erreur s'est produite lors de l'écriture dans le fichier : " + e.getMessage());
        }
    }
}
```

Dans cet exemple, nous utilisons `DataOutputStream` pour écrire des données binaires dans le fichier "donnees.bin". Nous utilisons des méthodes telles que `writeInt()`, `writeDouble()`, `writeUTF()` pour écrire différents types de données binaires dans le fichier.


#### Lire d'un fichier binaire

Pour lire à partir d'un fichier binaire en Java, vous pouvez utiliser la classe `FileInputStream` ou `DataInputStream`. Voici un exemple d'utilisation de `DataInputStream` pour lire des données binaires à partir d'un fichier :

```java
import java.io.DataInputStream;
import java.io.FileInputStream;
import java.io.IOException;

public class Main {
    public static void main(String[] args) {
        String filename = "donnees.bin";

        try (DataInputStream inputStream = new DataInputStream(new FileInputStream(filename))) {
            // Lecture des données binaires depuis le fichier
            int intValue = inputStream.readInt();  // Lit un entier
            double doubleValue = inputStream.readDouble();  // Lit un double
            String stringValue = inputStream.readUTF();  // Lit une chaîne de caractères UTF-8

            System.out.println("Entier lu : " + intValue);
            System.out.println("Double lu : " + doubleValue);
            System.out.println("Chaîne de caractères lue : " + stringValue);
        } catch (IOException e) {
            System.err.println("Une erreur s'est produite lors de la lecture du fichier : " + e.getMessage());
        }
    }
}
```

Dans cet exemple, nous utilisons `DataInputStream` pour lire des données binaires à partir du fichier "donnees.bin". Nous utilisons des méthodes telles que `readInt()`, `readDouble()`, `readUTF()` pour lire différents types de données binaires à partir du fichier.