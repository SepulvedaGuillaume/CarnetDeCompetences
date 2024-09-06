# Platform as a service

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- ce que c'est ✔️
- comment deployer une application sur une PaaS ✔️

## 💻 J'utilise

### Un exemple personnel commenté ✔️

```yml
# Exemple de déploiement d'une application Node.js sur Heroku

# Heroku est une plateforme PaaS populaire qui facilite le déploiement et la gestion des applications web.

# 1. Créez un fichier `Procfile` dans la racine de votre projet. Ce fichier indique à Heroku comment exécuter votre application.
#    Exemple de contenu du `Procfile` pour une application Node.js :
web: node index.js

# 2. Préparez votre application pour le déploiement :
#    - Assurez-vous que votre application écoute sur le port spécifié par la variable d'environnement `PORT`.
#    - Exemple d'écoute du port dans `index.js` :
const express = require('express');
const app = express();
const port = process.env.PORT || 3000; // Utilise le port fourni par Heroku ou 3000 en local

app.get('/', (req, res) => {
  res.send('Hello World!');
});

app.listen(port, () => {
  console.log(`Server running on port ${port}`);
});

# 3. Déployez l'application sur Heroku :
#    - Connectez-vous à votre compte Heroku avec `heroku login`.
#    - Initialisez un dépôt Git si ce n'est pas déjà fait :
git init
#    - Ajoutez tous les fichiers au dépôt et effectuez un commit :
git add .
git commit -m "Initial commit"
#    - Créez une nouvelle application Heroku :
heroku create
#    - Déployez votre application :
git push heroku master
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

### What is PaaS? 

- [Lien](https://www.techtarget.com/searchcloudcomputing/definition/Platform-as-a-Service-PaaS)
- Une explication de ce qu'est le PaaS, ses avantages et comment il simplifie le déploiement des applications en fournissant des environnements prêts à l'emploi.

### Heroku Deployment: Top 3 Ways to Deploy Apps to Heroku

- [Lien](https://codefresh.io/learn/heroku-deployment-top-3-ways-to-deploy-apps-to-heroku/#:~:text=To%20deploy%20on%20Heroku%2C%20you,integrations%20with%20third%2Dparty%20systems.)
- Un guide détaillé sur le déploiement d'applications sur une plateformee PaaS Heroky, incluant des étapes pratiques et des conseils pour réussir le déploiement.

## 🚧 Je franchis les obstacles

### Point de blocage ✔️

Description:
> Difficulté à comprendre comment configurer les variables d'environnement pour une application déployée sur une plateforme PaaS, ce qui entraîne des erreurs lors du démarrage de l'application.

Plan d'action : 

- action 1 ✔️ : Lire la documentation spécifique à la plateforme PaaS utilisée concernant la configuration des variables d'environnement.
- action 2 ✔️ : Créer un projet d'exemple simple sur la plateforme PaaS pour expérimenter la configuration des variables d'environnement.
- action 3 ✔️ : Vérifier les journaux de l'application pour identifier les erreurs liées aux variables d'environnement et ajuster la configuration en conséquence.

Résolution :
> J'ai consulté la documentation de la plateforme PaaS pour comprendre comment définir correctement les variables d'environnement. En créant un projet d'exemple et en testant différentes configurations, j'ai pu résoudre les erreurs liées aux variables d'environnement. Maintenant, je peux configurer les variables nécessaires pour que l'application fonctionne correctement lors du déploiement.

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ / ✔️
- J'ai fait une [présentation](...) ❌ / ✔️
