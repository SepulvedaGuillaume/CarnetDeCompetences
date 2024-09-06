# Microservices

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- les différences avec l'architecture monolithique ✔️
- la communication asynchrone entre services ✔️
- le deploiement d'un cluster ✔️

## 💻 J'utilise

### Un exemple personnel commenté ✔️

> J'ai développé une application composée de plusieurs microservices (gestion des utilisateurs, commandes et paiements). Chaque service communique via des événements publiés et consommés sur Kafka, ce qui permet une communication asynchrone et découplée.

```javascript
const kafka = require('kafka-node');
const Producer = kafka.Producer;
const client = new kafka.KafkaClient({ kafkaHost: 'localhost:9092' });
const producer = new Producer(client);

const order = { orderId: '123', userId: '456', amount: 100 };

producer.on('ready', () => {
  producer.send(
    [{ topic: 'order-created', messages: JSON.stringify(order) }],
    (err, data) => {
      if (err) {
        console.error('Erreur lors de la publication du message', err);
      } else {
        console.log('Message publié avec succès', data);
      }
    }
  );
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

### Microservice Architecture

- [Lien](https://microservices.io)
- Un guide complet sur l'architecture des microservices.

### Kafka Documentation

- [Lien](https://kafka.apache.org/documentation)
- Documentation officielle pour comprendre et configurer Kafka pour les microservices.

## 🚧 Je franchis les obstacles

### Point de blocage ✔️

Description:
> Difficulté à configurer Kafka pour assurer la fiabilité des messages entre les services.

Plan d'action : 

- action 1 ✔️ : Lire la documentation Kafka sur la configuration des brokers et des partitions.
- action 2 ✔️ : Suivre un tutoriel sur la gestion des consommateurs et des producteurs.

Résolution :
> J'ai réussi à configurer Kafka sur mon projet pro en lisant la documentation et en suivant les différents tutoriels à ma disposition. J'ai testé différentes configurations pour gérer les erreurs de production et les redémarrages automatiques.

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ / ✔️
- J'ai fait une [présentation](...) ❌ / ✔️
