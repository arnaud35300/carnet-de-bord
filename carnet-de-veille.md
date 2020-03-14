# carnet-de-bord

## Sprint 0
 
### 25/02/2020 - Day 01
 
 - Réunion d'équipe
 - Réflexion et mise en place du cahier des charges.
 - Discussion autour de l'organisation du projet
  
### 26/02/2020 - Day 02
 
- authentification JWT token en full api Symfony
- Mise en place du dictionnaire des données

### 27/02/2020

- ajout de nouvelles routes pour gérer les types et les subtypes, et modification du cdc par conséquent
- mise en place d'une convention de code
- modification des routes
- mise en place du MCD/MLD

## Sprint 1 

### 28/02/2020 - Day 01

- renseignement sur l'authentification symfony en API: 
	- https://symfony.com/doc/current/security/guard_authentication.html
	- essai sur guard-authentication
- recherche sur la création d'un projet skeleton symfony:
	- https://github.com/O-clock-Alumni/fiches-recap/blob/master/symfony/themes/symfony-basics.md
- compréhension des branches github

### 02/03/2020 - Day 02

- merge de 3 branch git
- recherche sur le crud en api REST:
	- https://medium.com/q-software/symfony-5-the-rest-the-crud-and-the-swag-7430cb84cd5
- utilisation plus poussé d'insomnia:
	- création de groupes de routes etc...

### 03/03/2020 - Day 03

- documentation sur les token:
	- Api platform
	- Auth0
	- LexiqJWTTokenBundle : https://github.com/lexik/LexikJWTAuthenticationBundle
 
### 04/03/2020 - Day 04

- documentation sur les contraintes symfony: 
	- https://symfony.com/doc/current/reference/constraints.html
- problématique sur les contraintes d'entités symfony: 
	- @Assert\Datetime

### 05/03/2020 - Day 05

- documentation sur les events symfo:
	- https://symfony.com/doc/current/doctrine/events.html
- réflexion sur les querybuilders
	- https://codereviewvideos.com/course/doctrine-performance-optimisations/video/doctrine-indexes
	
### 06/03/2020 - Day 06

- documentation sur les erreurs symfony:
    - réglage des erreurs des routes
- debug des routes, manipulation des dates:
    - https://www.php.net/manual/fr/datetime.createfromformat.php
- mise en place du serveur apache:
	- creation : https://github.com/O-clock-Alumni/fiches-recap/blob/master/adminsys/aws/create_server.md
	- installation: https://github.com/O-clock-Alumni/fiches-recap/blob/master/adminsys/aws/install.md
	- replay :https://drive.google.com/drive/folders/1pbt_wqBxXgZ3qiOchMdKN1knFklI8iHv
	- autres : https://github.com/arnaud35300/VMteleporteur/blob/master/README.md
- réécriture d'url apache:
	- https://forum.ubuntu-fr.org/viewtopic.php?id=164810

### 06/03/2020 - Day 07

- problème de cors avec le serveur (requêtes axios):
    - https://stackoverflow.com/questions/53298478/has-been-blocked-by-cors-policy-response-to-preflight-request-doesn-t-pass-acce
    - https://github.com/nelmio/NelmioCorsBundle
    - https://www.grafikart.fr/tutoriels/cors-http-navigateur-1180
- problème de commit:
    - utilisation de git revert nomducommit pour retourner en arrière
- gestion de l'authentification avec LexitJWTtoken:
    - problème de clé rsa sur le serveur:
        - résolution via chmod 644 config/jwt (problème de droit et d'accès) -> https://github.com/lexik/JWTRefreshTokenBundle/issues/366#issuecomment-437710202
- tuto sur https://github.com/markitosgv/JWTRefreshTokenBundle:
    - https://www.youtube.com/watch?v=Lj1hz-gJHD8&t=2s
  
## Sprint 2 

### 10/03/2020 - Day 01

- Documentation sur les events: 
    - https://symfony.com/doc/current/doctrine/events.html
    - https://www.doctrine-project.org/projects/doctrine-orm/en/2.6/reference/events.html
- Documentation sur les voters: 
    - https://symfony.com/doc/current/security/voters.html

### 11/03/2020 - Day 02

- Difficultés pour créer le service Delimiter:
    - réflexion mathématiques ( perimètre à gérer)
- Problèmes de regex pour le mot de passe des utilisateurs:
    -  création d'une nouvelle : https://www.imtiazepu.com/password-validation/
  
### 11/03/2020 - Day 03

- Réflexion pour débuguer le problème d'authentification avex lexiqJWT ( problème non résolu )
- Réflexion pour la mise en place d'un évènement kernel via un EventSubscriber

### 11/03/2020 - Day 04

- Problématique concernant l'upload d'image en full api :
    - http://image.intervention.io/use/basics
    - https://ourcodeworld.com/articles/read/53/how-to-upload-a-file-with-jquery-ajax-in-php-or-symfony
    - https://forum.omeka.org/t/upload-a-file-using-rest-api/3672