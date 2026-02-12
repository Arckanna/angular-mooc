# Angular Mooc

Application Angular destinée à l'apprentissage du framework Angular dans le cadre d'une formation MOOC (cours en ligne ouvert à tous).

## Description du projet

Ce projet est une application web générée avec Angular CLI 17.0.7. Il sert de base pour suivre les exercices et tutoriels du parcours de formation Angular. L'architecture utilise les **composants standalone** (sans modules NgModule), conformément aux recommandations récentes d'Angular.

### Technologies utilisées

- **Angular** 17.x — Framework frontend
- **TypeScript** 5.2 — Langage de développement
- **RxJS** 7.8 — Programmation réactive
- **Zone.js** — Détection des changements
- **Karma** / **Jasmine** — Tests unitaires

### Structure du projet

```
angular-mooc/
├── src/
│   ├── app/
│   │   ├── app.component.ts      # Composant racine (affichage de l'état du serveur)
│   │   ├── app.component.html   # Template principal avec liens vers la doc Angular
│   │   ├── app.config.ts        # Configuration de l'application
│   │   └── app.routes.ts        # Définition des routes (vide pour l'instant)
│   ├── assets/                   # Ressources statiques (images, etc.)
│   ├── styles.css               # Styles globaux
│   ├── index.html               # Point d'entrée HTML
│   └── main.ts                  # Point d'entrée TypeScript
├── angular.json                 # Configuration du projet Angular
├── package.json                 # Dépendances npm
└── tsconfig.json               # Configuration TypeScript
```

## Prérequis

Avant de lancer le projet, assurez-vous d'avoir :

- **Node.js** (version 18 ou supérieure recommandée)
- **npm** (généralement inclus avec Node.js)

Pour vérifier vos installations :

```bash
node --version
npm --version
```

## Installation

1. **Cloner ou télécharger** le projet

2. **Installer les dépendances** à la racine du projet :

```bash
npm install
```

3. **Lancer le serveur de développement** :

```bash
npm start
```

Ou avec Angular CLI directement :

```bash
ng serve
```

4. **Ouvrir l'application** dans votre navigateur à l'adresse : [http://localhost:4200/](http://localhost:4200/)

L'application se rechargera automatiquement lorsque vous modifierez les fichiers sources.

## Commandes disponibles

| Commande | Description |
|----------|-------------|
| `npm start` ou `ng serve` | Démarre le serveur de développement (port 4200 par défaut) |
| `ng build` | Compile le projet pour la production. Les fichiers générés sont dans le dossier `dist/` |
| `ng build --watch` | Compile en mode surveillance (recompilation à chaque modification) |
| `ng test` | Lance les tests unitaires avec Karma et Jasmine |

## Génération de code (scaffolding)

Angular CLI permet de générer rapidement des éléments du projet :

| Commande | Exemple |
|----------|---------|
| Composant | `ng generate component nom-du-composant` |
| Directive | `ng generate directive nom-de-la-directive` |
| Service | `ng generate service nom-du-service` |
| Pipe | `ng generate pipe nom-du-pipe` |
| Guard | `ng generate guard nom-du-guard` |
| Interface | `ng generate interface nom-de-l-interface` |

Version courte : `ng g c nom` au lieu de `ng generate component nom`.

## Tests

- **Tests unitaires** : exécutez `ng test` pour lancer la suite de tests Karma/Jasmine.
- **Tests e2e** : pour les tests end-to-end, il faut d'abord ajouter un paquet comme Cypress ou Playwright.

## Documentation et ressources

- [Documentation officielle Angular](https://angular.dev)
- [Tutoriels Angular](https://angular.dev/tutorials)
- [Référence Angular CLI](https://angular.io/cli)
- [Angular Language Service](https://angular.dev/tools/language-service)
- [Angular DevTools](https://angular.dev/tools/devtools) — Extension pour déboguer les applications Angular

## Licence

Projet de formation — usage éducatif.
