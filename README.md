# Docker-Compose [Traefik-Nginx-Mysql-Adminer-Nextcloud-Redis]

Cette stack vous permet d'avoir votre environnement  nextcloud derrière un reverse proxy comme traefik.

## Pre-requis

* Os Linux Ubuntu 18.04
* Docker & Docker-Compose installé sur la machine.
* Un nom de domaine et un enregistrement DNS pointé sur le domaine pour permettre à Traefik de génerer votre SSL

## Comment utilisé la stack ?

* Vous devez cloner le projet : git clone https://github.com/enassar225/docker-nextcloud-single-node.git
* Modifier le fichier .env dans le meme répertoire ou se trouve le projet
* Si vous ne modifiez pas le fichier .env, les variables par defaut dans la stack seront celles qui seront utilisées.
* Lancez la stack en tapant : docker-compose -f nextcloud.yml -f traefik.yml up -d

## Sources

* https://docs.docker.com/engine/install/ubuntu/ && https://docs.docker.com/compose/install/
* https://hub.docker.com/_/nextcloud
* https://github.com/nextcloud/docker/tree/master/.examples
