# <span style="color: blue;"> Commandes Git </span>

### - Cloner un depôt

- git clone <url_depot>

### - Récupérer la dernière version

- git pull

### - Initialiser un depot

- git init 

### - Initialiser un depot avec la branche main

- git init --initial-branch=main
- git init -b main

### - Ajouter des fichiers a l'index

- git add <nom_fichier>

### - Ajouter tous les fichiers à l'index

- git add .

### - Voir les modiifcations

- git status

### - Valider les modifications

- git commit -m <"message">

### - Valider et pousser

- git push

### - Voir les commits

- git log

### - Creer une branche

- git branch <nom_branche>

### - Basculer vers une branche

- git checkout <nom_branche>

### - Fusionner une branche avec la branche courante

- git merge <nom_branche>

### - Supprimer une branch

- git branch -d <nom_branche>

### Voici quelques exemples d’utilisation de git fetch :

Pour télécharger les mises à jour de la branche distante develop depuis le dépôt distant origin :

- git fetch origin develop

Pour télécharger les mises à jour de toutes les branches distantes configurées dans votre projet :

- git fetch --all

Pour ajouter les noms de références et les identifiants d’objets des références téléchargées au contenu existant de .git/FETCH_HEAD :

- git fetch --append

N’oubliez pas que git fetch ne fusionne pas automatiquement les modifications dans votre branche locale. Pour intégrer les mises à jour téléchargées, vous devrez utiliser git merge ou git pull

### - Supprimer une branche 

- git branch -d <nom_branche>


# <span style="color: blue;"> Commandes Git flow </span>

Initialisation : Pour initialiser Git Flow dans un dépôt existant, vous pouvez exécuter la commande suivante :

- git flow init

Créer une nouvelle fonctionnalité (feature) :
Pour commencer une nouvelle fonctionnalité, utilisez :

- git flow feature start nom_de_la_fonctionnalité

Faites vos modifications sur la branche de fonctionnalité.
Terminer une fonctionnalité :
Une fois la fonctionnalité terminée, fusionnez-la dans la branche develop :

- git flow feature finish nom_de_la_fonctionnalité

Créer une nouvelle version (release) :
Pour commencer une nouvelle version, utilisez :

- git flow release start 1.0.0

Effectuez les ajustements nécessaires (par exemple, mise à jour du numéro de version, correction de bugs).
Terminez la version avec :

- git flow release finish 1.0.0

Corriger un correctif (hotfix) :
Pour commencer un correctif, utilisez :

- git flow hotfix start nom_du_correctif

Effectuez les modifications nécessaires.
Terminez le correctif avec :

- git flow hotfix finish nom_du_correctif


