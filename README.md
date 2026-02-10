# DICEMEET

Application web full stack concue, développée et déployée dans le cadre de mon projet de fin d'étude.  
Le projet avait pour objectif la réalisation d’une application complète, avec une attention particulière portée à l’architecture, à la sécurité et au déploiement.

## Objectifs du projet
- Concevoir une application web fonctionnelle, avec un cahier des charges et un concept entierement personnalisé.
- Réaliser l’ensemble du projet: conception UX/UI (Figma), backend, frontend et déploiement
- Mettre en place une architecture claire avec séparation frontend / backend
- Déployer l’application sur VPS dans un environnement sécurisé

## Architecture générale
Le projet est structuré en deux parties distinctes:

- **Backend**: API REST développée avec Symfony 8
  https://github.com/StephaneLay/Dicemeet_API

- **Frontend**: Front-end developpé avec Angular 20 consommant l’API  
 https://github.com/StephaneLay/Dicemeet

## Stack technique

### Backend
- Symfony 8
- MySQL
- API REST
- Authentification et sécurité via JWT

### Frontend
- Angular 20
- TypeScript
- HTML / CSS 

## Fonctionnalités principales
- Authentification des utilisateurs et stockage sécurisé des données
- API Restful avec routes personnalisées et configurées selon permissions
- Utilisation recurrente d'evenements CRUD, de voters et de normalizers
- Communication sécurisée entre le frontend et le backend

## Déploiement
L’application a été entièrement déployée sur un VPS Ubuntu hébergé chez OVH, avec:
- configuration serveur
- gestion des variables d’environnement
- noms de domaine personnalisés

## Améliorations possibles
- ajout de plus de tests automatisés
- amélioration des performances malgré tests lighthouse satisfaisants
- dockerisation du projet

## Contexte
Projet réalisé en autonomie, de la conception à la mise en production SANS INTELLIGENCE ARTIFICIELLE !

## Documentation complémentaire
Un dossier de conception détaillé est disponible dans le repo

## Demonstration de trois fonctionnalités clés
- Recherche filtrée et paginée : https://drive.google.com/file/d/1OVhLg33-nWRZD4W5beKkYUalvFVqbI5V/view?usp=drive_link
- Edition de profil : https://drive.google.com/file/d/12Ub5twLUw9Ij68e6WIsOuX0GHgroC5ty/view?usp=drive_link
- Gestion d'evenements administrateur : https://drive.google.com/file/d/1YxdbMuFf3bOP-8JSu4rv4p_fgfZ-5umF/view?usp=drive_link

## Lancer le projet en local
L'hebergement par OVH n'étant plus actif voici les instructions pour lancer le projet en local:

###Backend
git clone https://github.com/StephaneLay/Dicemeet_API
composer install
php bin/console d:d:c
php bin/console d:m:m
symfony serve --no-tls

###Frontend
git clone https://github.com/StephaneLay/Dicemeet
npm install
ng serve
