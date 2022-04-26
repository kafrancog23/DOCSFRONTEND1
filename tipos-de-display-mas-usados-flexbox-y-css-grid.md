# 🎯 Tipos de display más usados: flexbox y CSS grid

#### ¿Y es mejor Flexbox o CSS Grid? 🤔

Si te hiciste esta pregunta vamos a aclarar algunas cosas 👀👇:\
.\
En general, en cualquier ámbito del desarrollo web no suele haber una tecnología mejor que otra, y este es el caso de Flexbox y CSS Grid. Ninguna es mejor que otra, de hecho, ¡ambas se complementan! No es como que tengas que elegir sí o sí una, es completamente posible usar ambas al mismo tiempo 👀.\
.\
Por ejemplo, algo que a mí me gusta hacer es usar Flexbox para estilizar elementos pequeños, tipo tarjetitas y así, y después a CSS Grid lo uso para estructurar toda mi página entera OwO. Este es mi modo de trabajar, pero incluso podrías hacerlo al revés, es decir, usar CSS Grid para cositas pequeñas y Flexbox para armar todo tu layout, ¡CSS es muy flexible!\
.\
Estos dos displays son temas muy interesantes y profundos, aquí te dejo una probadita de lo que se puede hacer con Flexblox 7u7 👇:\
.

#### Flexbox

Flexbox es magia, con Flexbox podemos literal manipular los elementos a como queramos. ¿Alguna vez has visto el meme de “programadores sufriendo por centrar un div”? Pues Flexbox rompe ese meme de manera épica 😎.\
.\
Con Flexbox podemos alinear los elementos a como queramos, así lo queramos a la izquierda, en el centro o a la derecha, tanto vertical como horizontalmente, por ejemplo, lo más común, centrar un elemento:\
.

```
<div class="container">
    <p>OwO</p>
</div>
```

.\
¡Podemos centrar el texto usando Flexbox!\
.

```
.container {
    display: flex;
    justify-content: center;
    background: papayawhip;
}
```

.\
Y con esto obtendríamos lo siguiente 👇\
.\
![flexbox.png](https://static.platzi.com/media/user\_upload/flexbox-b8190ef2-948b-4e18-a9cc-6de8f57f8599.jpg)\
.\
En este caso lo hice con un texto… ¡Pero funciona con cualquier elemento! OwO. Otro caso de uso por ejemplo, es cuando queremos hacer un header y queremos que el logo este a la izquierda y que el menú de navegación esté a la derecha. Hacer esto con Flexbox es pan comido 😎👇:\
.

```
<header>
    <picture class="header-child">Soy un logo UwU</picture>
    <nav  class="header-child">Soy un menú de navegación 7w7</nav>
</header>
```

.\
En este caso, tenemos dos elementos dentro de nuestro `<header>`, el logo debería estar del lado izquierdo, y el menú de navegación del lado derecho, ¿verdad? Bueno, es tan fácil como hacer esto:\
.

```
header {
    display: flex;
    justify-content: space-between;
    background: papayawhip;
}
```

.\
¡Y con eso tendríamos suficiente!\
.\
![header.png](https://static.platzi.com/media/user\_upload/header-d6983b07-9f81-438e-b6c7-7f09c7d23d4c.jpg)\
.\
Obviamente podemos darle más estilos para que se vea más vistoso UwU:\
.

```
header {
    display: flex;
    justify-content: space-between;
    background: papayawhip;
    padding: 15px;
}

.header-child {
    background: #ff9696;
    padding: 5px;
}
```

.\
![header2.png](https://static.platzi.com/media/user\_upload/header2-da6f74e2-c37d-43d8-8262-450cb6755908.jpg)\
.\
¡Y esto funciona en cualquier tamaño de pantalla!\
.\
![header3.png](https://static.platzi.com/media/user\_upload/header3-868aafdb-8fce-470d-a35b-2b3f4044052e.jpg)\
.\
Aquí únicamente hemos usado Flexbox, ahora imagínate lo que podemos hacer con CSS Grid 😏…
