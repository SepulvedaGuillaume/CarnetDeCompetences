# Integration continue

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- les enjeux de l'integration continue ✔️
- la mise en place d'une github action ✔️

## 💻 J'utilise

### Un exemple personnel commenté ✔️

```yml
# Exemple de configuration GitHub Actions pour l'intégration continue

name: CI Pipeline

on:
  push:
    branches:
      - main  # Déclenche le pipeline lorsqu'un push est fait sur la branche 'main'
  pull_request:
    branches:
      - main  # Déclenche le pipeline lorsqu'une pull request est faite vers la branche 'main'

jobs:
  build:
    runs-on: ubuntu-latest  # Exécute le job sur une machine Ubuntu la plus récente

    steps:
    - name: Checkout code
      uses: actions/checkout@v3  # Utilise l'action officielle pour vérifier le code source du dépôt

    - name: Set up Node.js
      uses: actions/setup-node@v3
      with:
        node-version: '16'  # Configure Node.js à la version 16

    - name: Install dependencies
      run: npm install  # Installe les dépendances du projet

    - name: Run tests
      run: npm test  # Exécute les tests définis dans le projet

```

### Utilisation dans un projet ❌ / ✔️

[lien github](...)

Description :

### Utilisation en production si applicable❌ / ✔️

[lien du projet](...)

Description :

### Utilisation en environement professionnel ❌ / ✔️

Description :

## 🌐 J'utilise des ressources

### GitHub Actions documentation

- [Lien](https://docs.github.com/en/actions)
- Documentation officielle pour configurer et utiliser GitHub Actions.

### CI/CD for absolute beginners

- [Lien](https://medium.com/mop-developers/ci-cd-for-absolute-beginners-1dd37715001)
- Guide d'introduction aux concepts d'intégration continue et à ses avantages.

## 🚧 Je franchis les obstacles

### Point de blocage ✔️

Description:
> Difficulté à configurer correctement les secrets et variables d'environnement dans GitHub Actions, ce qui empêche le pipeline de s'exécuter correctement.

Plan d'action : 

- action 1 ✔️ : Lire la documentation officielle sur la gestion des secrets et variables d'environnement dans GitHub Actions.
- action 2 ✔️ : Configurer les secrets et variables d'environnement dans le dépôt GitHub en suivant les meilleures pratiques.
- action 3 ✔️ : Tester le pipeline après chaque configuration pour s'assurer que les secrets et variables sont correctement pris en compte.

Résolution :
> Après avoir consulté la documentation et configuré correctement les secrets et variables d'environnement, le pipeline GitHub Actions s'exécute maintenant sans problème. Les secrets sont correctement utilisés, et le pipeline fonctionne comme prévu.

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ / ✔️
- J'ai fait une [présentation](...) ❌ / ✔️
