# App-Ombi

## First Time Prerequisites

1. Run [Traefik](https://github.com/HackingServerHomelab/App-Traefik)

## Running the Containers

1. Update the following mount in [docker-compose.yml](./Docker/docker-compose.yml)
    * `../Data/config:/config`
2. Update the Traefik host label in [docker-compose.yml](./Docker/docker-compose.yml)
    * ``"traefik.http.routers.ombi.rule=Host(`localhost`)"``
3. Run `docker-compose -f ./Docker/docker-compose.yml up -d`

## First Time Setup

1. Visit <https://your-ip>
2. Follow the first time setup wizard
