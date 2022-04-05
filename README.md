# React TS template

[![Node.js CI](https://github.com/semifir/react-ts-template/actions/workflows/nodejs.yml/badge.svg)](/react-ts-template/actions/workflows/nodejs.yml)

Ce projet sert de repository template pour les applications React en Typescript.

## Préparer le projet

Pour lancer le projet React, installer les dépendances: `npm i` ou `npm install`.

Ajouter les hooks à git si ce n'est pas déjà fait: `git config --global core.hooksPath ./.githooks`
> Ceci va activer les hooks qui vérifient le style du code et valider les messages de commit.

## Lancer le projet

Le package.json contient le script pour démarrer l'application React:
`npm start`

## Bonnes pratiques React

Quelques sites pour les bonnes pratiques à respecter:

- [betterprogramming.pub: 21 best practices for a clean react project](https://betterprogramming.pub/21-best-practices-for-a-clean-react-project-df788a682fb)

- [TatvaSoft: REACT BEST PRACTICES AND SECURITY](https://www.tatvasoft.com/blog/reactjs-best-practices/)

- [freecodecamp: React Best Practices – Tips for Writing Better React Code in 2022](https://www.freecodecamp.org/news/best-practices-for-react/)

- [15 React Best Practices You Need to Follow in 2022](https://www.codeinwp.com/blog/react-best-practices/)

Évidemment ces bonnes pratiques s'ajoute à SOLID, DRY, KISS, YAGNI, etc.

## Lancer les tests

Par defaut ce repo utilise Jest pour tester les composants.

Vous pouvez lancer les tests avec `npm test`

Si vous changez la façon de faire des tests changez le script du *package.json*.

## Formater le projet

Le projet vient avec ESLint et prettier, pour simplifier le format du code il est possible de vérifier le lint de tout le projet avec `npx run lint`.

## Construire le projet pour la production

Pour servir le projet dans un environnement de production, il faut construire le projet React.

Pour construire le projet `npm run build`

## SonarQube

Ce projet contient une config de base de pour SonarQube.
Il peut être utilisé avec un [Sonar scanner](https://docs.sonarqube.org/latest/analysis/scan/sonarscanner/) ou équivalent ou via [github actions](https://docs.sonarqube.org/latest/analysis/github-integration/).

## CICD

Dans le dossier [workflow](./github/worflows) se trouve les workflow CICD de [GitHub Actions](https://github.com/features/actions).

Vous y trouverez 2 fichiers:

- [nodejs.yml](/.github/workflows/nodejs.yml) avec le CI build et test de l'app
- [docker-build-and-package.yml](/.github/workflows/docker-build-and-package.yml) avec le CD build image docker et push sur le registry GitHub du repo (cf: [packages du repo](/packages))

## Dependances

- React: 17.0.2

## TODO

- [x] Ajouter les tests
- [x] Ajouter la config de SonarQube
- [x] Ajouter la génération du coverage
- [x] Ajouter les bonnes pratiques
- [x] Ajouter les hooks
- [x] Automatiser l'installation
- [x] Ajouter le CICD
  - [x] Ajouter le buil et test de l'app
  - [x] Ajouter le packaging Docker
- [x] Ajouter ESLint
- [x] Ajouter Prettier
- [ ] Ajouter les liens vers les process
  - [ ] Convention de commit
  - [ ] Procedure de pull request
  - [ ] Procedure de soumission d'issue
- [x] Ajouter le .gitignore
- [x] Ajouter les templates github
- [x] Ajouter le README
