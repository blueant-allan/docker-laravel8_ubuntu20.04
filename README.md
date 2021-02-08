# Docker development container for Laravel 8 using Ubuntu 20.04 LTS as base image


Stack

* Ubuntu 20.04
* Nginx
* PHP 7.4 FPM
* Unzip

Installed PHP Extension

* Mbstring
* Xml
* Bcmath
* Intl
* Gd
* Zip
* Mysql


## Compile the docker file

```
docker build -t laravel8-image -f Dockerfile.dev .
```


## Create instance of the container

```
docker run -p 1003:80 -it --name container_name-web --mount type=bind,source="$(pwd)",target=/var/www/html laravel8-image
```

## Manage container

```
docker exec -it laravelcart-web bash
```
