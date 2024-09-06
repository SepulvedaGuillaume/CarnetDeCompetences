# Sécurité dans le développement Web

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- Le rôle de l'OWASP ✔️
- Les injections SQL ✔️
- XSS ✔️
- CRSF ✔️

## 💻 J'utilise

### Un exemple personnel commenté ✔️

```php
<?php
// Connexion à la base de données avec PDO
$dsn = 'mysql:host=localhost;dbname=testdb';
$username = 'root';
$password = '';
$options = [PDO::ATTR_ERRMODE => PDO::ERRMODE_EXCEPTION];

try {
    $pdo = new PDO($dsn, $username, $password, $options);
} catch (PDOException $e) {
    die('Connection failed: ' . $e->getMessage());
}

// Préparation et exécution d'une requête pour éviter les injections SQL
$email = $_POST['email']; // Entrée utilisateur

// Vérification de l'entrée utilisateur pour éviter les injections SQL
if (!filter_var($email, FILTER_VALIDATE_EMAIL)) {
    die('Invalid email format');
}

// Préparation de la requête
$sql = 'SELECT * FROM users WHERE email = :email';
$stmt = $pdo->prepare($sql);
$stmt->bindParam(':email', $email, PDO::PARAM_STR);

// Exécution de la requête
$stmt->execute();

// Récupération des résultats
$results = $stmt->fetchAll(PDO::FETCH_ASSOC);

// Affichage sécurisé pour éviter les attaques XSS
foreach ($results as $user) {
    echo htmlspecialchars($user['name'], ENT_QUOTES, 'UTF-8') . '<br>';
}
?>
```

### Utilisation dans un projet ❌ / ✔️

[lien github](https://github.com/SepulvedaGuillaume/TheGoodCorner)

Description :
> Projet de cours => Créer un clone du Bon Coin pour la vente de produits. Mise en place d'une authentification via la générération d'un jeton JWT et utilisaton de la bibilothèque jsonwebtoken. Sécurisation des routes via des rôles inclus dans le token d'authentification côté front.

### Utilisation en production si applicable❌ / ✔️

[lien du projet](...)

Description :

### Utilisation en environement professionnel ❌ / ✔️

Description :

## 🌐 J'utilise des ressources

### OWASP Cheat Sheet Series

- [Lien](https://cheatsheetseries.owasp.org/index.html)
- Une série de fiches pratiques fournies par l'OWASP, couvrant les meilleures pratiques pour sécuriser les applications web contre diverses menaces comme les injections SQL et les attaques XSS.

### Web Security

- [Lien](https://developer.mozilla.org/en-US/docs/Web/Security)
- Documentation sur les pratiques de sécurité pour le développement web, incluant des informations sur les attaques courantes et les mesures de protection recommandées.

## 🚧 Je franchis les obstacles

### Point de blocage ✔️

Description:
> Difficulté à intégrer la génération et la validation des jetons JWT dans un projet TypeScript, notamment pour gérer l'authentification et l'autorisation des utilisateurs.

Plan d'action :

- action 1 ✔️ : Étudier la documentation de la bibliothèque JWT pour Node.js, comme jsonwebtoken, et comprendre comment l'utiliser avec TypeScript.
- action 2 ✔️ : Implémenter la génération d'un jeton JWT lors de l'authentification de l'utilisateur et la validation de ce jeton pour protéger les routes de l'application.

Résolution : 
> J'ai intégré la bibliothèque jsonwebtoken dans mon projet TypeScript pour générer des jetons JWT lors de l'authentification des utilisateurs et valider ces jetons pour les requêtes protégées. J'ai testé la génération et la validation des jetons, ce qui a confirmé que les fonctionnalités d'authentification et d'autorisation étaient correctement mises en place.

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ / ✔️
- J'ai fait une [présentation](...) ❌ / ✔️
