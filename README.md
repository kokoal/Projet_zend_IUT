# Instant Pics project
**created by Alan RIDARD & Louis MANGAND**

## Introduction
------------
C'est une application skeletton simple, se basant sur un MVC avec des modules d'uathentification et d'image.
Cette application permet de partager des images via un compte.

## Installation 
---------------------------

- Télécharger le projet depuis le tag github ou la branch Master et le mettre dans le fichier racine de votre serveur */www/ pour wampServer* ou */xamp/htdoc/ pour Xamp*

##### Installer composer :
- Commencer par vous déplacer depuis la console jusqu'au répertoire ou se trouve votre application
- Taper ensuite la commande d'installation composer : *composer install* -- Attendre la fin de l'installation
- Par mesure préventive vous pouvez taper : "composer update"

#####  Installer la base de donnée :
- Prendre le fichier BDD.sql dans le répertoire Source
- Vous pouvez, si une surcouche (ex: phpMyAdmin) est présente sur votre serveur, importer ce fichier sur votre serveur pour générer la base de donnée
- Dans phpMyAdmin, il existe un onglet "importer" qui vous permet directement d'importer la base de données
**OU**
- Vous pourrez l'ouvrir avec un éditeur de texte et vous servir des données pour générer votre base de données vous même 
- Pensez bien à appeler le Schema "zend2" placer les tables dans ce Schema
- Si votre connexion à votre base de donnée s'ouvre avec un mot de passe et/ou a un login différent de *root*, veuillez modifier le fichier *global.php* situé dans */config/autoload/global.php*

- Vous pouvez maintenant vous rendre sur votre navigateur pour ouvrir le chemin allant jusqu'à votre application

## En cas de problème

- Refaire l'installation du début et/ou vérifier que composer s'est installé correctement

- Vous pouvez me contacter par mon adresse mail : alan.ridard@gmail.com


#Manuel d'utilisation

##Création de compte : lancement de l'application
- Si vous venez d'installer l'application pour la premère fois, aller dans le dossier /public/ depuis votre navigateur.

- Créer un compte

- Connectez vous avec votre nouveau login et mot de passe

- Vous voici devant la page d'acceuil : les 20 images les plus likées de l'application


##Fonctionnalités

####Page d'acceuil : TOP 20 best pic's
- L'utilisateur peut visualiser les 20 images les plus aimées des utilisateurs

- Un petit bandeau vert indique le nom de l'utilisateur ayant posté la photo, ainsi que le nombre de likes que possédent la photo

- L'utilisateur peut arriver à tout moment sur cette page en cliquant sur *Home* ou sur la rubrique *Instant pics*

####Rubrique account
- L'utilisateur peut partager un lien qui redirige vers toutes ses images : c'est-à-dire la rubrique *My pic's* 

- En cliquant sur *settings*, l'utilisateur peut changer son mot de passe ou supprimer son compte

- En cliquant sur *logout*, l'utilisateur peut se deconnecter

####Rubrique My pic's
- L'utilisateur peut observer les images qu'il a posté sur l'application

- L'utilisateur peut, si il le désire, supprimer des images qu'il a posté en cliquant sur la petite croix rouge à droite de l'image

####Rubrique Instant add
- L'utilisateur peut upload une image sur l'application au format jpg ou png

####Aimer une image
- Si vous accèder à un lien d'un membre, de la forme : http://localhost/Projet_zend_IUT-Final/public/image/membre/ID_MEMBRE, il est possible d'aimer une ou plusieurs images de ce membre. Pour cela cliquer sur le petit pouce vert

- Vous pouvez disliker une photo en appuyant sur le pouce rouge, si jamais le pouce vert a déjà été appuyé