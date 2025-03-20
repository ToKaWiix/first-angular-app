# Angular Housing App

Ce projet est une application Angular permettant d'afficher une liste de logements disponibles en récupérant les données depuis un serveur JSON.

## Prérequis

Avant de commencer, assure-toi d'avoir installé les outils suivants :
- [Node.js](https://nodejs.org/)
- [Angular CLI](https://angular.io/cli)
- [JSON Server](https://github.com/typicode/json-server)

## Installation

1. **Cloner le projet**
   ```sh
   git clone <URL_DU_REPO>
   cd first-app-angular
   ```

2. **Installer les dépendances**
   ```sh
   npm install
   ```

## Lancement de l'application

1. **Démarrer le serveur JSON**
   ```sh
   json-server --watch db.json --port 3000
   ```
   Cela démarrera un serveur local sur `http://localhost:3000/locations`.

2. **Démarrer l'application Angular**
   ```sh
   ng serve
   ```
   L'application sera accessible à l'adresse `http://localhost:4200/`.

## Structure du projet

```
first-app-angular/
│── src/
│   ├── app/
│   │   ├── home/
│   │   │   ├── home.component.ts
│   │   │   ├── home.component.html
│   │   │   ├── home.component.css
│   │   ├── housing-location/
│   │   ├── housing.service.ts
│   │   ├── routes.ts
│   ├── assets/
│   ├── main.ts
│── db.json
│── angular.json
│── package.json
│── README.md
```

## Fonctionnalités
- Affichage d'une liste de logements.
- Filtrage des logements par ville.
- Navigation entre la liste et les détails d'un logement.
- Récupération des données depuis un serveur JSON.

## Problèmes connus
- Assurez-vous que le serveur JSON est bien démarré avant de lancer l'application.
- Vérifiez que l'URL utilisée dans `housing.service.ts` correspond bien à `http://localhost:3000/locations`.

## Auteur
Anna DE MATOS