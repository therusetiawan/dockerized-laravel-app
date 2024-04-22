## Dockerized Laravel App
A sample dockerized laravel app. 

## Usage

Make sure you have docker and docker compose on your machine.

[How To Install and Use Docker on Ubuntu](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-18-04)

[How To Install Docker Compose on Ubuntu](https://www.digitalocean.com/community/tutorials/how-to-install-docker-compose-on-ubuntu-18-04)

Clone the project

`cd` into the project directory

Run `docker-compose up -d`

This will build two docker container

app, webserver

Run composer install

```
docker-compose exec composer install
```

Generate app key

```
docker-compose exec app php artisan key:generate
```

Database migration
```
docker-compose exec app php artisan migrate
```
