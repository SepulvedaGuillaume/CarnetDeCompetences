# Titre de la compétence

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- l'état (_state_) pour contrôler l'affichage d'un composant ✔️
- les composants enfants et les _props_ qu'on leur passe ✔️
- le déclenchement d'instructions en fonction des actions de l'utilisateur ✔️
- le déclenchement d'instructions en fonction de l'étape du cycle de vie du composant ou du changement de valeur de ses props ✔️
- l'usage d'un reducer (_useReducer_) pour gérer un état composé dans un composant ✔️
- l'état stocké dans un composant avec un _context provider_ et accessible dans ses descendants via `useContext` ✔️

## 💻 J'utilise

### Un exemple personnel commenté ✔️

```javascript
// Exemple simple de composant React
export default function MyComponent() {
  return (
    <div className="container">
      <p className="text">Hello, React!</p>
    </div>
  );
};

.container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background-color: #f5fcff;
}

.text {
  font-size: 20px;
  text-align: center;
  margin: 10px;
}
```

### Utilisation dans un projet ✔️

[lien github](https://gitlab.com/sepulveda.guillaume/richard-et-lucy-les-cinephiles-en-folie)

Description :

### Utilisation en production si applicable ✔️
> Projet personnel en React + Express : développement d'une application web permettant aux utilisateurs de voir une liste de films populaires et consulter des informations détaillées sur ces films. Utilisation de nombreux packages et technos tels que Material-UI, Redis, JWT et Vercel pour le déploiement. Utilisation de contexts et d'hooks personnalisés pour l'authentification des utilisateurs (sécurisation des routes) et pour récupérer les datas (films) du backend avec une sécurisation via JWT Token.

[lien du projet](https://gitlab.com/sepulveda.guillaume/la-guerre-des-melodies)

Description :
> Projet personnel en React + Express : développement en React d'un blind test multijoueur côté frontend. Utilisation de contexts et d'hooks personnalisés pour la gestion des websockets et de l'authentificaton des joueurs.

### Utilisation en environement professionnel ❌ / ✔️

Description :

## 🌐 J'utilise des ressources

### Making Sense of React Hooks

- [Lien](https://medium.com/@dan_abramov/making-sense-of-react-hooks-fdbde8803889)
- Cet article de Dan Abramov sur Medium explique en détail les hooks, y compris useState, et fournit des exemples pratiques de leur utilisation.

### Introduction to Child-to-Parent Communication

- [Lien](https://blog.stackademic.com/introduction-to-child-to-parent-communication-5ca17c553366)
- Ce tutoriel décrit comment passer des props aux composants enfants et gérer la communication entre les composants parent-enfant.

## 🚧 Je franchis les obstacles

### Point de blocage ✔️

Description:
> J'avais des difficultés à comprendre comment utiliser useContext pour gérer l'état global de mon application React. Plus précisément, j'avais du mal à configurer le Context Provider et à consommer le contexte dans les composants enfants.

Plan d'action :

- action 1 ✔️ : Lire des articles et tutoriels sur useContext et la Context API pour comprendre comment configurer un contexte et l'utiliser dans les composants.
- action 2 ✔️ : Créer un exemple simple de contexte avec un Context Provider et des composants enfants pour pratiquer la configuration et l'utilisation de useContext. 
- action 3 ✔️ : Intégrer useContext dans un projet personnel pour gérer un état global, comme l'état d'authentification d'un utilisateur, afin de mieux comprendre comment appliquer ce concept à un projet réel.

Résolution : Après avoir suivi le plan d'action, j'ai réussi à configurer et à utiliser useContext dans un projet personnel. J'ai mis en place un Context Provider pour gérer l'état d'authentification des utilisateurs, et j'ai utilisé useContext pour accéder à cet état dans plusieurs composants enfants. Cette pratique m'a permis de maîtriser la gestion d'état global avec la Context API et de l'intégrer efficacement dans mon application React.

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ / ✔️
- J'ai fait une [présentation](...) ❌ / ✔️
