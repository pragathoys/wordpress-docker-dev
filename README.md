# wordpress-docker-dev
A Docker Compose YAML file for quick Wordpress development. It fetches the latest version of Wordpress.

# Configuration

Before starting the container dont forget to change the username and password of the WP admin, db user

# Just ...

- Inside the folder run: docker compose up [to start the stack]
- open your browser to http://localhost:9090 [for the latest WP]
- open your browser to http://localhost:9091 [to admin the DB]
- hit: Ctrl+c [to stop the stack]

# Network

If you want to connect the docker in a different network eg. proxy :

- docker network connect proxy <container_id>

# Updating

- docker compose down
- docker compose pull
- docker compose up --build
