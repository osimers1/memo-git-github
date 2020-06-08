Mémo sur GIT et GITHUB
======================
>tous d'abord bonjour.  vois ci mon mémo sur git et github qui, je l'èspere pourra aider certain <br/>

Pour la configuration
=====================

* git config --global user.name "Nom d'utilisateur" **==>** Pour configurer le nom 
* git config --global user.email "utilisateur@mail.com" **=>** Pour definir son adresse mail 
* git remote add origin https://github.com/osimers1/memo-git-github.git **==>** Ajoute un referentiel 
* git remote -v **==>** Voir les referentiels 
* git init **==>** pour initialiser le dossier avec git <br/>

Méssage et version
==================

* git status **==>** Pour voir le statut des modification
* git add NomDuFichier **==>** Ajout d'un fichier 
* git add . **==>** pour ajouter tous les fichier 
* git commit -m "message" **==>** Prepare l'envoie avec un message<br/>

Envoyer
======

* git push **==>** envoi normal 
* git push origin master **==>** envoi dansla branche master <br/>

Recevoir
========

* git fetch **==>** recupere branch master mais ne merge pas avec le repertoir de travail
* git pull <remote> <branch> **==>** simple reception
* git pull origin master **==>** Recupere la branche master et merge avec le repertoire de travail<br/>

Les branches
============

* git branch **==>** permet de voir les branche et de voir sur quelle branche on se trouve
* git branch NomdeLaBranche **==>** créer une branche avec son nom
* git checkout NomDeLaBranche **==>** permet de se deplacer sur la  branch desiré
* git checkout -b NomDeLaBranche **==>** créer une branche et va direct dessus
* git branch -d NomDeLaBranche **==>** suprime la branch de nom mais erreur si il y a des commit
* git branch -D NomDeLaBranche **==>** suprime la branch de nom meme si des commit sont present
* git diff **==>** permet de voir les difference entre la branche master et la branch actuel
* git merge NomDeLaBranche **==>** fusionne nom de la branch avec la branch en cour
* git checkout HEAD~4 **==>** deplace le curseur HEAD de 4 niveaux<br/>

Annulation
==========

* git reset HEAD~1 **==>** annule le dernier commit (fonctionne que en local)
* git revert HEAD **==>** annule pour push,nouveaux commit