---
title: "Escribir en Markdown"
date: 2021-01-19T00:30:58-03:00
author: Luis Zambrana
draft: false
---


**Markdown** es una forma sencilla de agregar formato a textos en la web y funciona incorporando algunos caracteres a nuestro contenido. Es un texto plano, simple e intuitivo de escribir y fácil de leer en HTML.
Lo primero que tenemos que saber es que los archivos mardown tienen extensión **md** y se pueden leer con cualquier tipo de editor de texto. Al principio recomiendo usar la web [Dilinger](blank:#https://dillinger.io/) para practicar de manera online.

### Negrita
Debemos encerrar la palabra entre asterizcos doble (en cada lado):
Ejemplo:
Una palabra en **Negrita**
```
$ Una palabra en **Negrita**
```
### Titulos

Para escribir un titulo usamos el numeral antes de la oración. Entonces con 1 numeral tendremos el famoso h1, con 2 numerales el h2 y asi sucesivamente.

Ejemplo:

# Titulo h1
## Titulo h2
### Titulo h3
#### Titulo h4
##### Titulo h5
```
# Titulo h1
## Titulo h2
### Titulo h3
#### Titulo h4
##### Titulo h5
```

### Enlaces o Links

Los enlaces se pueden construir de dos maneras: 1) abandonando la página en la que se está navegando y yendo directamente al sitio al que deriva el enlace; 2) abriendo el sitio del enlace en otra pestaña, manteniendo la navegación en nuestro portal.

Ejemplo 1:

Este es un link hacia [mi blog personal](https://www.luiszambrana.com.ar/)

```
Este es un link hacia [mi blog personal](https://www.luiszambrana.com.ar/)
```

Este es un link hacia [mi blog personal](blank:#https://www.luiszambrana.com.ar/) que abre el enlace en otra pestaña nueva y permite mantener la navegación en mi sitio github.

```
Este es un link hacia [mi blog personal](blank:#https://www.luiszambrana.com.ar/) que abre el enlace en otra pestaña nueva y permite mantener la navegación en mi sitio github.

```
### Vincular Correos electronicos

 Este es un link a mi mail[soy@luiszambrana.com.ar](mailto:soy@luiszambrana.com.ar)

```
Este es un link a mi mail[soy@luiszambrana.com.ar](mailto:soy@luiszambrana.com.ar)
```

### Vincular numeros de telefono

Este es un link al teléfono [(54–11) 6496-4236](tel:+541164964236)
```
Este es un link al teléfono [(54–11) 6496-4236](tel:+541164964236)
```
Ahora podriamos hacer es que nuestro enlace del telefono nos lleve hacia algun sitio web:

Este es un link al teléfono [(54–11) 1164964236](blank:#https://api.whatsapp.com/send?phone=541164964236)


Esta opcion de tambien te permite agregar un mensajito preseateado, por ejemplo, si se usa para una mesa de ayuda y estoy en la pagina de soporte tecnico podria poner links que diga para tal cosa tal link y que el link me lleve a ese telefono correspondiente:

Este es un link al teléfono [(54–11)6496-4236](blank:#https://api.whatsapp.com/send?phone=5491164964236&text=¡Hola,%20necesito%20soporte!)

```
Este es un link al teléfono [(54–11)6496-4236](blank:#https://api.whatsapp.com/send?phone=5491164964236&text=¡Hola,%20necesito%20soporte!)

```

### Imagenes

Podemos utilizar una imagen que este dentro de nuestro proyecto.

```
![Hola Soy Luis](https://luisazambrana.github.io/puntolibre/images/profile.jpg)
```
y se veria asi:

![Hola Soy Luis](https://luisazambrana.github.io/puntolibre/images/profile.jpg)

Tambien podriamos agregarle un titulo alternativo a nuestra imagen de este modo:
```
![Texto alternativo](/ruta/a/la/imagen.jpg "Título alternativo")
```

### Insertar código

Conozco dos maneras, las mas comunes son:

`con un color`
```
`con un color`
```
Encerrando el texto en un recuadro como se viene haciendo en esta entrada:
```
Esto seria el codigo y se hace: poniendo 
\``` 
luego bajamos un espacio y luego cerramos el parrafo con 
\```
```
### Insertar un video de youtube
Aca te dejo un video:
[![BigBlueButton Sobre Docker](http://img.youtube.com/vi/lRIAQAmwnBY/0.jpg)](http://www.youtube.com/watch?v=lRIAQAmwnBY "BigBlueButton Sobre Docker")

y asi queda el codigo:

```
[![BigBlueButton Sobre Docker](http://img.youtube.com/vi/lRIAQAmwnBY/0.jpg)](http://www.youtube.com/watch?v=lRIAQAmwnBY "BigBlueButton Sobre Docker")

```

### Omitir Markdown

En el caso anterior que tuve que explicar la inserción de códigos, si o si tuve que evitar el reconocimiento de simbolos sino no podria haberlo mostrado.
Para hacer esto se utiliza una barra invertida:

\# Sin la barra hubiera sido un titulo h1

```
\# Sin la barra hubiera sido un titulo h1
```

Esto fue todo por hoy sobre **Markdown** y espero que les haya gustado!! Recuerden visitarme en mi [blog personal](blank:#https://luiszambrana.com.ar/) y si les gusta compartir en sus redes sociales.
