# Formation JS Ismin

Ce repository git sert de base à la seconde formation Javascript
donnée par Mathieu CAROFF et Youen FROGER en novembre 2018.

La suite de ce fichier README explique l'installation des dépendances et
comment obtenir un environnement de développemenet prêt à être utilisé.

Si vous rencontrez des difficultés à un point quelconque de ce tutoriel, vous
pouvez contacter Mathieu CAROFF par mail ou par messenger pour obtenir de
l'aide.

## Installation des dépendances

### NodeJS, NPM et Git

Le moteur NodeJS et le gestionnaire de paquets NPM sont nécessaires.
Le système de gestion de sources Git est optionnel.

#### Windows et MacOS

Sur Windows et MacOS, NodeJS et NPM peuvent être installés ensembles en
téléchargeant [un installeur depuis le site officiel](https://nodejs.org/en/download/).
Le choix par défaut inclut aussi le gestionnaire de paquets NPM dont nous auront besoin.

Alternativement, sur Windows, si vous utilisez
[Chocolatey](https://chocolatey.org/), l'installation peut se faire en
executant la commande ci-dessous dans un terminal Windows lancé en tant
qu'administrateur.

```cmd
chocolatey install nodejs git
```

Alternativement, sur MacOS, si vous utilisez [Homebrew](https://brew.sh/), vous
pouvez installer nodejs et npm avec la commande ci-dessous :

```bash
brew install nodejs npm git
```

#### Linux

Sur linux Ubuntu et toutes les distributions utilisant APT, l'installation se
fait facilement en executant la ligne de commande ci-dessous :

```bash
sudo apt install nodejs npm git
```

### Récupération des sources

Si vous n'avez pas installé git, téléchargez ce dossier sous forme de `.zip` en
utilisant le bouton vert en haut à droite de la page "Cloner ou télécharger",
puis décompressez l'archive.

Si vous avez installé git, vous pouvez utiliser la commande ci-dessous pour
télécharger le repository. Cela créera un dossier "formation-js-ismin" dans le
dossier courant. Note : le dossier courant est celui désigné par la variable
`$PWD`. Utilisez la commande `pwd` pour afficher sa valeur.

```bash
git clone https://github.com/mathieucaroff/formation-js-ismin.git
```

### Installation des paquets NodeJS spécifiés dans package.json

Se placer à l'intérieur du repository (par exemple avec `cd
formation-js-ismin`), et exécuter:

```bash
npm install
```

Ceci va créer localement un dossier `node_modules` contenant les dépendances "p5",
"webpack", "webpack-cli" et "webpack-dev-server".

## Tester l'installation

Si tout a fonctionné, vous devez pouvoir exécuter la commande ci-dessous depuis
l'intérieur du repository,

```bash
npm run dev
```

puis ouvrir votre navigateur à l'adresse http://localhost:9000/ et voir un
rectangle noir.

### Tester le rechargement automatique de la page

Ouvrez la console développeur. Le message "Formation-JS-ISMIN" doit y être
écrit.

Ouvrez le fichier index.js et changer le text "Formation-JS-ISMIN" par autre
chose. Lorsque vous sauvegardez, la page web doit se recharger automatiquement
et la console afficher le nouveau texte.

### Lien(s) util(s)

Documentation de la librairie de dessin p5: https://p5js.org/
