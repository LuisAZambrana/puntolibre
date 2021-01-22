---
title: "Crear Un Servidor Sftp Sobre Docker"
date: 2021-01-21T09:45:34-03:00
draft: false
Author: Luis Zambrana
description: "Armar un servidor sftp sobre docker"
tags: ["docker","sftp","software libre","docker-compose"]
---

En esta oportunidad les vamos a mostrar como en menos de 5 minutos podes tener un servidor **Servidor SFTP sobre Docker**. Sin muchas vueltas, por que verdaderamente el **docker-compose.yml** es muy sencillo sobre todo si venis viendo los tutoriales sobre docker que vamos posteando poco a poco.

Encontes creamos el docker-compose.yml y en su interior:

```
sftp:
    image: atmoz/sftp
    volumes:
      - ./storage:/home/user/storage
    ports:
      - "2222:22"
    command: user:password:1000

```
Luego ejecutamos:


```
docker-compose up -d

```

y charan! a probar con cualquier cliente como filezilla etc.