# 🎯 Tipos de selectores: pseudoclases y pseudoelementos

también podemos ver a las pseudoclases como estados de algún elemento (con el mouse encima, visitado, activo, etc.) y a los pseudoelementos como elementos que escribimos desde CSS, por ejemplo, el `::after` y el `::before` nos puedes funcionar como divs, como su nombre lo dice, son elementos, pero no necesariamente están escritos desde el HTML 👀.\
.\
Gracias a las pseudoclases podemos cambiar los estilos de algún elemento cuando sucede algo, por ejemplo, cuando un botón está siendo clicado se activa el pseudoelemento `active`, entonces nosotros desde CSS podemos cambiar el color del botón a un color más oscuro para dar ese efecto de clicado 😄:\
.

```
button {
    color: #1a73e8;
}

button:active {
    color: #1557ad;
}
```

.\
Un dato curioso es que también podemos escribir colores usando código hexadecimal como en este caso 👀. Y ahora que ya sabes esto, ¡también podemos combinar pseudoelementos con pseudoclases! Por ejemplo, con el ejemplo de la profesora tenemos esto:\
.

```
p::before {
    content: "✨";
}
```

.\
Pero también podríamos agregarle un `:hover` y cambiar su contenido 👀👇:\
.

```
p::before {
    content: "✨";
}

p:hover::before {
    content: "💅";
}
```

¡Les reto a probarlo! Hay muchas cosillas más increíbles que se pueden hacer con CSS 😄.
