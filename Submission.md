WhoRunTheWorld
Bienvenue dans l'application WhoRunTheWorld ! Cette application vous permet de créer des sondages en permettant aux utilisateurs de voter entre deux options et d'afficher les résultats en temps réel.

Fonctionnalités
Interface utilisateur conviviale pour la soumission des votes.
Collecte asynchrone des votes via Redis.
Stockage sécurisé des votes dans une base de données PostgreSQL.
Affichage en temps réel des résultats à l'aide d'une application web Node.js.
Gestion efficace des microservices grâce à Docker, Docker Compose, et Kubernetes.
Prérequis
Assurez-vous d'avoir les éléments suivants installés avant de lancer l'application :

Docker
Docker Compose
Kubernetes (pour le déploiement sur un cluster)
Lancement de l'Application en Mode Développement
Clonez le dépôt :
bash git clone https://github.com/SpookyTaru/supdevinci/tree/master

Lancez l'application en utilisant Docker Compose :

Commande: docker-compose up

L'application sera disponible à l'adresse:

http://localhost:5000

Déploiement sur un Cluster Kubernetes:

1-Faut s'assurer que le cluster Kubernetes est opérationnel. 2-Utilisez les fichiers de configuration Kubernetes fournis :

kubectl apply -f kubernetes/deployments/ kubectl apply -f kubernetes/services/

Faut suivre les logs pour être sur que l'application se deploit correctement:

kubectl logs -f deployment/worker kubectl logs -f deployment/frontend kubectl logs -f deployment/results kubectl logs -f deployment/redis kubectl logs -f deployment/database

L'application sera accessible à l'aide des services Kubernetes
