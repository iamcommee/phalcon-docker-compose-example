<img align="right" width="175px" src="http://i.imgur.com/mdZ8Ktf.png" />
<img align="right" width="175px" height="100px" src="https://d33wubrfki0l68.cloudfront.net/5a27d37defa5f82b8542756e2ecb0108db2f5a45/eb216/assets/images/footer_logo.svg" />


# Phalcon Docker Compose

The unofficial Phalcon Docker Environment

This is an unofficial example for Phalcon projects that run on [Docker][:docker:] and [Phalcon][:phalcon:].
The purpose of this repository is making it easier to develop phalcon project for development and production environments.


## Get Started

1. Install [Docker][:docker:] for your OS
2. Clone or Download this repo then extract it

```bash
git clone https://github.com/commee67/phalcon-docker-compose-example.git
cd phalcon-docker-compose-example
docker-compose up
```

3. Check your local with localhost , 127.0.0.1 in your browser. Done!

## Usage

1. Dockerfile - You can manage php extension or change the version of php in docker/app/Dokerfile. eg.
```
FROM php:7.2-apache -> php:7.x-apache

ARG PHALCON_VERSION=3.4.3 -> PHALCON_VERSION=4.0.0-alpha.5 ( not recommend because there are some problems)

```
 List version here - [phalcon-version][:phalcon-version:]
 
 **Note : When you change Dockerfile, remember you have to run docker-compose build before docker-compose up.**
 
 2. docker-compose.yml - You can add service here. such as memcached-server , phpmyadmin , etc.
 
 3. variables.env - This file use to define the environment variable of service.

 Note : You have to look the variable in your image. eg. [mysql-docker][:mysql-docker:] (Environment Variables Section)
 
 4. application folder - This folder is the directory of your project.
   
[:phalcon:]:        https://github.com/phalcon/cphalcon
[:docker:]:         https://www.docker.com
[:phalcon-version:]:  https://github.com/phalcon/cphalcon/releases
[:mysql-docker:]:   https://hub.docker.com/_/mysql
