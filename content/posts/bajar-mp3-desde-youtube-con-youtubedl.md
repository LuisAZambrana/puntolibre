---
title: "Bajar Mp3 Desde Youtube Con Youtubedl"
date: 2021-01-21T14:08:27-03:00
draft: false
description: "Bajar Mp3 Desde Youtube Con Youtubedl"
tags: ["mp3","youtubedl","software libre","youtube", "tutoriales"]
---

Hola amigos como andan? Espero que muy muy bien!!! Muchos de uds seguro tendrán alguna app de **streaming de audio** pago o gratuito con el cual disfrutar de musica offline en viajes o momentos en los que no contamos con conectividad. En esta oportunidad les traigo un pequeño tutorial para instalar **youtube-dl** y obviamente ver como se hace para Bajar mp3 desde un video en youtube con youtube-dl en dos simples pasos. Si les gusta, como siempre les pido, compartan en su redes sociales y mil mil gracias por pasar!!

**La instalación de youtube-dl** la vamos a hacer en este tutorial sobre Ubuntu pero bien funciona en sistemas operativos de la misma base (debian, mint etc).

Primero actualizamos por las dudas:

```
sudo apt update && sudo apt upgrade
sudo apt install curl
sudo curl -L https://yt-dl.org/downloads/latest/youtube-dl -o /usr/local/bin/youtube-dl
sudo chmod a+rx /usr/local/bin/youtube-dl

```

Luego con la url del video que queremos bajar nos queda pararnos en una carpeta donde queramos que quede nuestra musica y ejecutar:

```
youtube-dl --extract-audio --audio-format mp3 https://www.youtube.com/watch?v=nbjAnwgNgS4

```
Lo mas importante para que tengas en cuenta que el link de youtube va a tener un identificador y necesitamos aprender a reconocerlo. En el ejemplo anterior veremos que es: 'nbjAnwgNgS4'

Espero les haya servido este sencillo tutorial!