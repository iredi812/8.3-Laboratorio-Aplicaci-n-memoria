Laboratorio Módulo 8.3 - Aplicación Memoria

Introducción

Queremos implementar el clásico juego de las parejas ¿En que consiste esto?

Mostramos al usuario 12 cartas boca abajo.
El usuario pincha en una carta y se ve el contenido de la misma (por ejemplo un gatito).
El usuario pincha en otra carta y se ve el contenido de la misma
Si por ejemplo es un perrito, ambas cartas se ocultan y vuelta a empezar.
Si es un gatito (y la carta origen era el mismo gatito), se quedan las dos cartas bocarriba y el usuario vuelve a jugar.
Esto así hasta que el usuario encuentre todas las parejas.


Prueba de concepto 1 - barajar las cartas

Vamos a tener un array de cartas y ¿Sabes que? Nos va a hacer falta barajar las cartas (si no cada partida sería igual), ¿Cómo hacemos esto?

Prueba de concepto 2 - Mostrar imagen y volver la carta

En esta prueba de concepto vamos a mostrar una carta, y cuando el usuario pinche en ella, la carta se va a volver y va a mostrar la imagen.

¿Cómo lo hacemos?

Vamos a crear un div con una imagen dentro en el HTML.
Vamos a escuchar al evento click del div.
Cuando el usuario pinche en el div, vamos a cambiar el src de la imagen.
Sólo una carta, es para desmotrarnos que sabemos resolver este desafío.


Prueba de concepto 3 - Mostrar un Grid de cartas

Ahora vamos a mostrar un grid de cartas, ¿Cómo lo hacemos?

En el HTML vamos a tener un div, contenedor, con 12 divs dentro.
Usamos CSS Grid para mostrar las cartas en una rejilla de 4x3.
Sólo queremos el grid, no queremos que las cartas se puedan voltear.


Prueba de concepto 4 - Mostrar segunda imagen y volver las dos cartas

Ahora vamos a mostrar dos cartas, y cuando el usuario pinche en la segunda, las dos cartas se van a voltear y van a mostrar la imagen.

¿Cómo lo hacemos?

Vamos a crear dos divs con una imagen dentro de cada uno en el HTML.
Vamos a escuchar al evento click de los divs.
Cuando el usuario pinche en el primer div, vamos a cambiar el src de la imagen.
Cuando el usuario pinche en el segundo div, vamos a cambiar el src de la imagen.
Sólo dos cartas, es para desmotrarnos que sabemos resolver este desafío.


Prueba de concepto 5 - Mapear el DIV que contiene la carta con la posición del array de las cartas

Lo que queremos hacer en esta prueba de concepto es mapear el div que contiene la carta con la posición del array de las cartas, es decir, si el usuario pincha en la primera carta, queremos saber que es la primera carta del array de cartas.

¿Cómo lo hacemos?

Vamos a crear un array de cartas.
El array va a tener 2 cartas de cada foto.
Vamos a crear un div por cada carta.
A cada div le vamos a poner un atributo
con el indice del array de cartas que le corresponde.
Vamos a escuchar al evento click de los divs.
Dentro de cada div vamos a tener una imagen, y vamos a cambiar el src de la imagen.
Para hacer esto dentro de cada imagen vamos a tener un atributo  que va a tener el mismo índice que el div que la contiene.
Cuando el usuario pinche en el primer div, vamos a leer el atributo data-indice-id y vamos a saber que es la primera carta del array de cartas y mostraremos la imagen correspondiente.

Apartados opcionales

Mostrar cuantos intentos lleva el usuario.
Mostrar una animación cuando el usuario pinche en una carta.
Mostrar un efecto hover cuando el usuario ponga el ratón sobre una carta.
Que si el usuario pincha en una carta ya volteada le salga un mensaje.
