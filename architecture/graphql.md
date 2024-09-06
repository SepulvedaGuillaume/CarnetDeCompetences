# GraphQL

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- la différence entre REST et GraphQL ✔️
- les besoins auxquels répond GraphQL ✔️
- la définition d'un schéma ✔️
- Query ✔️
- Mutation ✔️
- Subscription ✔️

## 💻 J'utilise

### Un exemple personnel commenté ✔️

```gql
# schema.graphql 
type User {
  id: ID!
  name: String!
  email: String!
}

type Query {
  # Définition de la query 'users' pour récupérer la liste des utilisateurs
  users: [User!]!
}
```

```javascript
// resolvers.js
const users = [
  { id: '1', name: 'Alice', email: 'alice@example.com' },
  { id: '2', name: 'Bob', email: 'bob@example.com' },
  { id: '3', name: 'Charlie', email: 'charlie@example.com' },
];

// Resolvers pour les types du schéma
const resolvers = {
  Query: {
    // Resolver pour la query 'users'
    users: () => {
      return users; // Retourne la liste des utilisateurs définis plus haut
    },
  },
};
```

### Utilisation dans un projet ✔️

[lien github](https://github.com/SepulvedaGuillaume/TheGoodCorner)

Description :
> Projet de cours => Créer un clone du Bon Coin pour la vente de produits. Développement des entités côté back avec typeorm et graphql, création des résolvers (Queries et Mutations) et utilisation côté frontend. Utilisation d'Apollo Client et Server pour facilité la mise en place de graphql dans le projet.

### Utilisation en production si applicable❌ / ✔️

[lien du projet](...)

Description :

### Utilisation en environement professionnel ❌ / ✔️

Description :

## 🌐 J'utilise des ressources 

### Apollo GraphQl Tutorials

- [Lien](https://www.apollographql.com/tutorials)
- Un tutoriel complet pour apprendre à utiliser Apollo avec GraphQL avec des exemples concrets.

### The Fullstack Tutorial for GraphQL

- [Lien](https://www.howtographql.com/)
- Guide complet et gratuit pour tout savoir sur GraphQL et passer de zéro à la production. Présenté par la communauté GraphQL et Visma.

## 🚧 Je franchis les obstacles

### Point de blocage ✔️

Description: 
> J'ai eu des difficultés à implémenter des subscriptions pour les mises à jour en temps réel.

Plan d'action : 

- action 1 ✔️ : Lire la documentation sur les subscriptions.
- action 2 ✔️ : Suivre un tutoriel sur les WebSockets pour comprendre comment les subscriptions fonctionnent en arrière-plan.

Résolution :
> J'ai lu la documentation d'Apollo Server et suivi un tutoriel sur les WebSockets, ce qui m'a aidé à comprendre les configurations nécessaires. J'ai implémenté un exemple de subscription basique pour tester les mises à jour en temps réel et ajusté les configurations pour résoudre les problèmes rencontrés. Les tests ont confirmé que les subscriptions fonctionnent correctement, permettant des notifications en temps réel aux clients connectés.

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ / ✔️
- J'ai fait une [présentation](...) ❌ / ✔️
