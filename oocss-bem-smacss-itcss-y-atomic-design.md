# 🎯 OOCSS, BEM, SMACSS, ITCSS y Atomic Design



Las Metodologías o Arquitecturas CSS nos ayudaran a escribir código CSS más predecible, reutilizable, mantenible y escalable.\
**CSS orientado a objetos (OOCSS)**\
CSS orientado a objetos (OOCSS) nos permite separar el contenedor y el contenido con “objetos” CSS

> Al igual que con cualquier método de codificación basado en objetos, el objetivo de OOCSS es fomentar la reutilización del código y, en última instancia, hojas de estilo más rápidas y eficientes que son más fáciles de agregar y mantener.

1. Estructura y piel separadas.
2. Contenedor separado y contenido

**Blocks, Elements and Modifiers (BEM)**\
BEM es una abreviatura de los elementos clave de la metodología: Bloque, Elemento y Modificador. BEM significa Modificador de Bloques de Elementos (Block Element Modifier) por sus siglas en inglés. Sugiere una manera estructurada de nombrar nuestras clases, basado en las propiedades del elemento en cuestión. Cuando utilizamos la metodología BEM, hay que tomar en cuenta que solamente podemos usar nombres de clases (no IDs). Los nombres de clases permiten repetir el nombre BEM si es necesario, y crear una estructura de código más consistente (en ambos archivos el HTML y CSS/Saas).

**Scalable and Modular Architecture for CSS (SMACSS)**\
En el núcleo de SMACSS (Arquitectura en CSS Escalable y Modular) está la categorización. Al clasificar las reglas CSS, comenzamos a ver patrones y podemos definir mejores prácticas en torno a cada uno de estos patrones.\
El objetivo principal de esta metodología es reducir la cantidad de código y simplificar el mantenimiento. Para ello, se dividen los estilos en cinco partes:

* **Reglas básicas**: se establecen los estilos por defectos de los elementos HTML individuales, los típicos selectores CSS de tipo. Por ejemplo

```
reset, html, body, button, h1
```

* **Reglas del layout:** se divide la página en secciones y se asignan los estilos relacionados con su estructura.

```
header, main content, footer, navigation
```

* **Reglas de módulos**: elementos que pueden ser reusables, modulares e independientes del contexto. Por ejemplo: llamadas a la acción o galerías de imágenes.
* **Reglas de estados:** se define el comportamiento del layout y sus módulos en diferentes estados: hover, active, diferentes resoluciones, etc.).
* **Reglas de temas**: estilos que afectan al layout y módulos. Estas reglas son opcionales, y las puedes utilizar para estilos que puede que quieras reemplazar.

**Scalable and Maintainable CSS Architecture — Xfive**\
ITCSS es una arquitectura que tiene como principal objetivo estructurar la forma en la que escribimos CSS.

* **Configuración** : se utiliza con preprocesadores y contiene fuentes, definiciones de colores, etc.
* **Herramientas** : mixins y funciones de uso global. Es importante no generar ningún CSS en las 2 primeras capas.
* **Genérico** : restablecer y / o normalizar estilos, definición de tamaño de caja, etc. Esta es la primera capa que genera CSS real.
* **Elementos** : estilo para elementos HTML desnudos (como H1, A, etc.). Estos vienen con un estilo predeterminado del navegador para que podamos redefinirlos aquí.
* **Objetos** : selectores basados ​​en clases que definen patrones de diseño no decorados, por ejemplo, objetos de medios conocidos de OOCSS
* **Componentes** : componentes específicos de la interfaz de usuario. Aquí es donde tiene lugar la mayor parte de nuestro trabajo y nuestros componentes de la interfaz de usuario a menudo están compuestos de objetos y componentes
* **Utilidades** : utilidades y clases auxiliares con la capacidad de anular cualquier cosa anterior al triángulo, por ejemplo. ocultar clase auxiliar

**Atomic Design**\
El diseño atómico es una metodología para crear sistemas de diseño. Hay cinco niveles distintos en el diseño atómico:

* Atomos: Los átomos son los componentes básicos de la materia. Aplicados a las interfaces web, los átomos son nuestras etiquetas HTML
* Moleculas: Las cosas comienzan a ponerse más interesantes y tangibles cuando comenzamos a combinar átomos juntos. Las moléculas son grupos de átomos unidos entre sí y son las unidades fundamentales más pequeñas de un compuesto
* Organismos: Las moléculas nos dan algunos bloques de construcción para trabajar, y ahora podemos combinarlas para formar organismos
* Plantillas: En la etapa de plantilla, rompemos nuestra analogía química para entrar en un lenguaje que tenga más sentido para nuestros clientes y nuestro resultado final
* Paginas: Las páginas son instancias específicas de plantillas. Aquí, el contenido del marcador de posición se reemplaza con contenido representativo real para dar una descripción precisa de lo que un usuario finalmente verá
