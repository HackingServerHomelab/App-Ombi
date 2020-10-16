# App-Ombi

## Running the Containers

1. Run `./Config/gen_certs.sh` to generate the SSL certificates (alternatively,
   add custom certs to the private folder)
2. Update the `server_name` in [nginx.conf](./Config/nginx.conf)
3. Update the following mount in [docker-compose.yml](./Docker/docker-compose.yml)
    * `../Data/config:/config`
4. Run `docker-compose -f ./Docker/docker-compose.yml up -d`

## First Time Setup

1. Visit <https://your-ip>
2. Follow the first time setup wizard
