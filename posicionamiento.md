# 🎯 Posicionamiento

## Static

Utilizamos este valor no vamos a tener ningún cambio porque todas las etiquetas vienen con este valor.

Cuando estamos en este position no podemos utilizar las propiedades left, top, right y bottom.

### Absolute

Con absolute el elemento sale de su lugar y el navegador reacomoda los elemento, poniendo otro elemento en el lugar del elemento con position absolute. Podemos posicionar al elemento como queramos.

### Relative

Con relative no sucede lo mismo que absolute, el elemento mantiene su lugar, pero podemos posicionarlo donde queramos.

Lo podemos usar como contenedor para que los elementos que tengan un position absolute tomen como referencia al padre que nosotros queremos (se adhiere al elemento relativo más cercano) y no a otro, delimita el movimiento del hijo.

### Fixed

Este valor de position nos permite que el elemento que queramos nos siga a todos lados desde el momento en el que nos topemos con él.

### Sticky

Es similar a fixed con la diferencia que cuando encuentra a otro elemento con su mismo position, sticky, le da lugar al ese elemento.

### Initial

Vuelve el position de un elemento a como estaba originalmente.

### Inherit

Lo usamos si queremos que nuestro elemento herede el position de su padre.

### Left, top, right y bottom

Con estas cuatro propiedades podemos mover a los elementos que tengan como position a absolute, relative fixed o sticky a los lugares que queramos.\
\
El tema de `position` es muy interesante porque es prácticamente otra forma que tenemos de posicionar con CSS 👀.\
.\
Usualmente es preferible trabajar con nuestras técnicas de alineamiento comunes como CSS Grid o Flexbox, pero suele haber casos donde sí o sí necesitamos usar `position`.\
.\
El ejemplo más común es con el menú de navegación, que casi siempre solemos verlo en todas las páginas. Aunque también podríamos usarlos si queremos posicionar un elemento con base en otro (aquí es donde intervienen el `relative` con el `absolute`), y de hecho esta también es una técnica muy usada cuando se dibuja con CSS 7u7.\
.\
¡Hagamos algo! Imaginemos que queremos darle su bola de estambre a este michi 😼:\
.\
**Bola de estambre**\
.\
![estambre.png](https://static.platzi.com/media/user\_upload/estambre-41afab11-199b-4105-82be-58c50e4800d8.jpg)\
.\
**Michi**\
.\
![michi.jpg](https://static.platzi.com/media/user\_upload/michi-0cd46b59-feda-4746-81a0-cc48179411ae.jpg)\
.\
Lo primero que haría es crear un contenedor y dentro meter al michi y a la bola de estambre (las imágenes las toma desde internet):\
.

```
<div class="container">

    <img id="estambre" src="https://pixabay.com/get/gcace262ba99b669194b5054d0a18589d64d2858de5ccde802a2bd69112122969cc55406c4d138c9738ad55e21d831bab_640.png" alt="Estambre">

    <img id="michi" src="https://static.platzi.com/media/user_upload/michi-0cd46b59-feda-4746-81a0-cc48179411ae.jpg" alt="Michi">
    
</div>
```

.\
Nota que a cada uno le puse un id. También me interesa que mi bola de estambre esté chiquita para que el michi la pueda agarrar, así que desde CSS le puedo cambiar el tamaño:\
.

```
.container,
#michi {
    width: 800px;
}
#estambre {
    width: 100px;
}
```

.\
Con esto hago que mi contenedor y el michi midan 800px y que la bolita de estambre mida 100px, así que me queda así:\
.\
![michi-estambre.png](https://static.platzi.com/media/user\_upload/michi-estambre-46ff8042-0f01-4272-a408-587c835e2708.jpg)\
.\
Ahora solo nos queda dársela, para eso podemos usar `position`. Simplemente a mi container le pongo un `position: relative;` y al estambre le pongo un `position: absolute;`. Recuerda que cuando usamos un `absolute`, este elemento se va a mover con respecto al elemento `relative` más cercano, así que en este caso moveremos el estambre con respecto a nuestro contenedor 😄.\
.\
Sabiendo que podemos mover el estambre dentro de nuestro container, nos tocará adivinar cuántos pixeles hacia abajo y cuántos pixeles hacia la izquierda deberemos moverlo para dárselo al michi 👀. En este caso, yo sé que debo moverlo 190 pixeles hacia abajo y 245 pixeles hacia la izquierda, por lo que el resto de mi código CSS quedaría así:\
.

```
.container {
    position: relative;
}

#estambre {
    position: absolute;
    top: 190px;
    right: 245px;
}
```

.\
¡Y con esto el michi ya tendría su estambre!\
.\
![michi-con-estambre.png](https://static.platzi.com/media/user\_upload/michi-con-estambre-75054364-51d5-4167-85c0-1ed3da43cad5.jpg)\
.\
Este es un ejemplo de cómo podemos usar `position` para posicionar un elemento con respecto a otro, pero realmente hay varios usos que podemos darle, así que te toca practicar 😼.\
\
