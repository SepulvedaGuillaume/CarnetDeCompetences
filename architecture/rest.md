# REST API

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- les verbes HTTP ✔️
- les statuts HTTP ✔️
- les endpoints ✔️
- CORS ✔️
- la nomenclature recommandée pour les routes ✔️

## 💻 J'utilise

### Un exemple personnel commenté ✔️

```javascript
// Exemple de route pour créer une nouvelle tâche avec Express
const express = require('express');
const app = express();
app.use(express.json());

let tasks = [];

// POST /tasks - Crée une nouvelle tâche
app.post('/tasks', (req, res) => {
  const task = { id: tasks.length + 1, title: req.body.title, completed: false };
  tasks.push(task);
  res.status(201).json(task); // Statut 201 pour indiquer une création réussie
});

app.listen(3000, () => console.log('Server running on port 3000'));
```

### Utilisation dans un projet ❌ / ✔️

[lien github](https://github.com/SepulvedaGuillaume/TheGoodCorner)

Description :
> Projet de cours => Créer un clone du Bon Coin pour la vente de produits. Développement sous TypeScript (TSX pour React). Création de routes REST via les verbes HTTP GET, POST, PUT et DELETE pour la gestion des annonces, des catégories et des tags pour la récupération côté frontend.

### Utilisation en production si applicable ✔️

[lien du projet](https://gitlab.com/sepulveda.guillaume/la-guerre-des-melodies)

Description :
> Projet personnel en React + Express : développement en javascript (JSX pour React et JS pour le reste) d'un blind test multijoueur. Création de endpoints côté backend pour la récupération, ajout, modification et suppression des parties, musiques et utilisateurs.

### Utilisation en environement professionnel ❌ / ✔️

Description :

## 🌐 J'utilise des ressources

### Learn REST API Design

- [Lien](https://www.restapitutorial.com)
-  Un site dédié aux API REST qui couvre les bases, les verbes HTTP, la gestion des statuts, les bonnes pratiques, et les erreurs courantes dans la conception d'API.

### HTTP response status codes

- [Lien](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status)
- Explication détaillée des codes de statut HTTP pour mieux comprendre les réponses des serveurs REST.

## 🚧 Je franchis les obstacles

### Point de blocage ✔️

Description:
> Difficulté à gérer le CORS lors des requêtes cross-origin, provoquant des erreurs d'accès depuis le frontend.

Plan d'action :

- action 1 ✔️ : Lire la documentation sur le CORS et comprendre comment les en-têtes HTTP sont utilisés pour gérer les requêtes cross-origin.
- action 2 ✔️ : Implémenter et tester différentes configurations CORS dans Express pour permettre des requêtes depuis le frontend sans compromettre la sécurité.

Résolution : 
> J'ai configuré les en-têtes CORS en utilisant le middleware cors dans Express, ce qui a permis de résoudre les problèmes d'accès cross-origin. Des tests supplémentaires ont confirmé que l'API REST fonctionne correctement avec les clients frontend, sans erreurs de CORS.

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ / ✔️
- J'ai fait une [présentation](...) ❌ / ✔️
