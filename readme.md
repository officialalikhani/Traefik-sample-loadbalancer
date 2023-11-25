# Traefik Load Balancer with Nginx

This repository provides a sample setup for running a Traefik load balancer with three Nginx instances.

## Prerequisites

- Docker and Docker Compose installed on your machine.

## Getting Started

Clone this repository:

 ```bash
 git clone https://github.com/officialalikhani/Traefik-sample-yaml.git

```

Update the docker-compose.yml file:

    Specify the desired domain name for your load balancer in the traefik.http.routers.traefik.rule label.
    Update the Nginx container configurations (e.g., port, volumes, etc.) if needed.

Start the Traefik load balancer and Nginx containers:

```bash
docker compose up -d
```

This command will start the Traefik load balancer and three Nginx instances.

Verify the setup:

    Open your web browser and navigate to http://localhost or the domain name
    You should see the default Nginx welcome page.
    Refresh the page multiple times to observe Traefik's load balancing in action, as the requests are distributed across the Nginx instances.

Cleanup:

To stop and remove the containers, run the following command:

```bash
docker compose down
```

This will remove the Traefik load balancer and Nginx containers.

Configuration!

