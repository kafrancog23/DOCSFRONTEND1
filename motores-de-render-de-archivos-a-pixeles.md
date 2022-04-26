# 🎯 Motores de render: de archivos a píxeles

Motores de renderizado

![Captura de pantalla 2021-09-30 152210.png](https://static.platzi.com/media/user\_upload/Captura%20de%20pantalla%202021-09-30%20152210-812f4f0c-28fe-4c13-9edf-85086007ca7d.jpg)

Cuando escribimos nuestros archivos HTML y CSS con ciertas etiquetas, selectores, atributos, propiedades, etc, todo eso el navegador no lo entiende y para poder entenderlo cada navegador tiene un motor que le permite entender y hacer visible en pixeles lo que nosotros hemos escrito.

### Navegadores y sus motores

Cada navegador tiene diferentes motores, pero realizan el mismo proceso.\
![Captura de pantalla 2021-09-30 152938.png](https://static.platzi.com/media/user\_upload/Captura%20de%20pantalla%202021-09-30%20152938-f2d67aa9-993b-40c7-b905-d0afa30a5446.jpg)\
Los 5 pasos de los motores:

1. Pasa los archivos de HTML a objetos (El DOM). Esto para que el navegador pueda entenderlo.
2. Calcula el estilo correspondiente a cada nodo en el DOM.
3. Calcula las dimensiones de cada nodo y va a empezar a estructurar la página web.
4. Pinta las diferentes cajas.
5. Toma las capas y las convierte en una imagen, para finalmente mostrar esta imagen en la pantalla.
