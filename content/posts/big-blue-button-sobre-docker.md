---
title: "Big Blue Button Sobre Docker"
date: 2021-01-19T23:43:05-03:00
author: Luis Zambrana
draft: false
---
Dar clases online es todo un tema y más aun cuando requerimos compartir contenidos, cuando hablamos de seguridad de los datos etc etc. A sabiendas que hay una resolución nueva en argentina donde se establece el **Plan Básico Universal y Obligatorio** para Internet, Tv, Comunicación celular etc y que en la misma se ve que **la navegacion de los servicios bajo dominios .gob.ar .edu.ar son gratuitos** para los usuarios que ingresan a sus webs etc es un buen momento para montar una sala de conferencias como Big Blue Button. Entre muchas de pago si optas por algo libre y no digo gratuito por que requiere pago de hosting etc que veremos luego, si Buscas un software de código abierto para dar clases Big Blue Button es la opción.

Como les decia anteriormente los servicios bajo dominios .edu.ar y gob.ar seran gratuitos para el Plan Basico Universal y Obligatorio.

##Para ver más info del Plan Básico Universal y Obligatorio de comunciaciónes:
- [Prestación en Argentina.gob.ar](blank:#https://www.argentina.gob.ar/noticias/plan-basico-universal-obligatorio-para-celulares-internet-tv-paga-y-telefonia-fija-desde)

- [Prestacipon en enacom.gob.ar](blank:#https://www.enacom.gob.ar/prestacion-basica-universal_p4792)

Se me ocurrió probar **BigBlueButton** en casa, sobre mi propia notebook y quede chocho por que si bien no conocia algunas cuestiones fueron bastante intuitivas.

![BigBluegButton]((/images/bigbluebutton.jpeg) "BigBluegButton")

La instalacion de **BigBlueButton** la vamos a realizar sobre **Docker** por lo que recomiendo que lo tengas instalado (en mi caso lo hice sobre ubuntu 20.04) y que conozcas algunas cuestiones de docker.

```
git clone --recurse-submodules https://github.com/LuisAZambrana/bigbluebutton-docker.git bbb-docker

```
Ingresamos a la carpeta que recien creamos

```
cd bbb-docker

```
Ejecutamos el script que va a hacer le trabajo por nosotros

```
./scripts/setup

```
Inciamos los contenedores

```
./scripts/compose up -d

```

Luego que ya esten andando los contenedores en otra terminal vamos a crear el usuario administrador para que peudas manejar las salas de **BigBlueButton**

```
./scripts/compose exec greenlight bundle exec rake admin:create

```
Espero que les haya gustado y hayan logrado seguir este paso a paso que si bien es larguito el script ayuda a que no haga un monton de cosas que llevarían muchisimo mas tiempo. Les dejo un video sencillo que subi a youtube para darles un ejemplo de lo que se logra:

[![BigBlueButton Sobre Docker](http://img.youtube.com/vi/lRIAQAmwnBY/0.jpg)](http://www.youtube.com/watch?v=lRIAQAmwnBY "BigBlueButton Sobre Docker")