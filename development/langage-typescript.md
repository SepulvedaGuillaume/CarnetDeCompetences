# TypeScript

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- l'intéret de TypeScript dans l'IDE ✔️
- les types de bases ✔️
- comment et pourquoi étendre une interface ✔️
- les classes et les decorators ✔️

## 💻 J'utilise

### Un exemple personnel commenté ✔️

```typescript
// Déclaration d'une fonction fléchée qui calcule l'énergie d'une masse donnée
const calculateEnergy = (mass: number): number => {
  const speedOfLight: number = 299792458; // Vitesse de la lumière en mètres par seconde
  return mass * speedOfLight ** 2; // Formule E=mc^2
};

// Exemple pour 1 kilogramme 
console.log(calculateEnergy(1)); // Affiche 8.987551787368176e+16 (J)
```

### Utilisation dans un projet ✔️

[lien github](https://github.com/SepulvedaGuillaume/TheGoodCorner)

Description :
> Projet de cours => Créer un clone du Bon Coin pour la vente de produits. Développement sous TypeScript (TSX pour React). Définition d'interfaces et de types avec implements et extends. Utilisation de codegen pour générer du code peuvent créer des types TypeScript ou des fragments GraphQL à partir de schémas GraphQL.

### Utilisation en production si applicable❌ / ✔️

[lien du projet](...)

Description :

### Utilisation en environement professionnel ❌ / ✔️

Description :

## 🌐 J'utilise des ressources

### Basic Types

- [Lien](https://www.typescriptlang.org/docs/handbook/basic-types.html)
- Ce guide couvre les types de base en TypeScript, y compris string, number, boolean, array, tuple, enum, any, void, null, et undefined. Il explique comment déclarer et utiliser ces types pour améliorer la robustesse du code.

### Extending Interfaces in TypeScript

- [Lien](https://www.typescriptlang.org/docs/handbook/interfaces.html)
- Ce document détaille comment créer et étendre des interfaces en TypeScript. L'extension d'interfaces permet de réutiliser des types et d'ajouter des fonctionnalités supplémentaires sans modifier les interfaces existantes, ce qui conduit à un code plus modulaire et maintenable.

### TypeScript Decorators

- [Lien](https://www.typescriptlang.org/docs/handbook/decorators.html)
- Ces sections du manuel TypeScript expliquent comment utiliser les décorateurs.Ces derniers fournissent une manière puissante d'ajouter des métadonnées et de modifier le comportement des classes et de leurs membres de manière déclarative.

## 🚧 Je franchis les obstacles

### Point de blocage ✔️

Description:
> J'avais du mal à comprendre comment et pourquoi utiliser les décorateurs dans les classes TypeScript.

Plan d'action : 

action 1 ✔️ : J'ai suivi un tutoriel détaillé sur les décorateurs pour comprendre leur fonctionnement.
action 2 ✔️ : J'ai pratiqué en manipulant des décorateurs pour mon projet The Good Corner (clone le Bon Coin). Utilisation de décorateurs sur mes entités TypeORM et mes résolvers GraphQL.

Résolution :
> Après avoir suivi le tutoriel et pratiqué régulièrement, j'ai acquis une bonne compréhension de l'utilisation des décorateurs. Je les utilise maintenant pour ajouter des fonctionnalités et des métadonnées à mes classes.

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ / ✔️
- J'ai fait une [présentation](...) ❌ / ✔️
