---
title: "Instalar Docker Sobre Ubuntu"
date: 2021-01-18T20:44:54-03:00
author: "Luis Zambrana"
draft: false
description: "Post para que aprendas a escribir en el lenguaje de marcado Markdown"
tags: ["docker", "ubuntu", "software libre"]
---

Pasos para la instalación:

- sudo apt update && sudo apt upgrade
- sudo apt install curl python3-pip apt-transport-https ca-certificates software-properties-common
- sudo apt install docker.io
- sudo usermod -aG docker tuusuario
- sudo systemctl enable --now docker

Para ver si esta todo ok vamos a ejecutar el comando:

- docker --version

Para ver la entrada en mi blog personal te invito a pasar a:

https://luiszambrana.com.ar/2020/05/14/instalar-docker-sobre-ubuntu-20-04/