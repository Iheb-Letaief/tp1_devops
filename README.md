# Compte Rendu TP 1 - Maîtrise de Git

Ce fichier `readme.md` présente un compte rendu du TP 1 - Maîtrise de Git.

## Objectifs
- Se familiariser avec Git, un système de gestion de version décentralisé largement utilisé.
- Apprendre à gérer des projets, collaborer avec d'autres développeurs et utiliser les fonctionnalités avancées de Git.

## Partie 1: Préparation de l'environnement Git
  ### 1. Création de clé SSH
  ```shell
  ssh-keygen -t rsa -b 4096 -C iheb.eltaief@polytechnicien.tn
  ```

  ### 2. Copier la clé publique SSH
  ```shell
  cat .\id_rsa.pub
  ```

  ### 3. Tester la connexion SSH à GitHub
  ```shell
  ssh -T git@github.com
  ```
  
## Partie 2: Clonage d'un Projet Existant
  ### 1. Cloner un projet Git distant en utilisant mon URL SSH
  ```shell
  git clone git@github.com:Iheb-Letaief/tp1_devops.git
  ```
  
  ### 2. Changer le répertoire de travail vers le projet cloné
  ```shell
  cd .\tp1_devops\
  ```

## Partie 3 : Concepts de base de Git
  ### 1. Créer un nouveau fichier nommé 'index.html'
  ```shell
  touch index.html
  ```
  
  ### 2. Ajouter 'index.html' à la zone de staging de Git
  ```shell
  git add .\index.html
  ```
  
  ### 3. Effectuer le premier commit avec un message descriptif
  ```shell
  git commit -m "Premier commit : ajout de index.html"
  ```
  
  ### 4. Voir l'historique des commits
  ```shell
  git log
  ```

## Partie 4 : Collaborer sur Git
  ### 1. Créer et basculer vers une nouvelle branche pour une fonctionnalité spécifique
  ```shell
  git branch ma-fonctionnalite
  git checkout ma-fonctionnalite
  ```
  
  ### 2. Effectuer des modifications et les mettre en staging pour le commit
  ```shell
  git add .
  git commit -m "Modification de la fonctionnalité"
  ```
  
  ### 3. Pousser les modifications vers le dépôt distant
  ```shell
  git push origin ma-fonctionnalite
  ```
  
  ### 4. Basculer entre les branches 
  ```shell
  git checkout master
  ```
  
## Partie 5 : Utilisation de GitFlow
  ### 1. Initialiser GitFlow dans le projet
  ```shell
  git flow init
  ```
  
  ### 2. Démarrer une nouvelle fonctionnalité
  ```shell
  git flow feature start ma-fonctionnalite
  ```
  
  ### 3. Démarrer une nouvelle version
  ```shell
  git flow release start ma-version
  ```
  
  ### 4.Finaliser une fonctionnalité
  ```shell
  git flow feature finish ma-fonctionnalite
  ```
  
  ### 5.Démarrer un correctif si nécessaire
  ```shell
  git flow hotfix start mon-correctif
  ```


## Conclusion
Ce résumé couvre les étapes essentielles pour travailler avec Git, gérer les branches et utiliser GitFlow pour la gestion des versions et des fonctionnalités. Vous pouvez personnaliser davantage cette documentation en fonction de votre expérience spécifique et des besoins de votre projet.









