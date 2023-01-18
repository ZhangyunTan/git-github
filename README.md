Cours OPENCLASSROOMS:  Gérez du code avec Git et Github 


Initialiser un dépôt Git: Pour travailler sur Git, vous devez créer un dépôt local, c'est-à-dire un dossier dans lequel toutes vos modifications seront enregistrées. 


Configurez votre identité: 
$ git config --global user.name "John Doe" 
$ git config --global user.email johndoe@example.com

Grâce à l’option --global, vous n’aurez besoin de le faire qu'une fois.


vérifier les autres paramètres: 
$ git config --list 


Configurez les couleurs: 
$ git config --global color.diff auto 
$ git config --global color.status auto 
$ git config --global color.branch auto


Configurez l’éditeur:
$ git config --global core.editor notepad++ 
$ git config --global merge.tool vimdiff


Les deux méthodes pour créez un dépôt local:
   1: créer un dépôt local vide pour accueillir un nouveau projet.
   2: cloner un dépôt distant.


Initialisez votre dépôt en créant un dépôt local vide: 
$ cd git-github
$ git init


Travaillez depuis votre dépôt local Git: 

    - créez un fichier “index.html” avec son contenu.
    - créez un fichier “styles.css” avec son contenu. 


Indexez vos fichiers avec la commande git add: 
$ git add index.html styles.css


Créez une nouvelle version avec la commande git commit: 
$ git commit -m “Ajout des fichiers html et css de base”


Envoyez votre commit sur le dépôt distant avec la commande git push: 
$ git remote add origin https://github.com/EtudiantOC/OpenclassroomsProject.git
Vous avez relié le dépôt local au dépôt distant.

$ git branch -M main
$ git push -u origin main



Reprenez le fichier HTML créé. Disons que vous allez modifier le titre “Un super titre” en “Un super titre !”.

Pour créer une version du projet avec le fichier HTML à jour et l’envoyer sur le dépôt distant GitHub,
$ git add index.html


Créer une nouvelle version grâce à la commande: 
$ git commit -m “Modification du titre H1”


Envoyer la nouvelle version sur le dépôt distant: 
$ git push origin main
