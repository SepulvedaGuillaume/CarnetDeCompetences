# Titre de la compétence

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- Comment développer en utilisant un système de *livereloading* (`nodemon` par exemple) ✔️
- La connexion de mon application à une base de données avec et sans ORM/ODM (avec `mongodb` puis `mongoose` par exemple) ✔️
- Le développement d'une API REST et GraphQL (avec les packages `express` et `graphql` par exemple) ✔️
- *Bonus : la manipulation des fichiers système avec `fs` et l'utilisation des streams en NodeJS* ✔️

## 💻 J'utilise

### Un exemple personnel commenté ❌ / ✔️

```javascript
// this function takes a path to a .md file of the host system and write the HTML version of this file
// the .html file is given back
const convertMDFileToHTML = (pathToMDfile) => {
  const fs = require('fs');
  const marked = require('marked');

  // Lecture du fichier .md
  const markdown = fs.readFileSync(pathToMDfile, 'utf8');

  // Conversion en HTML
  const htmlContent = marked(markdown);

  // Chemin du fichier HTML à créer
  const pathToHTMLfile = pathToMDfile.replace('.md', '.html');

  // Écriture du contenu HTML dans le fichier
  fs.writeFileSync(pathToHTMLfile, htmlContent);

  return pathToHTMLfile;
};
```

### Utilisation dans un projet ❌ / ✔️

[lien github](https://github.com/SepulvedaGuillaume/TheGoodCorner)

Description :
> Projet de cours => Créer un clone du bon coin pour la vente de produits. Apprentissage avec Express, TypeOrm, GraphQL dans un environnement Node.js.

### Utilisation en production si applicable❌ / ✔️

[lien du projet](https://gitlab.com/sepulveda.guillaume/la-guerre-des-melodies)

Description :
> Projet personnel en React + Express : développement d'un blind test multijoueur. Possibilité d'uploader des musiques via Youtube en utilisant des packages comme ffmpeg et ytdl-core => transformation des vidéos en mp3 et découpage des 30 premières secondes. Connexion à une base de données noSql avec MongoDB. Utilisation du package mongoose qui sert de passerelle entre mon serveur Node.js et ma base de données MongoDB.

### Utilisation en environement professionnel ❌ / ✔️

Description :

## 🌐 J'utilise des ressources

### Nodemon

- [Lien](https://nodemon.io)
- Le site officiel de nodemon m'a aidé à configurer le livereloading pour un développement plus efficace et réactif.

### Mongoose

- [Lien](https://mongoosejs.com)
- Cette ressource m'a aidé à apprendre comment utiliser mongoose pour interagir avec une base de données MongoDB.

## 🚧 Je franchis les obstacles

### Point de blocage ✔️

Description:
> J'avais des difficultés à comprendre et à mettre en place une authentification sécurisée dans une application NodeJS, en particulier l'utilisation de JWT (JSON Web Tokens).

Plan d'action :

- action 1 ✔️ : Suivre des tutoriels spécifiques sur l'authentification avec JWT dans NodeJS.
- action 2 ✔️ : Étudier les meilleures pratiques de sécurité pour le stockage et la gestion des tokens.
- action 3 ✔️ : Implémenter une solution d'authentification avec JWT dans un projet personnel, en suivant les étapes de création, vérification et renouvellement des tokens.

Résolution : 
> Après avoir suivi les tutoriels et mis en œuvre les solutions dans un projet personnel, j'ai réussi à comprendre les mécanismes de JWT et à implémenter une authentification sécurisée dans mon application. J'ai également appris à gérer les sessions et à protéger les routes sensibles, garantissant ainsi une meilleure sécurité pour les utilisateurs.

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ / ✔️
- J'ai fait une [présentation](...) ❌ / ✔️
