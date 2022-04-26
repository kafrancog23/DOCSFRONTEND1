# 🎯 Tipos de selectores: básicos y combinadores



#### Selectores combinadores

Ahora que ya entendemos los selectores básicos, vienen los combinadores, que realmente nos ayudan a ser muchos más específicos 👀.\
.

1. **Descendientes:** En este selector, el que está más a la izquierda es el selector padre y los que están a su derecha serán los selectores hijos, por ejemplo:\
   .\
   ![carbon (8).png](https://static.platzi.com/media/user\_upload/carbon%20\(8\)-2f40be2f-b500-45ba-b640-0fa77a19e6d9.jpg)\
   .\
   En este selector, el `div` es el padre y el `.rojito` es el hijo. ¿Esto qué significa? Básicamente que este selector va a agarrar cualquier elemento que tenga la clase “rojito”, pero este elemento **tiene que estar DENTRO de un div**. O sea, si encuentra algún elemento que tenga la clase `.rojito`, pero este elemento NO está dentro de un `div`, pues ese elemento NO lo va a agarrar 😄.\
   .\
   ![carbon (9).png](https://static.platzi.com/media/user\_upload/carbon%20\(9\)-581bad9f-d5c9-49d2-8f43-5d412accaa46.jpg)
2. **Hijo directo**: Este caso es similar al anterior, pero ahora solo agarrará a los hijos que este directamente adentro del padre. Recuerda que en el elemento padre nosotros podemos tener más cajitas con más elementos dentro, en este caso, este selector NO agarrará a esos otros elementos, por ejemplo:\
   .\
   ![carbon (11).png](https://static.platzi.com/media/user\_upload/carbon%20\(11\)-5e9b9bbe-64e9-4210-9c64-de62874fc8c4.jpg)\
   .\
   Al poner el signo `>` estoy especificando que quiero seleccionar a cualquier elemento que tenga la clase `.rojito`, pero este elemento tiene que estar directamente dentro de un `<div>`.\
   .\
   ![carbon (12).png](https://static.platzi.com/media/user\_upload/carbon%20\(12\)-bb3cebd4-4d9b-4c1b-86be-2b09e4b9bfb4.jpg)\
   .\
   En este ejemplo el `<span>` que está dentro del `<section>` NO sería seleccionado porque, aunque está dentro del `<div>` NO está directamente dentro del `<div>` 😄.
3. **Elemento adyacente**: Básicamente selecciona a la etiqueta que esté debajo de la primera etiqueta 👀.\
   .\
   ![carbon (13).png](https://static.platzi.com/media/user\_upload/carbon%20\(13\)-b686df82-3b46-42dd-bc17-c9375796fe50.jpg) ![carbon (14).png](https://static.platzi.com/media/user\_upload/carbon%20\(14\)-91dc5df7-44b3-4bce-b1a7-860696b3c6ce.jpg)\
   .
4. **General de hermanos**: Es similar al adyacente, pero esta vez no solo selecciona al de abajo, sino a cualquiera que esté al mismo nivel que el selector original, es decir, a sus hermanos :3\
   .\
   ¡Y podemos combinar más selectores! OwO. Por ejemplo:\
   .\
   Puedo seleccionar a todas las etiquetas `<p>` que estén **directamente adentro** de cualquier elemento con la clase `azulitos` y que a su vez, estos elementos sean hermanos de algún elemento con la clase `.rojito` y que este elemento con la clase `.rojito` esté dentro de un `<div>` OwO:\
   .\
   ![carbon (15).png](https://static.platzi.com/media/user\_upload/carbon%20\(15\)-1c6c80d5-7927-4e58-8345-0c62c80a6aca.jpg)\
   .\
   Este es un selector MUY específico, y podemos ser aún más específicos, pero quiero que veas como podemos empezar a combinar selectores, y muchas veces es más fácil leer estos selectores de derecha a izquierda 😄.\
   .\
   Este puede ser un tema un poco complicado, ¡no te desanimes! Recuerda los consejos, para a practicar un rato, experimenta, curiosea, repite la clase si es necesario, pero hazlo hasta que lo consigas
