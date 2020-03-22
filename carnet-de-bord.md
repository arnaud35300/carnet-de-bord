# carnet-de-bord

## Sprint 0
 
### 25/02/2020 - Day 01

- Réunion d'équipe
- Réflexion et mise en place du cahier des charges.
- Discussion autour de l'organisation du projet


### 26/02/2020 - Day 02

- Réunion d'équipe
- Création du Trello:
	- Mise en place des user Stories
	- Product Backlog + V2
	- Planning poker 
- Rédaction du cahier des charges et des routes
- Définition d'une convention Git
- Recherches techniques sur l'authentification JWT token en full api Symfony
- Mise en place du dictionnaire des données

### 27/02/2020 - Day 03

- Réunion d'équipe
- ajout de nouvelles routes pour gérer les types et les subtypes, et modification du cdc par conséquent
- mise en place d'une convention de code
- modification des routes
- mise en place du MCD/MLD

## Sprint 1

### 28/02/2020 - Day 01

- Réunion d'équipe
- Réflexion sur la map
- Modification du mcd/mld/data-dictionnary : Ajout des champs x et y pour l'entité CelestialBody
- Installation du serveur symfony et de ses dépendances
- Création des entités, choix de l'encryptage des mots de passe (argon2i)

### 02/03/2020 - Day 02

- Réunion d'équipe
- Mise en place des fixtures
- Création du service Slugger
- Mise en place du UserController

### 03/03/2020 - Day 03

- Réunion d'équipe
- Review du code
- Documentation sur LexiqJWTToken 

### 04/03/2020 - Day 04

- Réunion d'équipe
- Ajout des contraintes sur les entités
- Modification des méthodes update et create de UserControler/CelestialBodyController
- Création du AdminController
- Review du code et respect de la convention de code 

### 05/03/2020 - Day 05 

- Réunion d'équipe
- Mise en place des events sur les entités
- Réunion bilan sprint 01
- Update des fixtures
- Réflexion sur les query builders

### 06/03/2020 - Day 06

- Réunion d'équipe
- Debug des routes/controller
- Mise en place du serveur apache
- Réecriture d'url 

### 09/03/2020 - Day 07

- Réunion d'équipe
- mise en place de NelmioCors pour gérer les soucis liés au CORS
- mise en place de JWTRefreshTokenBundle pour l'authentification(token)
- mise en place de JWTRefreshTokenBundle pour rafraichir les tokens a chaque requête

## Sprint 2 

### 10/03/2020 - Day 01

- Réunion d'équipe
- Présentation en équipe du projet
- Gestion des events sur UserController
- Création des voters et gestion des permissions
- Update du serveur (git pull + maj de la base)

### 11/03/2020 - Day 02

- Réunion d'équipe
- Mise en place d'une regex pour le password
- Modification de UserEvent (ajout du birthday)
- Gestion de la largeur des astres ( services Delimiter crée)
- Création d'une route dans UserController qui retourne l'utilisateur connecté
- Aide pour la modification du CelestialBodyController et de ses méthodes (création en prime de la méthode verifyDelimiter)
 
### 12/03/2020 - Day 03

- Réunion d'équipe
- Début du debug de l'authentification
- Désinstallation de refreshJWTtokenbundle et test
- Mise en place d'un event kernel empechant aux utilisateurs d'etre banni

### 13/03/2020 - Day 04

- Réunion d'équipe
- Mise en place d'un service pour l'upload d'image

### 16/03/2020 - Day 05

- Réunion d'équipe
- Correction du problème de token ( suppression de l'event preUpdate du UserEvent qui réencodait le mdp à 	chaque fois)
- Upload d'image en place
- Modification des controlers (UserController|CelestialBodyController) pour gérer l'upload d'images
- Création de regex pour gérer les noms de fichiers et vérifier le format du champ birthday de l'entité User
- Modification du resize des images (on les crop désormais par rapport a leur hauteur)

## Sprint 3

### 17/03/2020 - Day 01

- Réunion d'équipe
- Mise en place de l'envoi d'email avec SwiftMailer
- Mise en place du dictionnaire des mots interdit et d'un évènement du Kernel

### 18/03/2020 - Day 02

- Réunion d'équipe
- Refactorisation du code
- Déploiement du serveur front
- Debuguage sur banbuilder sur le serveur

### 19/03/2020 - Day 03

- Gestion des cors pour autoriser uniquement le domaine front
- Veille technologique sur l'authentification avec Anthony
- Récupération des images(avatar, badges etc...)
- Rectification du service delimiter dans les contôleurs
- Envoi d'email lors du ban 

### 20/03/2020 - Day 04

- Intégration de nouvelles images
- Authentification sur le back office
- Début des pages du back office
- Modification de AdminController pour le backOffice

### 21/03/2020 - Day 05

- Intégration des pages du backoffice 
- Modification de fichiers de configuration (.env)