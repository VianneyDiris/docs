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
