# Laravel 5.6 Docker Sample

This is sample how to run laravel project into Docker conatiner.

## Installation

Run this command

```
git clone https://github.com/ar-android/laravel-docker

cd laravel-docker

cp src/.env.example src/.env

docker-compose run --rm --no-deps blog-server composer install

docker-compose run --rm --no-deps blog-server php artisan key:generate

docker-compose run --rm --no-deps blog-server php artisan migrate

docker-compose up -d

# If you are using docker-machine open the machine ip
http://docker-machine-ip/

# If you not using docker-machine
http://localhost/
```
