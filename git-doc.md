# GIT

## Installation et configuration

### Installation

* Linux
  ```shell
  sudo apt-get update
  sudo apt-get install git
  ```
* Windows
  * utilisez l'installer sur : <https://gitforwindows.org/>
  * ouvrir git bash et tapez :
  ```shell
  git --version
  ```

### Configuration

* identifiant:
    ```shell
    git config --global user.name votre_nom
    git config --global user.email votre_email
    ```
* accès SSH sur un dépôt distant:
  * génération de la clé SSH:
    ```shell
    ssh-keygen
    ```
  * allez dans l'onglet "settings" de votre profil Github ensuite cliquez sur la catégorie "SSH and GPG keys" pour enfin copier votre clé publique après avoir cliqué sur "New SSH key".

---
## Les commandes de bases

### débuter un projet

* en local :
  * créez le dossier qui contiendra votre projet
  * entrez dans le dossier et ouvrez un terminal
  * tapez la commande :
  ```shell
  git init
  ```

* via Github :
  * cliquez sur "New repository"
  * dans la page qui vient de s'ouvrir, vous devez remplir le nom du repository et vous avez les options suivantes :
    *  mettre le repo en public ou privé
    *  ajouter un fichier Readme.md
    *  ajouter un fichier .gitignore
    *  mettre votre repository sous licence
 * enfin validez le tout en cliquant sur "Create repository"
 * sur votre ordinateur, ouvrez un terminal au niveau du dossier où vous voulez mettre votre repository
 * entrez la commande :
  ```shell
  git clone git@github.com:nom_utilisateur/nom_repository.git
  ``` 

* lier les 2 :
  * si vous avez crée un dépôt local avec git init et un repository : ne faîtes pas un git clone
  * il suffit juste de tapez :
  ```shell
  git remote add origin https://github.com/nom_utilisateur/nom_repository.git
  ```

### ajouter des documents sur un repository

* voir le status de votre dépôt local
  ```shell
  git status
  ````
* ajouter un document ou tous les documents
  ```shell
  git add nom_du_document
  git add .
  ```
  * valider l'ajout ou la modification
  ```shell
  git commit -m "message du commit"
  ```
  * envoyer les informations sur le repository distant
  ```shell
  git push origin nom_de_la_branche
  ```


