## Dockerize web app (PHP, Lavarel, MySQL, NGINX)

#### Services principaux:

- Nginx : Server qui reçoit les requêtes venant des utilisateurs sur le port 8000
- Php: Gérer la logique et retourner des réponses
- MySql: Base de donnée

#### Services utilitaires:

- Composer: Générer le projet Lavarel
- Artisan: Initialiser la base de données
- Npm: installation des dépendances pour certaine parties front

### Start all services:

    docker-compose up -d --build server

### Stop all service and remove all volumes:

    docker-compose down -v

Note: </br>
For production: A snapshot of each service is created by copying the source code or config file into the image.</br>
For development: All bind mount volumes are kept.
