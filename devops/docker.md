# Docker

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- la création d'une image docker ✔️
- l'éxécution d'un container ✔️
- l'orchestration de containers avec docker-compose ✔️


## 💻 J'utilise

### Un exemple personnel commenté ✔️

```yml
# Exemple de docker-compose.yml
services:
  app:
    build: .
    volumes:
      - ./app:/usr/src/app
    ports:
      - "8080:8080"
```

```yml
# Exemple de Dockerfile

# Utiliser une image de base officielle de Node.js. L'image officielle assure que nous avons une version stable et fiable de Node.js.
FROM node:lts-alpine

# Créer un répertoire de travail dans le conteneur. Cela permet de structurer notre application et de garder les fichiers organisés.
WORKDIR /app

# Copier les fichiers package.json et package-lock.json dans le répertoire de travail du conteneur. 
COPY package*.json ./

# Installer les dépendances de l'application. Cette étape utilise npm pour récupérer toutes les dépendances listées dans package.json.
RUN npm install

# Copier le reste du code de l'application dans le répertoire de travail du conteneur.
COPY . .

# Exposer le port 3000 sur lequel l'application écoute. Cela permet à Docker de savoir quel port utiliser pour les connexions.
EXPOSE 3000

# Définir la commande à exécuter lorsque le conteneur démarre.
CMD ["npm", "run", "dev"]
```

### Utilisation dans un projet ✔️

[lien github](https://github.com/SepulvedaGuillaume/TheGoodCorner)

Description :
> Projet de cours => Créer un clone du Bon Coin pour la vente de produits. Mise en place de la dockerisation sur le projet. Création d'un fichier docker-compose.yml pour lancer des services buildés pour le frontend et backend et à partir d'image existante pour postgres, admirer et pgadmin. Définition des Dockerfile, des volumes et des variables d'environnement.

### Utilisation en production si applicable❌ / ✔️

[lien du projet](...)

Description :

### Utilisation en environement professionnel ❌ / ✔️

Description :

## 🌐 J'utilise des ressources

### Learn Docker Beginner to Expert

- [Lien](https://medium.com/@kmdkhadeer/docker-get-started-9aa7ee662cea)
- Un guide pour monter en compétences sur Docker, comprendre les concepts fondamentaux, l'installer et créer des images.

### Docker Compose Quickstart

- [Lien](https://docs.docker.com/compose/gettingstarted)
- Un guide détaillé sur Docker Compose, expliquant comment orchestrer plusieurs conteneurs et configurer des applications multi-services.

## 🚧 Je franchis les obstacles

### Point de blocage ✔️

Description:
> Difficulté à comprendre comment correctement exposer les ports dans un conteneur Docker pour accéder à l'application depuis l'extérieur.

Plan d'action : 

- action 1 ✔️ : Lire la documentation officielle de Docker sur l'exposition des ports et la configuration des règles de publication.
- action 2 ✔️ : Configurer un simple conteneur Docker avec une application web de base, en exposant les ports nécessaires.
- action 3 ✔️ : Vérifier que l'application est accessible depuis le navigateur en utilisant l'adresse localhost et le port exposé.

Résolution :
> J'ai appris à exposer les ports correctement en modifiant le Dockerfile pour inclure EXPOSE 8080 et en utilisant la configuration appropriée dans le docker-compose.yml pour mapper le port du conteneur au port de l'hôte. Après avoir testé la configuration, j'ai pu accéder à l'application via localhost:8080, ce qui a confirmé que les ports étaient correctement exposés et m'a permis de résoudre le problème d'accès à l'application.

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ / ✔️
- J'ai fait une [présentation](...) ❌ / ✔️
