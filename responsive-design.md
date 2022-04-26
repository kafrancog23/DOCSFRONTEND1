# 🎯 Responsive Design



### ¿Para qué es responsive design?

Es para que nuestro proyecto web pueda ser multiplataforma, que se pueda ver bien en un smartphone, desde una tablet, iPad y que se vean excelente desde una laptop o computadora de escritorio.

Esto realizándolo siempre con buenas prácticas.

Para empezar debemos saber:

### Media Queries

Con los media queries podemos jugar con el layout, cuando la pantalla del dispositivo sea pequeña el contenido se ve de una forma, pero si está pantalla crece el contenido también lo hace sin perjudicar el diseño.

Podemos cambiar la orientación de los contenedores, podemos cambiar su orden, incluso cambiar las dimensiones.

#### Breakpoint

Son la dimensión en el viewport, es decir el width y el height de la pantalla, en donde vamos a generar un cambio.

Este cambio es la forma en la que puedo reposicionar ciertos elementos o redimensionar ciertos contenedores, todo esto para que se vea bien la web app y sin importar el dispositivo en el que se abra.

#### min-width

Esto quiere decir que cuando la pantalla sea igual o más grande que el valor que coloquemos, el código que esté adentro del media querie se va a ejecutar.

Pero si la pantalla es mayor a ese min-width habrá otro media querie que aplicará estilos diferentes.

#### max-width

Esto quiere decir que cuando la pantalla sea igual o más pequeña que el valor que coloquemos, el código que esté adentro del media querie se va a ejecutar.

### La mejor forma de aplicar media queries

Tiene de nombre Mobile First o Mobile Only.

Esto quiere decir que el proyecto ya debe estar diseñado para dispositivos mobile, ya no debemos preocuparnos por que se vea bien desde una laptop o computadora de escritorio.

El diseño del proyecto va a partir desde un dispositivo mobile y desde ahí va a ir creciendo a los demás dispositivos con mayor pantalla.

Si hacemos lo contrario de ir de una pantalla grande a una más pequeña, esto se llama solamente responsive design y no es lo que estamos buscando.

#### Aplicado directo desde CSS con media queries

1. Arriba de los media queries vamos a tener el código base, que es el que está hecho y optimizado para dispositivos mobile.
2. Vamos a generar un breakpoint para realizar ciertos cambios en dispositivos más grandes.
3. Vamos a generar otro breakpoint que va a ser para una tablet o para computadoras con un viewport más pequeño como ser netbooks
4. Luego vamos a generar otro breakpoint que será para computadoras de escritorio, desktop o dispositivos con pantallas más grandes.

**Orden para aplicar los media queries**

Partimos desde los dispositivos más pequeños y terminamos con los dispositivos más grandes.

Si lo hacemos de forma inversa tendremos problemas, ya que como CSS funciona en cascada, nunca se van a aplicar los estilos de los medias queries con un viewport más grande.

Empezamos por:

1. Los celulares o dispositivos mobile.
2. Las tablets.
3. Laptops o computadores de escritorio.

#### Aplicado directo desde HTML (la mejor practica)

Este método se utiliza, ya que dependiendo del dispositivo donde esté el usuario va a necesitar un archivo CSS u otro, esto es para evitar que carguen archivos que el usuario no va a necesitar ni usar.

Lo agregamos en el `head`, aquí en vez de ligar un archivo de CSS vamos a ligar más de uno, dependiendo de los dispositivos en los que queramos aplicar los estilos.

**Estilos enfocados a mobile**

```html
<link rel="stylesheet" href="style.css">
```

**Si tenemos archivos CSS que van a impactar en otros dispositivos con diferente viewport**

```html
<link rel="stylesheet" href="tablet.css" media="screen and (min-width: 768px)">
<link rel="stylesheet" href="desktop.css" media="screen and (min-width: 1024px)">
```

Agregamos el atributo `media` cuyo valores va a ser el mínimo que necesitamos para hacer ese breakpoint, que es ese cambio en el layout.

**Orden final**

```html
<link rel="stylesheet" href="style.css"> <!-- Los dispositiivos mobiles -->
<link rel="stylesheet" href="tablet.css" media="screen and (min-width: 768px)">
<link rel="stylesheet" href="desktop.css" media="screen and (min-width: 1024px)">
```

