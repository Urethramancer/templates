# Templates
A collection of basic templates to quickly make Docker images.

## Go
Go configurations.

### go-minimal
The bare minimum required to build and run a Go app. Required packages are downloaded, and a tiny image is built. Hello World will be around 800k.

## PHP
PHP configurations.

### php7-apache-debian
Based on official PHP images. Sets up PHP7 with Apache in front.

* docker-compose-mysql-stretch: Debian Stretch-based image and embedded MySQL from the latest official image.

## Redmine
Redmine issue tracker config which actually works.

### redmine
Based on official Postgres and Redmine images, using latest.

* docker-compose-postgres: Sets up database and server with persistent directories outside.
