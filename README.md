# Docker (Matomo - MariaDB)

[Matomo](https://matomo.org) is the leading open-source analytics platform that gives you more that just powerful analytics:

- Free open-source software
- 100% data ownership
- User privacy protection
- User-centric insights
- Customisable and extensible

## How to Use

1. Clone repository
1. Update config
    1. `docker-compose.yml`
        - `MYSQL_ROOT_PASSWORD`
    1. `db.env`
        - `MYSQL_PASSWORD`
1. Run
    - Deploy
        - `docker compose up --build`
    - `--build`
        - Builds the image before starting the container

## Clean-up

1. Get a list of all containers and delete
    - `docker container ls -a`
    - `docker container rm [OPTIONS] CONTAINER [CONTAINER...]`
1. Get and remove the images
    - `docker image ls -a`
    - `docker image rm [OPTIONS] CONTAINER [CONTAINER...]`
1. Prune the volumes
    - `docker volume prune`