### ¿Para qué es responsive design?

Es para que nuestro proyecto web pueda ser multiplataforma, que se pueda ver bien en un smartphone, desde una tablet, iPad y que se vean excelente desde una laptop o computadora de escritorio.

Esto realizándolo siempre con buenas prácticas.

Para empezar debemos saber:

### Media Queries

Con los media queries podemos jugar con el layout, cuando la pantalla del dispositivo sea pequeña el contenido se ve de una forma, pero si está pantalla crece el contenido también lo hace sin perjudicar el diseño.

Podemos cambiar la orientación de los contenedores, podemos cambiar su orden, incluso cambiar las dimensiones.

#### Breakpoint

Son la dimensión en el viewport, es decir el width y el height de la pantalla, en donde vamos a generar un cambio.

Este cambio es la forma en la que puedo reposicionar ciertos elementos o redimensionar ciertos contenedores, todo esto para que se vea bien la web app y sin importar el dispositivo en el que se abra.

#### min-width

Esto quiere decir que cuando la pantalla sea igual o más grande que el valor que coloquemos, el código que esté adentro del media querie se va a ejecutar.

Pero si la pantalla es mayor a ese min-width habrá otro media querie que aplicará estilos diferentes.

#### max-width

Esto quiere decir que cuando la pantalla sea igual o más pequeña que el valor que coloquemos, el código que esté adentro del media querie se va a ejecutar.

### La mejor forma de aplicar media queries

Tiene de nombre Mobile First o Mobile Only.

Esto quiere decir que el proyecto ya debe estar diseñado para dispositivos mobile, ya no debemos preocuparnos por que se vea bien desde una laptop o computadora de escritorio.

El diseño del proyecto va a partir desde un dispositivo mobile y desde ahí va a ir creciendo a los demás dispositivos con mayor pantalla.

Si hacemos lo contrario de ir de una pantalla grande a una más pequeña, esto se llama solamente responsive design y no es lo que estamos buscando.

#### Aplicado directo desde CSS con media queries

1. Arriba de los media queries vamos a tener el código base, que es el que está hecho y optimizado para dispositivos mobile.
2. Vamos a generar un breakpoint para realizar ciertos cambios en dispositivos más grandes.
3. Vamos a generar otro breakpoint que va a ser para una tablet o para computadoras con un viewport más pequeño como ser netbooks
4. Luego vamos a generar otro breakpoint que será para computadoras de escritorio, desktop o dispositivos con pantallas más grandes.

**Orden para aplicar los media queries**

Partimos desde los dispositivos más pequeños y terminamos con los dispositivos más grandes.

Si lo hacemos de forma inversa tendremos problemas, ya que como CSS funciona en cascada, nunca se van a aplicar los estilos de los medias queries con un viewport más grande.

Empezamos por:

1. Los celulares o dispositivos mobile.
2. Las tablets.
3. Laptops o computadores de escritorio.

#### Aplicado directo desde HTML (la mejor practica)

Este método se utiliza, ya que dependiendo del dispositivo donde esté el usuario va a necesitar un archivo CSS u otro, esto es para evitar que carguen archivos que el usuario no va a necesitar ni usar.

Lo agregamos en el `head`, aquí en vez de ligar un archivo de CSS vamos a ligar más de uno, dependiendo de los dispositivos en los que queramos aplicar los estilos.

**Estilos enfocados a mobile**

```html
<link rel="stylesheet" href="style.css">
```

**Si tenemos archivos CSS que van a impactar en otros dispositivos con diferente viewport**

```html
<link rel="stylesheet" href="tablet.css" media="screen and (min-width: 768px)">
<link rel="stylesheet" href="desktop.css" media="screen and (min-width: 1024px)">
```

Agregamos el atributo `media` cuyo valores va a ser el mínimo que necesitamos para hacer ese breakpoint, que es ese cambio en el layout.

**Orden final**

```html
<link rel="stylesheet" href="style.css"> <!-- Los dispositiivos mobiles -->
<link rel="stylesheet" href="tablet.css" media="screen and (min-width: 768px)">
<link rel="stylesheet" href="desktop.css" media="screen and (min-width: 1024px)">
```
