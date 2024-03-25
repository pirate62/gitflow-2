### Commandes Git

## Pour débuter un projet avec Git

# Initialiser un depot

git init

# initialiser un depot avec la branche main

git init --initial-branch=main
git init -b main

# ajouter des fichiers a l'index

git add <nom_fichier>

# ajouter tous les fichiers à l'index

git add .

# Voir les modiifcations

git status

# valider les modifications

git commit -m "<message>"

# creer une branche

git branch <nom_branche>

# basculer vers une branche

git checkout <nom_branche>

# fusionner une branche avec la branche courante

git merge <nom_branche>

# supprimer une branche

# Afficher la liste des branches :
git branch

# Supprimer une branche :
git branch -d <nom_branche>


### commandes Git flow

## Pour débuter un projet avec Git Flow :

# Initialiser un dépôt
git init

# Créer une branche de développement
git flow init -d

# Ajouter des fichiers à l'index
git add <nom_fichier>

# Valider les modifications
git commit -m "<message>"

# Créer une nouvelle fonctionnalité
git flow feature start <nom_fonctionnalité>

# Terminer une fonctionnalité et la fusionner dans la branche de développement
git flow feature finish <nom_fonctionnalité>

# Préparer une version Release
git flow release start <numéro_version>

# Terminer une version Release et la fusionner dans la branche de développement et la branche principale
git flow release finish <numéro_version>

# Gérer les bugs dans la branche principale
git flow hotfix start <numéro_version>

# Terminer la gestion d'un bug et la fusionner dans la branche de développement et la branche principale
git flow hotfix finish <numéro_version>
