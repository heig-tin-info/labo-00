# Prise en main de l'ordinateur

**Durée: 2x45 minutes**
**Rendu: au plus tard 6 jours après le début du laboratoire, avant minuit**

<!-- TOC -->

- [Prise en main de l'ordinateur](#prise-en-main-de-lordinateur)
  - [Introduction](#introduction)
  - [Objectifs](#objectifs)
  - [Prise en main de votre ordinateur](#prise-en-main-de-votre-ordinateur)
  - [Rendu du laboratoire](#rendu-du-laboratoire)
    - [Microsoft Word](#microsoft-word)
    - [Notepad](#notepad)
    - [Calculatrice Windows](#calculatrice-windows)
  - [Informatique à la HEIG-VD](#informatique-%c3%a0-la-heig-vd)
    - [Imprimante](#imprimante)
  - [Installation des outils](#installation-des-outils)
    - [Chocolatey](#chocolatey)
    - [Git](#git)
    - [WSL](#wsl)
  - [< Meuuuuuh >](#meuuuuuh)
  - [( Bilbon, je t'aurais )](#bilbon-je-taurais)
    - [Visual Studio Code](#visual-studio-code)
  - [GitHub](#github)
    - [Création d'un compte](#cr%c3%a9ation-dun-compte)
    - [Déloyement de votre clé publique](#d%c3%a9loyement-de-votre-cl%c3%a9-publique)
    - [Découvertes des fonctionnalités](#d%c3%a9couvertes-des-fonctionnalit%c3%a9s)
    - [Clone du laboratoire](#clone-du-laboratoire)
  - [Python (point optionnel si vous êtes curieux et que vous avez le temps)](#python-point-optionnel-si-vous-%c3%aates-curieux-et-que-vous-avez-le-temps)

<!-- /TOC -->

## Introduction

Ce travail pratique permet à l'étudiant la prise en main avec Microsoft Windows et les outils qui seront utilisés durant le semestre. Le cours étant essentiellement axé ligne de commande, il est naturel de s'orienter davantage sur un environnement de travail en ligne de commande. Depuis 2016 Microsoft propose un produit nommé Windows Subsystem for Linux. Il s'agit d'une distribution Linux tournant dans Windows. C'est cet outil qui sera proposé pour le semestre.

## Objectifs

- Familiarisation avec la structure IT de la HEIG-VD
- Savoir lire un intitué de laboratoire (oui, oui c'est pas si facile)
- Appliquer la marche à suivre pour obtenir et rendre un travail pratique
- Découverte et installation des outils utiles pour ce cours

## Prise en main de votre ordinateur

Démarrez votre PC et connectez-vous au réseau de l'école en utilisant vos identifiants personnels [AAI](https://aai-admin.hes-so.ch).

Une fois connecté sur votre ordinateur, expérimentez:

- Un bref appui sur la touche Windows positionnée sur le clavier à gauche de la barre d'espace et entre `<CTRL>` et `<ALT>`
  - ouvre le menu **démarrer** duquel vous accédez à vos programmes.
  - Une frappe au clavier alors que le menu est ouvert vous permet la recherche de programmes
- La combinaison de touches `<CTRL>`+`<R>` fait apparaître le menu **exécuter**.
  - L'invité de dialogue vous permet d'entrer un nom de programme.
- La combinaison de touches `<CTRL>`+`<E>` fait apparaître l'explorateur de fichiers.
  - Il permet de naviguer dans votre arborescence et d'accéder à vos documents.
- La combinaison de touches `<WIN>`+`<L>` vérouille votre ordinateur.
  - Il est important de toujours vérouiller votre ordinateur lorsque vous vous absentez.

Notez qu'une séquence au clavier peut être exprimée comme une suite de combinaisons de touches. Les chevrons `<>` seront utilisés pour différentier un ou des caractères de d'une touche du clavier. Par exemple, la touche de tabulation (↹) sera indiquée `<TAB>` alors que `TAB` correspondra à la frappe des trois caractères `T`, `A` et `B`. Lorsque des touches sont séparées par le signe `+` cela correspond à une combinaison de touches. C'est à dire le maintien simultané des touches mentionnées. Ainsi `<CTRL>`+`<R>` correspond à maintenir la touche **contrôle** pendant que la touche `R` est appuyée.

Voici deux séquences de touches, que font-elles ?

```text
<WIN>+<R> calc <ENTER> <ALT>+<1> <ESC> 3.14 * 2 = <CTRL>+<C> <ALT>+<F4>
<WIN>+<R> notepad <ENTER> <CTRL>+<V> <CTRL>+<S> two-pies.txt <ENTER>
```

Exécutez `%userprofile%` depuis le menu *exécuter*, l'explorateur de fichiers s'ouvre. Quel est ce dossier ? Si vous ne savez pas, cherchez une référence utile sur internet et intégrez là à votre rapport.

Soyez succint, votre rapport doit être précis et doit aller à l'essentiel.

## Rendu du laboratoire

Durant ce travail pratique, plusieurs documents seront à rendre. Pour se préparer à ce rendu, commençons tout d'abord par créer un dossier.

1. Dans `Mes Documents` ou sur votre bureau, créez un dossier intitulé `labo-0`.
2. Placez-y le fichier `two-pies.txt` créé plus haut.

A la fin de ce travail vous aurez dans votre dossier la structure suivante:

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

Crééez une archive [compressée](https://www.google.com/search?q=windows+how+to+compress+folder) de ce dossier puis envoyez votre archive comprimée par e-mail à votre professeur.

### Microsoft Word

Microsoft Office est la suite de bureautique la plus utilsée dans l'industrie, que vous la détestiez ou l'adoreriez, vous serez inévitablement amené à l'utiliser. A cette fin il vous est demandé de rendre un compte rendu Microsoft Word.

1. Démarrer Microsoft Word avec `<WIN>+<R> winword <ENTER>`.
2. Créez un nouveau document.
3. Cherchez le menu `Styles` et sélectionnez `Titre` et entrez `Rapport de laboratoire`.
4. Sélectionnez `Sous-titre` et entrez `Laboratoire 0: Familiarisation avec l'ordinteur`.
5. Constatez que la faute d'orthographe se souligne en rouge.
6. Utiliser un clic-droit sur la faute pour la corriger.
7. Entrez votre nom, prénom et la date du jour.
8. Insérez une section avec `<CTRL>+<ALT>+<1>` intitulée `Microsoft Word`.
9. Faite une capture d'écran pour insérer dans votre rapport:

   ![word](assets/winword.png)

10. Gardez votre document ouvert pour la suite des opérations.
11. ... Une fois toutes les autres étapes terminées, sauvegardez votre rapport dans votre dossier de rendu.

### Notepad

1. Ouvrez l'éditeur de texte `notepad` depuis `<WIN>+<R> notepad <ENTER>`
2. Saississez le programme C suivant:

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

3. Sauvegardez-le sous le nom `hello.c` dans votre dossier de rendu.
   1. Veillez à ne pas choisir "Document Texte" lors de la sauvegarde pour que l'extension du fichier soit `.c` et non `.c.txt`
4. Quelle est la version de Notepad que vous utilisez ?

### Calculatrice Windows

Commencez pas collecter quelques informations liées à cette calculatrice:

1. Démarrez la calculatrice Windows écrivant `calc` dans le menu *exécuter*.
2. Démarrez votre navigateur internet en recherchant `edge` dans la barre de recherche du menu démarrer.
    1. Cherchez `windows 10 calculator shortcuts`
    2. Trouvez dans les résultats de recherche un site donnant les raccourcis clavier pour:
       1. afficher le mode scientifique,
       2. calculer la racine carrée,
       3. afficher le mode programmeur,
          1. choisir le mode `HEX`,
          2. choisir le mode `OCT`,
          3. choisir le mode `BIN`.
3. Ouvrir le menu en haut à gauche et observez les différents modes de conversions:
   1. conversions de longueur,
   2. modes de calculatrice.
4. Rendez-vous sur [Microsoft/calculator](https://github.com/Microsoft/calculator).
   1. Constatez qu'il s'agit du code source de votre calculatrice.
   2. Cliquez sur `Issues` et constatez la liste des bogues ouverts.

A présent, effectuez les opérations suivantes et reportez vos observations dans votre rapport.

1. Convertir une température de Farenheit en Celsius. Faite une capture d'écran à placer dans votre rapport
   ![Conversion de température](assets/temperature.png)
2. Trouver la puissance mécanique équivalente à 42 Chevaux vapeurs:
   1. la petite icône `Cheval` doit montrer `42`.
   2. Capturez la fenêtre de la calculatrice avec `<ALT>+<PRINT SCREEN>`.
   3. Insérer la capture dans votre rapport.
3. Entrez en mode programmeur
   1. Saisir en hexadécimal (HEX) la valeur `0x5F3759DF`
   2. Le sauver dans la mémoire (MS)
   3. Entrez en mode d'édition des bits
      1. Commutez les bits 0, 8, 16 et 23
      2. Sauver ce nouveau nombre dans la mémoire
      3. Le soustraire à l'ancien nombre en sélectionnant `M-` sur la valeur préalablement sauvegardée dans la mémoire.
         1. Que vaut ce résultat en décimal (`DEC`) ?
   4. Faite une capture d'écran similaire à celle-ci mais avec les bonnes valeurs soit:
      1. Deux valeurs dans la mémoire `0x5F3759DF` et le résultat de la soustraction
      2. Le mode de changement de bits

      ![Calculatrice](assets/calc.png)

## Informatique à la HEIG-VD

### Imprimante

La HEIG-VD dispose de stations de travail à chaque étage permettant l'impression et le scan de documents. La technologie **FollowMe** permet de retenir vos impressions jusqu'à ce que vous soyez pret à récupérer vos documents.

1. Chercher dans l'[intranet](intra.heig-vd.ch) la documentation sur **FollowMe**.
2. Installer les deux imprimantes proposées.
3. Imprimez la première page de votre rapport en Noir et Blanc.
4. Faite un avion en papier.
5. Faite une photo de l'avion en papier avec votre téléphone ou celui d'un camarade
6. Récupérez la photo sur votre ordinateur
7. Ouvrez la photo avec le programme `Photos`
8. Redimensionnez l'image à `500x500` pixels
9. Sauvegardez l'image avec le nom `avion`
10. Offrez votre création à votre professeur

Si vous êtes perdu, ne levez pas tout de suite la main, chercher sur internet par exemple "Comment redimensionner une photo sous Windows 10". Le but de ce laboratoire et aussi de vous inciter à être autonome.

## Installation des outils

Il vous est proposé d'installer quelques outils qui vous serons utiles pour la suite de votre Bachelor et peut-être même votre Master, et peut-être même plus tard lorsque vous serez dans l'industrie.

- **Chocolatey** : un gestionnaire de programme pour Windows
- **Python** : un langage de programmation utile au quotidien
- **Git** : un logiciel de gestion de version logiciel
- **Visual Studio Code** : un éditeur de code
- **WSL** : un système Linux sous Windows 10

### Chocolatey

Chocolatey est un gestionnaire de paquets pour Windows, une solution simplifiée et unifiée pour l'installation de programmes.

1. Rendez-vous sur [chocolatey.org](https://chocolatey.org/).
2. Installer Chocolatey sur votre ordinateur
3. Rechercher le logiciel `HxD - Hex Editor and Disk Editor`
4. Notez dans votre rapport:
   1. combien de fois ce logiciel a été téléchargé,
   2. la date de sa dernière mise à jour,
   3. vérifier si ce packet est un *trusted package* et expliquer ce que cela signifie dans votre rapport.
5. Installez ce logiciel si vous le souhaitez.

### Git

Git est un logiciel de gestion de version très utilisé chez les développeurs. Il est utilisé dans ce cours comme outil principal pour accéder aux énnoncés de laboratoire et soumettre vos modifications.

1. Installer **Git** avec `choco install git`.
2. Exécutez le programme `Git Bash` à présent disponible sur votre ordinateur.
3. Configurer votre environnement Git, remplacez nom prénom et e-mail par vos identifiants HEIG-VD.

   ```sh
   git config --global user.name "Emmet Lathrop Brown"
   git config --global user.email emmet.brown@heig-vd.ch
   ```

Cet outil permet des échanges sécurisés en utilisant une clé cryptographique nommée clé SSH. Pour créer une telle clé utilisez simplement la commande:

```sh
ssh-keygen
```

Utilisez toutes les valeurs par défaut et si vous souhaitez protéger votre clé par un mot de passe, spécifiez-en un. Vous n'êtes pas obligé si vous êtes certain que personne d'autre que vous n'a accès à votre ordinateur.

A l'issue de cette étape vous obtiendrez quelque chose comme ceci:

```sh
Generating public/private rsa key pair.
Enter file in which to save the key (/t//.ssh/id_rsa):
Created directory '/t//.ssh'.
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /t//.ssh/id_rsa.
Your public key has been saved in /t//.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:roMkIIUQP4DcTzitPsPCNjIA/myLCwZbjkQl0wJ6xm0 john-doe@einet
The key's randomart image is:
+---[RSA 3072]----+
|X=o.o            |
|=*=* o           |
|+oB E            |
|=+ + .           |
|=o*     S        |
|=X.O.  .         |
|*o*o+.  .        |
|o. .. ..         |
| ..   ..         |
+----[SHA256]-----+
```

Ce programme a créé deux clés:

- Une clé privée que vous ne devez jamais communiquer à personne
- Une clé publique que vous pouvez transmettre à ceux qui souhaitent communiquer avec vous.

Plus haut nous avons pu lire: `Your public key has been saved in /t//.ssh/id_rsa.pub.`. Pour consulter votre clé utilisez:

```sh
cat /t//.ssh/id_rsa.pub
```

Vous devriez obtenir un texte étrange commençant par `ssh-rsa`. Copiez ce texte et insérez le dans votre rapport.

### WSL

Windows Subsystem for Linux est une couche de compatibilité pour Windows permettant de faire tourner un vrai système Linux sur votre ordinateur Windows. Si vous avez peur de la ligne de commande, n'ayez crainte, nous allons avidement l'utiliser durant ce cours.

Cette solution récente rapproche Windows des autres systèmes d'exploitation comme macOS et Linux et simplifie de nombreux développements qui ne ciblent pas uniquement Windows. Installer WSL vous permettra de suivre quelques exemples cités dans le cours plus simplement que sous Windows.

1. Utilisez la [documentation](https://docs.microsoft.com/en-us/windows/wsl/install-win10) de Microsoft pour installer WSL
2. Choisissez votre distribution préférées. À défaut, optez pour **Ubuntu**.
3. Une fois l'installation terminée n'oubliez pas d'[initialiser](https://docs.microsoft.com/en-us/windows/wsl/initialize-distro) votre distribution.
4. Installez `wsltty`:
   1. utilisez Chocolatey et la commande: `choco install wsltty`;
   2. n'oubliez pas d'exécuter une fois l'installation terminée le programme `WSL Generate Shortcuts`.
5. Sur votre bureau, exécutez l'icône avec le manchot [Tux](https://fr.wikipedia.org/wiki/Tux) nommée `WSL Terminal`
6. Mettez à jour votre distribution avec la commande `sudo apt update && sudo apt upgrade`

Pour se familiariser avec les exécutables Linux essayons d'installer un programme:

1. Installez le programme `cowsay` (vache qui parle) avec `sudo apt-get install cowsay`
2. Exécutez `cowsay` suivi d'une phrase de votre choix, p.ex:

   ```text
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

3. Affichez le manuel du programme avec la commande `man cowsay`
4. Cherchez dans le manuel que fait l'option `-d`
5. Essayez cette option
6. Essayez une autre option possible de ce programme, copiez le texte de sortie et insérez-le dans votre rapport.
7. (optionnel) A votre avis, quelle ligne de commande permet d'afficher ceci ?

   ```text
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

Ce que vous devez retenir c'est que:

- Pour installer un programme sous Linux Ubuntu il faut utiliser la commande `apt-get install` suivi du nom de la commande que vous voulez utiliser.
- Pour consulter l'aide d'un programme, utiliser le programme `man` qui affiche le manuel d'un programme.
- L'appel des programmes peut être modifié avec des options comme `-d`.

### Visual Studio Code

[Visual Studio Code](https://code.visualstudio.com/) est un éditeur de code extensible développé par [Microsoft](https://fr.wikipedia.org/wiki/Microsoft) pour Windows, Linux et macOS. Il est un bon point de départ pour programmer dans différents langages.

Cet éditeur a été choisi pour ce cours car il est très complet, assez léger et surtout, il fonctionne très bien avec WSL.

1. Installer Visual Studio Code depuis Chocolatey avec `choco install vscode`
2. Exécutez Visual Studio Code
3. Avec le racourci `<CTRL>+<K> <CTRL>+<O>`, ouvrez votre dossier de rendu:
   1. sur la gauche de la fenêtre vous avez la liste des fichiers de votre dossier.
4. Ouvrez le fichier `hello.c` que nous avons écris plus haut.

## GitHub

[GitHub](https://github.com/) est une plateforme pour les développeurs permettant le partager et la collaboration de projets *open-source*. Nous avons vu plus haut que le code source de la calculatrice Windows est sur GitHub de même que plus de 3'000'000 autres projets. Étant donné que cet outil est massivement utilisé dans le développement logiciel, il est bon que tout étudiant en ingénierie soit familiarisé avec. Aussi, les travaux pratiques utiliseront le plus souvent Git et GitHub.

### Création d'un compte

Avant toute chose, et si ce n'est pas déjà fait, il vous faut créer un compte GitHub.

1. Allez sur [GitHub](https://github.com/)
2. Sélectionnez `Sign Up` et créer un compte GitHub.
3. Choisissez un `username` à votre convenance, ou utilisez 'prenom-nom' en **minuscule** si vous n'avez pas d'idées.
4. Utilisez (dans la mesure du possible) votre e-mail de la HEIG-VD afin de bénécifier des avantages du Campus Program.

### Déloyement de votre clé publique

Vous rappelez-vous, nous avions créé une clé `SSH` pour sécuriser nos transactions avec Git. Il est temps d'ajouter cette clé à votre compte GitHub.

1. Ayez sous la main votre clé public de la forme:

   ```text
   ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQC3RiOdvxC/+qW0IDpb0UGPFgFOMqKLzzJ
   MxRLNbRN2QIcCvLbLUI0UmzOYvLoawXtmv3W3N+kvVCKc/ED+hAOorx1P2ZaFbyzim6PjBU
   0tBGKWZoN5DsMfy4xo7h1IO5uugFjC7KyDLfCUk+1gAuiDDYy2hLZn+Agfh9oG6YONVEYDX+OZeNK0UhwNahZxjHWQK0No4nvK9Al0IpChY5Y3Kz+shHtYYNXiFtYSgz86BbiAwjzkIh32
   wAa349VT4FmVWlSyVX0c2ZlwEUogXfKrM3IFjH+bqOwKCWL1BjNdi/geJ9tlRTiy4lpa5AW
   rdHCpz7NuBfXbaMjEjgH ycr@ordinateur
   ```

2. Rendez-vous sur GitHub dans vos préférences puis dans l'onglet *SSH and GPG keys*.
3. Ajoutez une nouvelle clé SSH avec *New SSH key*.
4. Copier/coller votre clé publique.
5. Nommez votre clé `HEIG-VD`.

### Découvertes des fonctionnalités

1. Rendez-vous sur le fichier [addrman.cpp](https://github.com/bitcoin/bitcoin/blob/d0f81a96d9c158a9226dc946bdd61d48c4d42959/src/addrman.cpp) du code source des Bitcoin
2. Cherchez s'il y a une [Delorean](https://fr.wikipedia.org/wiki/DeLorean_DMC-12) dane le fichier
3. Cherchez qui a ajouté cette ligne de code
4. Cliquez sur le numéro de la ligne incriminée
5. Cliquez sur les trois petits points
6. Sélectionner *View git blame*
7. Cliquez l'avatar de la personne concernée par ce changement
8. Ajouter à votre rapport
9. Le nombre de contributions dans l'année.
10. Le nombre de référentiels publics.
11. Le nombre de *followers*.
12. Cliquez sur le titre du *commit* (texte à côté de l'avatar)
13. Notez dans votre rapport
    1. La date du changement
    2. Le *hash* du commit (qui est quelque chose comme `e91846ca1c1c57011e57491013f9bd...`)
    3. Le nombre de fichiers changés
    4. La version associée à ce *commit* (à côté de l'icône avec la petite étiquette)

Expliquez dans votre rapport ce que vous avez compris de cette fonctionnalité `Git Blame`.

### Clone du laboratoire

Par la suite, les énnoncés des travaux pratiques seront accompagnés de code source à compléter. Les référentiels de code seront disponibles sur GitHub. Le rendu du travail consistera à publier vos changements sur GitHub.

1. Lancer WSL
2. Cloner le référentiel de ce travail pratique avec la commande:

   ```sh
   git clone git@github.com:heig-vd-tin/info1-labo-00.git
   ```

3. Naviguer dans ce répertoire avec `cd info1-labo-00`
4. Ouvrez le projet avec Visual Studio Code avec `code .` (n'oubliez pas le point)

## Python (point optionnel si vous êtes curieux et que vous avez le temps)

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

Pour quitter l'interface, utilisez la commande `quit` ou utiliser `<CTRL>+<D>`.
