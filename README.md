#Instalación de Bootstrap
Para este trabajo de instalación del **framework Bootstrap**, he creado una web que servirá de base para una empresa que me ha pedido que le desarrolle una página web. La empresa se llama **Gastrokontu** y se dedica a dar servicio contable a sociedades gastronómicas, entidades con mucho arraigo en San Sebastián. 

Si bien la temática era libre, se podía haber usado este trabajo para adelantar el diseño de la web del TFM. No obstante, en mi casuística particular he decidido apostar por algo que podré reutilizar en breve.

Para ello, he utilizado una estructura básica para una web de una Pyme:
* Página principal.
* Sobre nosotros - Información sobre la empresa
* Servicios
* Consulta / Presupuesto

Como los textos aún no están elaborados, me valgo de texto falso Lore Ipsum para seguir las indicaciones de la actividad y del foro.

En primer lugar, he descargado la plantilla Carousel que es la que he utilizado como base en el proyecto.

## Ajustes de composición de página

### Menú

El primer ajuste de composición de página que he hecho ha sido el relativo al menú superior. Lo he fijado al borde superior del navegador. Para ello, lo que he hecho es añadir `navbar-fixed-top` al `class` de su `<nav>`.

### Rejilla

El segundo cambio significativo que he llevado a cabo en el Index es del modificar la rejilla, pasa de tener 3 elementos a tener 4. Esto lo he hecho modificando el `class`: en vez de `col-lg-4` he puesto `col-md-3`.

## estilos de bloques
### Imágenes del Index.
He cambiado la forma de las imágenes del Index. En un inicio eran circulares y ahora son cuadradas con los bordes redondeados.
### hr
En bootstrap.css he creado un estilo de clase que se llama `linea`. Este estilo tiene como objetivo que el `<footer>` se demarque mejor con respecto al resto de apartados de la página. Por ello, he añadido un `<hr>` con esta clase a los `<footer>`.

### Otros cambios
He intentado modificar el archivo CSS bootstrap-theme.css cambiando cosas, sin ningún exito. Por ejemplo, he intentado modificar `btn-primary` para cambiar el color de todos los botones, y aún cambiando los `background-color` necesarios, no he conseguido ningún cambio visual.
Lo mismo me ha ocurrido con los `<h1>`, `<h2>`, etc. He intentado cambiarlos de color, pero no ha surtido ningún efecto. También he intentado que `<li>` tuviese un estilo `square` pero ha sido imposible. He probado a cambiar los estilos de `<ul>` y de `<li>`, incluso he creado una clase propia que he asignado en HTML. Aun así, ha sido imposible.
Me sorprende porque las páginas sí me responden a nuevos estilos como `linea`. Creo que los estilos de bootstrap.css entran en conflicto, de algún modo, con los de bootstrap-theme.css y por eso los cambios no surten efecto, porque HTML lee los de este último.

## 5 estilos de javascript
En el desarollo del proyecto he añadido las siguientes funciones JavaScript que permite Bootstrap. Tres de ellas las he usado en el formulario de la página presupuestos.html, dado que considero que da juego para ello.

### Tooltip

En la página presupuesto.html he creado un formulario en el que he utilizado la función Tooltip de JavaScript. De esta manera, cada vez que alguien posicione el cursor sobre el campo a rellenar le aparecerá un mensaje emergente con información.

### Botón formulario

En la misma página, en vez de usar la clásica opción de menú desplegable para seleccionar si quiero hacer una pregunta o pedir un presupuesto deberé seleccionar uno de los dos botones.

### Modal
A la hora de pulsar el botón enviar, emergerá una ventana informando sobre la utilización que se dará de la información recogida en el formulario en función de la Ley Orgánica de Protección de Datos.

### Toggable tab
He utilizado Toggable tab en nosotros.html. Creo que este sistema de pestañas de JS es muy adecuado si se quiere mostrar información variada pero no muy extensa en la misma página.

### Collapse
En servicios.html he usado Collapse. Es una buena manera de mostrar un listado de servicios y con el efecto acordeón solo desplegar el que te interese.
