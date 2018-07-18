# Laravel 5.6 Docker Sample

This is sample how to run laravel project into Docker conatiner.

## Installation

Clone this repository

```
git clone https://github.com/ar-android/laravel-docker
```
Open the directory project
```
cd laravel-docker
```
Copy eniroment file
```
cp src/.env.example src/.env
```
Inatall php dependencies
```
docker-compose run --rm --no-deps blog-server composer install
```
Generate laravel key
```
docker-compose run --rm --no-deps blog-server php artisan key:generate
```
Migrate database
```
docker-compose run --rm --no-deps blog-server php artisan migrate
```
Run docker compose as daemon
```
docker-compose up -d
```

# If you are using docker-machine open the machine ip
http://docker-machine-ip/

# If you not using docker-machine
http://localhost/
```
