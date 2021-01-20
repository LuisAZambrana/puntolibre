---
title: "Docker Y Sus Comandos Mas Usados"
date: 2021-01-20T09:54:15-03:00
draft: false
author: Luis Zambrana
description: "Post para listar los comandos más utilizados de Docker"
tags: ["docker"]
---

En esta oportunidad un buen ayuda memoria para tener a mano los comandos más utilizados de **docker**

docker ps **Lista los contenedores en ejecución ademas de obtener el id de alguno de los contenedores.**

docker ps -a **Muestra los contenedores que están funcionando**

docker stop idcontenedor **Detiene el contenedor**

docker start idcontenedor **Inicia el contenedor**

docker rm idcontenedor **Borra el contenedor. Primero debe apagarse.**

docker stop $(docker ps -a -q) **Stopea todos los contenedores de una**

docker rm $(docker ps -a -q) **Borra todos los contenedores de una**

docker images **Nos devuelve las imágenes descargadas localmente y nos da los id correspondientes**

docker rmi idIMAGEN **Borra la imagen. Si una imagen depende de otra lo mejor es borrar desde la nueva a la vieja una por una para que no queden pequeños basureros dando vuelta ocupando lugar de gusto**

docker logs idcontenedorONombredelContenedor **Nos devuelve los logs del mismo. Muy útil para cuando el contenedor inicia y se cae.**

docker stats **Me muestra el consumo de memoria de los contenedores y espacio utilizado**

docker exec -it idContainer /bin/sh **Me deja ingresar por ssh al terminal del contenedor.**

docker network ls **Nos permite saber las redes creadas. Muchas veces ya no estan en uso luego de borrar contenedores de prueba.**

docker network rm NombredeLaRed **Mucho cuidado antes de borrar una red. Revisar que ya no haya contenedores ya que si los hay quedaran incomunidados. Las redes Bridge, Host, y Null no son posible eliminar.**

docker network disconnect MiRed MiContenedor **Este comando separa al contenedor MiContenedor de la red MiRed quedando dejandolo fuera del alcance de los contenedores que estan en esa red. Muy útil si un contenedor trae problemas.**

docker network connect MiRed MiContenedor **Este comando ayuda a incorporar al contenedor MiContenedor a la red MiRed**

