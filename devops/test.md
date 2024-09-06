# Tester son application

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- les tests unitaires ✔️
- les mocks ✔️
- les tests d'integration ✔️
- les tests de bout en bout (end to end) ✔️
- le TDD ✔️
- les tests par snapshot ✔️

## 💻 J'utilise

### Un exemple personnel commenté ✔️

```javascript
// Exemple de tests unitaires avec Jest pour une fonction simple d'addition

// Fonction à tester
function add(a, b) {
  return a + b;
}

// Test unitaire
test('ajoute 1 + 2 pour obtenir 3', () => {
  expect(add(1, 2)).toBe(3);
});
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

### Jest Documentation

- [Lien](https://jestjs.io/docs/getting-started)
- Documentation officielle de Jest pour écrire et exécuter des tests unitaires et d'intégration.

### React Testing Library

- [Lien](https://testing-library.com/docs/react-testing-library/intro)
- Guide complet sur les tests d'interface utilisateur avec Testing Library, adapté pour les tests de bout en bout.

## 🚧 Je franchis les obstacles

### Point de blocage ✔️

Description:
> Difficulté à isoler les tests unitaires en raison de dépendances externes non mockées, ce qui entraîne des échecs de test lorsqu'une API externe n'est pas disponible.

Plan d'action : 

- action 1 ✔️ : Identifier les dépendances externes utilisées dans les tests et les remplacer par des mocks pour isoler les tests unitaires.
- action 2 ✔️ : Utiliser des bibliothèques de mocking comme jest.mock pour simuler les réponses des API externes.
- action 3 ✔️ : Exécuter les tests unitaires avec les mocks pour s'assurer que les tests passent indépendamment des services externes.

Résolution :
> En remplaçant les dépendances externes par des mocks dans les tests unitaires, j'ai réussi à isoler les tests et à éviter les échecs causés par l'indisponibilité des API externes. Les tests unitaires fonctionnent maintenant de manière fiable et indépendante des services externes.

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ / ✔️
- J'ai fait une [présentation](...) ❌ / ✔️
