# 🎯 Modelo de caja



El modelo de caja también podemos verlo como los ogros… ¡Capas! ¡Los ogros tiene capas!\
.\
![shrek1.jpg](https://static.platzi.com/media/user\_upload/shrek1-c1e4604f-23b3-4fab-b844-8e16e2986bbe.jpg)\
.\
Esto es un tema muy mindblow 🤯. Básicamente porque todo en HTML son cajitas, sí, incluso un texto es una caja. Cuando tú insertas un texto, lo que estás haciendo es que estás insertando una cajita que adentro tiene texto (y lo mismo aplica para cualquier etiqueta). Esta cajita tiene un fondo transparente, pero si tú le pones cualquier fondo usando la propiedad `background` podrás ver esa cajita. Esta cajita, además de su contenido, tiene estas 3 capas externas que serían el padding, el border y el margin 👇:\
.

* **`padding`**: Es básicamente el espaciado que hay entre la caja y el contenido de la caja, es un espaciado interno. Lo solemos usar mucho para permitir que los elementos “respiren”, por ejemplo, aquí les dejo una comparación de un botón **sin** padding y **uno** con padding 👇\
  .\
  ![padding.png](https://static.platzi.com/media/user\_upload/padding-46ae4565-4049-482e-9a24-a7e21040468a.jpg)\
  .
* **`border`**: Es el delineado que le podemos dar a una caja, y un borde puede ser tan grueso como quieras. Simplemente debemos ponerle el grosor, el tipo de borde y el color del borde, por ejemplo, podemos hacer una caja con bordes y líneas intermitentes OwO:\
  .

```
<div class="box">
    <p>Arrastra una imagen</p>
</div>
```

.

```
.box {

    border: 4px dashed dodgerblue;

    display: flex;
    justify-content: center;
    align-items: center;
    ;

    width: 500px;
    height: 200px;
    color: dodgerblue;
    font-weight: bold;

}
```

.\
![box.png](https://static.platzi.com/media/user\_upload/box-b34571e7-c884-47d8-af3e-b5743441c6c9.jpg)\
.\
Nota como en este caso lo combiné incluso con Flexblox 7u7.\
.

* **`margin`**: Este es básicamente el espaciado entre elementos. Es la distancia que podemos dejar de un elemento hacia otro.\
  .\
  Con estas capitas podemos conformar el modelo de caja 😄.

.\
Y para resumir la propiedad **`box-sizing: border-box;`** es sencilla: si pones esta propiedad, ekl tamaño final de tu caja va a ser del `width` que tú le pongas, si no la pones, eol tamaño final de tui caja va a ser del `width` que tú le pongas más el tamaño de tu padding, más el de tu borde má el de tu margin UwU.\
.\
Y de ahora en adelante cuando empieces a desarrollar, notarás que muchos usan esto en CSS 👇:\
.

```
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
```
