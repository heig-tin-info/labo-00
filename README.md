# Prise en main de l'ordinateur

**Durée: 2x45 minutes**
**Rendu: au plus tard 3 jours après le début du laboratoire, avant minuit**

## Objectifs

- Familiarisation avec la structure IT de la HEIG-VD
- Savoir lire un intitué de laboratoire (oui, oui c'est pas si facile)
- Appliquer la marche à suivre pour obtenir et rendre un travail pratique
- Découverte et installation des outils utiles pour ce cours

## Prise en main de votre ordinateur

Démarrez votre PC et connectez-vous au réseau de l'école en utilisant vos identifiants personnels.

Une fois logué sur votre ordinateur, expérimentez:

- Un bref appui sur la touche Windows localisée entre `<CTRL>` et `<ALT>` à gauche de la barre d'espace:
  - Ouvre le menu démarrer duquel vous accédez à vos programmes.
  - Une frappe au clavier alors que le menu est ouvert vous permet la recherche de programmes
- La combinaison de touches `<CTRL>`+`<R>` fait apparaître le menu *exécuter*:
  - L'invité de dialogue vous permet d'entrer un nom de programme.
- La combinaison de touches `<CTRL>`+`<E>` fait apparaître l'explorateur de fichiers:
  - Il permet de naviguer dans votre arborescence et d'accéder à vos documents.
- La combinaison de touches `<WIN>`+`<L>` vérouille votre ordinateur:
  - Il est important de toujours vérouiller votre ordinateur lorsque vous n'êtes pas devant.

Notez qu'une suite au clavier peut être exprimée comme une suite de combinaison de touches donc les raccourcis claviers sont donnés entre chevrons `<>`. Des symboles entre chevrons séparés par le signe `+` correspond à une combinaison de touches c'est à dire maintenir simultanément les touches mentionnées.

```text
<WIN>+<R> calc <ENTER> <ALT>+<1> <ESC> 3.14 * 2 = <CTRL>+<C> <ALT>+<F4>
<WIN>+<R> notepad <ENTER> <CTRL>+<V> <CTRL>+<S> two-pies.txt <ENTER>
```

Essayez ces séquences; que font-elles ?

- Exécutez `%userprofile%` depuis le menu *exécuter*
  - Quel est ce dossier ?

## Rendu du laboratoire

Plusieurs documents seront à rendre. Commençons tout d'abord par créer un dossier.

1. Dans `Mes Documents` ou sur votre bureau, créez un dossier intitulé `labo-0`
2. Placez-y le fichier `two-pies.txt` créé plus haut

A la fin du laboratoire vous aurez dans votre dossier:

```text
.
├── README.md
├── avion.png
├── hello
├── hello.c
├── hello.exe
├── rapport.docx
└── two-pies.txt
```

Crééez un fichier `.zip` ou `.tar.gz` de votre dossier par un clic droit sur le dossier puis en choisissant l'option "Envoyer vers" puis "Fichier compressé".

Envoyez votre archive comprimée par e-mail à votre professeur.

### Microsoft Word

Microsoft Office est la suite de bureautique la plus utilsée dans l'industrie, que vous la détestiez ou l'adoreriez, vous serez amené à l'utiliser. A cette fin il vous est demandé de rendre un compte rendu Word.

1. Démarrer Microsoft Word avec `<WIN>+<R> winword <ENTER>`
2. Créez un nouveau document
3. Cherchez le menu `Styles` et sélectionnez `Titre` et entrez `Rapport de laboratoire`
4. Sélectionnez `Sous-titre` et entrez `Laboratoire 0: Familiarisation avec l'ordinteur`
5. Constatez que la faute d'orthographe se souligne en rouge
6. Utiliser un clic-droit sur la faute pour la corriger
7. Entrez votre nom, prénom et la date du jour
8. Insérez une section avec `<CTRL>+<ALT>+<1>`: Microsoft Word
9. Faite une capture d'écran pour insérer dans votre rapport

   ![word](assets/winword.png)

10. Gardez votre document ouvert pour la suite des opérations
11. ... Une fois toutes les autres étapes terminées
    1. Sauvegardez votre rapport dans un dossier

### Notepad

1. Ouvrez l'éditeur de texte `notepad` depuis `<WIN>+<R> notepad <ENTER>`
2. Ecrivez le programme C suivant:

   ```c
   /**
   * My first program in C
   * Author: Brian Kernighan <brian.kernighan@hello-world.com>
   **/
   #include <stdio.h>

   int main(void) {
      printf("hello, world\n");
      return 0;
   }
   ```

3. Sauvegardez-le sous le nom `hello.c` dans votre dossier de rapport
   1. Veillez à bien à ne pas choisir "Document Texte" pour que l'extension soit `.c` et non `.c.txt`

### Calculatrice Windows

Commencez pas collecter quelques informations liées à cette calculatrice:

1. Démarrez la calculatrice Windows écrivant `calc` dans le menu *exécuter*.
2. Démarrez votre navigateur internet en recherchant `edge` dans la barre de recherche du menu démarrer.
    1. Cherchez `windows 10 calculator shortcuts`
    2. Trouvez dans les résultats de recherche un site donnant les raccourcis clavier pour:
       1. Afficher le mode scientifique
          1. Calculer la racine carée `@`
       2. Afficher le mode programmeur
          1. Choisir le mode `HEX`
          2. Choisir le mode `OCT`
          3. Choisir le mode `BIN`
3. Ouvrir le menu en haut à gauche et observez les différents modes de conversions:
   1. Conversions de longueur
   2. Modes de calculatrice
4. Rendez-vous sur [Microsoft/calculator](https://github.com/Microsoft/calculator)
   1. Constatez qu'il s'agit du code source de votre calculatrice
   2. Cliquez sur `Issues`:
      1. Constatez bugs et propositions d'améliorations de la calculatrice Windows

Insérez dans votre rapport, la suite des opérations suivantes:

1. Convertir une température de Farenheit en Celcius. Faite une capture d'écran à placer dans votre rapport

   ![Conversion de température](assets/temperature.png)

2. Trouver la puissance équivalente à 42 Chevaux vapeurs.
   1. La petite icône `Cheval` doit montrer `42`!
   2. Capturez la fenêtre de la calculatrice avec `<ALT>+<PRINT SCREEN>`
   3. Insérer la capture dans votre document Word

3. Entrez en mode programmeur
   1. Saisir en hexadécimal (HEX) la valeur `0x5F3759DF`
   2. Le sauver dans la mémoire (MS)
   3. Entrez en mode d'édition des bits
      1. Commutez les bits 0, 8, 16 et 23
      2. Sauver ce nouveau nombre dans la mémoire
      3. Le soustraire à l'ancien nombre:
         1. Sélectionner `M-` sur la valeur sauvegardée dans la mémoire
   4. Faite une capture d'écran similaire à celle-ci mais avec les bonnes valeurs soit:
      1. Deux valeurs dans la mémoire `0x5F3759DF` et le résultat de la soustraction
      2. Le mode de changement de bits

      ![Calculatrice](assets/calc.png)

## Informatique à la HEIG-VD

### Imprimante

La HEIG-VD dispose de stations de travail à chaque étage permettant l'impression et le scan de documents. La technologie **FollowMe** permet de retenir vos impressions jusqu'à ce que vous soyez pret à récupérer vos documents.

1. Chercher dans l'[intranet](intra.heig-vd.ch) la documentation sur **FollowMe**
2. Installer les deux imprimantes proposées
3. Imprimez la première page de votre rapport en Noir et Blanc
   1. Faite un avion en papier
      1. Faite une photo de l'avion en papier avec votre téléphone ou celui d'un camarade
         1. Récupérez la photo sur votre ordinateur
         2. Ouvrez la photo avec le programme `Photos`
            1. Redimensionnez l'image à `500x500` pixels
            2. Sauvegardez l'image avec le nom `avion`
   2. Offrez votre création à votre professeur

## Installation des outils

Il vous est proposé d'installer quelques outils qui vous serons utiles pour la suite de votre Bachelor et peut-être votre Master

- Chocolatey : un gestionnaire de programme pour Windows
- Python : un langage de programmation utile au quotidien
- Git : un logiciel de gestion de version logiciel
- VsCode : un éditeur de code
- WSL : un système Linux sous Windows 10

### Chocolatey

Chocolatey est un gestionnaire de paquets pour Windows, une solution simplifiée et unifiée pour l'installation de programmes.

1. Rendez-vous sur [chocolatey.org](https://chocolatey.org/).
2. Installer Chocolatey sur votre ordinateur
3. Rechercher le logiciel `HxD - Hex Editor and Disk Editor`
   1. Notez dans votre rapport:
      1. combien de fois ce logiciel a été téléchargé,
      2. la date de la dernière mise à jour
      3. vérifier si ce packet est un *trusted package* et expliquer ce que cela signifie dans votre rapport
   2. Installez ce logiciel si vous le souhaitez.

### Git

Git est un logiciel de gestion de version très utilisé chez les développeurs. Il est utilisé dans ce cours comme outil principal pour accéder aux énnoncés de laboratoire et soumettre vos modifications.

1. Installer **Git** avec `choco install git`
2. Exécutez le programme `Git Bash` à présent disponible sur votre ordinateur
3. Configurer votre environnement Git, remplacez nom prénom et e-mail par vos identifiants HEIG-VD.

   ```sh
   git config --global user.name "Emmet Lathrop Brown"
   git config --global user.email emmet.brown@heig-vd.ch
   ```

### WSL

Windows Subsystem for Linux est une couche de compatibilité pour Windows permettant de faire tourner un vrai système Linux tel que Ubuntu. Cette solution rapproche Windows des systèmes macOS et Linux et simplifie de nombreux développements qui ne ciblent pas uniquement Windows. Installer WSL vous permettra de suivre quelques exemples cités dans le cours.

1. Utilisez la [documentation](https://docs.microsoft.com/en-us/windows/wsl/install-win10) de Microsoft pour installer WSL
   1. Choisissez votre distribution préférées. À défaut, optez pour **Ubuntu**.
   2. Une fois l'installation terminée n'oubliez pas d'[initialiser](https://docs.microsoft.com/en-us/windows/wsl/initialize-distro) votre distribution.
2. Installez `wsltty`
   1. Utilisez Chocolatey et la commande: `choco install wsltty`
   2. N'oubliez pas d'exécuter une fois l'installation terminée le programme `WSL Generate Shortcuts`
3. Sur votre bureau, exécuter l'icône avec le manchot [Tux](https://fr.wikipedia.org/wiki/Tux) nommée `WSL Terminal`
   1. Mettez à jour votre distribution avec `sudo apt update && sudo apt upgrade`

Pour ce familiariser avec les exécutables Linux, installons un programme:

1. Installez le programme `cowsay` avec `sudo apt-get install cowsay`
2. Exécutez `cowsay` suivi d'une phrase de votre choix

   ```sh
   $ cowsay Meuuuuuh
   __________
   < Meuuuuuh >
   ----------
         \   ^__^
          \  (oo)\_______
             (__)\       )\/\
                ||----w |
                ||     ||
   ```

3. Afficher le manuel du programme avec `man cowsay`
   1. Cherchez dans le manuel que fait l'option `-d`
      1. Essayez cette option
   2. Essayez une autre option possible de ce programme, faites une capture d'écran pour votre rapport
4. Quelle ligne de commande permet d'afficher ceci?

   ```sh
   _____________________
   ( Bilbon, je t'aurais )
   ---------------------
         o                    / \  //\
         o    |\___/|      /   \//  \\
               /0  0  \__  /    //  | \ \
            /     /  \/_/    //   |  \  \
            @_^_@'/   \/_   //    |   \   \
            //_^_/     \/_ //     |    \    \
         ( //) |        \///      |     \     \
         ( / /) _|_ /   )  //       |      \     _\
      ( // /) '/,_ _ _/  ( ; -.    |    _ _\.-~        .-~~~^-.
   (( / / )) ,-{        _      `-.|.-~-.           .~         `.
   (( // / ))  '/\      /                 ~-. _ .-~      .-~^-.  \
   (( /// ))      `.   {            }                   /      \  \
   (( / ))     .----~-.\        \-'                 .~         \  `. \^-.
               ///.----..>        \             _ -~             `.  ^-`  ^-_
                  ///-._ _ _ _ _ _ _}^ - - - - ~                     ~-- ,.-~
                                                                     /.-~
   ```

### Visual Studio Code

[Visual Studio Code](https://code.visualstudio.com/) est un éditeur de code extensible développé par [Microsoft](https://fr.wikipedia.org/wiki/Microsoft) pour Windows, Linux et macOS. Il est un bon point de départ pour programmer dans différents langages.

1. Installer Visual Studio Code depuis Chocolatey avec `choco install vscode`
2. Avec le racourci `<CTRL>+<K> <CTRL>+<O>`, ouvrez votre dossier de rendu
3. Ouvrez le fichier `hello.c`

### Python

Python est un langage de programmation qui vous sera certainement utile durant vos études. Il n'est pas nécessaire pour ce cours de programmation en C, cette étape est par conséquent optionelle.

1. Ouvrez un terminal WSL (Icône Tux sur votre bureau)
2. Installer Python avec `sudo apt-get install python3 python3-pip python3-ipython` (n'oubliez pas le `3`)
3. Exécutez Python avec `ipython` et saisissez le listing suivant:

```python
c = 299792458 # Vitesse de la lumière en mètres par secondes
D = 149597870 # Distance soleil-terre en kilomètres
d = 6378.137 # Rayon équatorial de la terre

D * 1000 / c / 60 # Temps en minutes du parcours de la lumière du soleil à la terre
```

## GitHub

[GitHub](https://github.com/) est une plateforme pour les développeurs permettant de partager du code source et de contribuer à d'autres projets. Nous avons vu plus haut que le code source de la calculatrice Windows est sur GitHub de même que plus de 3'000'000 autres projets. Étant donné que cet outil est très utilisé dans le développement logiciel, il est bon que tout étudiant en ingénierie soit familiarisé avec. Aussi, les travaux pratiques utiliseront le plus souvent Git.

Avant toute chose, et si ce n'est pas déjà fait, il vous faut créer un compte GitHub.

1. Sélectionnez `Sign Up` et créer un compte GitHub.
   1. Choisissez un `username` à votre convenance, ou utilisez 'prenom-nom' si vous n'avez pas d'idées
   2. Utilisez (dans la mesure du possible) votre e-mail de la HEIG-VD
2. Rendez-vous sur le fichier [addrman.cpp](https://github.com/bitcoin/bitcoin/blob/d0f81a96d9c158a9226dc946bdd61d48c4d42959/src/addrman.cpp) du code source des Bitcoin
   1. Cherchez s'il y a une [Delorean](https://fr.wikipedia.org/wiki/DeLorean_DMC-12) dane le fichier
   2. Cherchez qui a ajouté cette ligne de code
      1. Cliquez sur le numéro de la ligne incriminée
      2. Cliquez sur les trois petits points
         1. Sélectionner *View git blame*
         2. Cliquez l'avatar de la personne concernée par ce changement
            1. Ajouter à votre rapport
               1. Le nombre de contributions dans l'année.
               2. Le nombre de référentiels publics.
               3. Le nombre de *followers*.
         3. Cliquez sur le titre du *commit* (texte à côté de l'avatar)
            1. Notez dans votre rapport
               1. La date du changement
               2. Le *hash* du commit (qui est quelque chose comme `e91846ca1c1c57011e57491013f9bd...`)
               3. Le nombre de fichiers changés
               4. La version associée à ce *commit* (à côté de l'icône avec la petite étiquette)

