# Flexbox

Flexbox es un sistema de elementos flexibles personaliza ble, en la que los elementos se adaptan y es más fácil personalizar los diseños. Diseñado para crear estructuras de una sola dimensión.

Conceptos básicos 


![](https://paper-attachments.dropbox.com/s_3EB164AEBE23197C4F8586483D72E967BACFEA471F935A2A9F1D6620D4C73D53_1577667372026_flexbox-como-funciona.png)



- Contenedor: Existe un elemento padre que es el contenedor que tendrá en su interior cada uno de los ítems flexibles y adaptables.


- Eje principal: Los contenedores flexibles tendrán una orientación principal. Por defecto, es en horizontal (fila).


- Eje secundario: De la misma forma, los contenedores flexibles tendrán una orientación secundaria, perpendicular a la principal. Si la principal es en horizontal, la secundaria será en vertical, y viceversa.
- 
- Ítem: Cada uno de los hijos flexibles que tendrá el contenedor en su interior.

Los ejes principal y secundario, pues existirá un inicio y un fin para cada uno de los ejes.

![](https://paper-attachments.dropbox.com/s_3EB164AEBE23197C4F8586483D72E967BACFEA471F935A2A9F1D6620D4C73D53_1577668579917_4173.png)

Display flex

Al contenedor principal en un esquema Flexbox es al que le asignamos "display: flex". Esta propiedad hace que cambien las reglas con las cuales sus hijos van a ser representados en la página.


    .flex-container {
      display: flex;
    }


Display inline-flex: 

No se expanden para ocupar todo el espacio en la horizontal.


Propiedad flex-direction

Esta propiedad nos sirve para definir la dirección del flujo de colocación de los elementos.


- row (valor predeterminado): Indica que los elementos se colocan en una fila, uno al lado del otro, de izquierda a derecha.
- row-reverse: se colocan en una fila, pero con orden de derecha a izquierda.
- column: se colocan uno debajo del otro, en orden los primeros arriba.
- column-reverse: se colocan en una columna, pero los primeros aparecerán abajo.


Propiedad flex-wrap

Sirve para indicar si queremos que haya saltos de línea en los elementos que se colocan en el contenedor


- nowrap (predeterminado): hace que nunca se produzcan saltos de línea.
- wrap: hace que si no caben, entonces se coloquen en la siguiente línea.
- wrap-reverse: El salto de línea se producirá al contrario, o sea, hacia arriba.


Propiedad flex-flow

Esta propiedad no aporta nada nuevo, pues simplemente es un atajo para escribir de 1 sola vez flex-direction y flex-wrap. El valor predeterminado es "row nowrap”


    .flex-container {
      display: flex;
      flex-flow: row wrap;
    }


Propiedad justify-content

Esta propiedad es muy útil para indicar cómo se van a colocar los justificados y márgenes de los ítems.


![](https://paper-attachments.dropbox.com/s_3EB164AEBE23197C4F8586483D72E967BACFEA471F935A2A9F1D6620D4C73D53_1577672281915_4191.png)



Propiedad align-items

Esta propiedad es muy similar a la propiedad anterior, justify-content, solo que ahora estamos alineando con respecto al eje secundario y no el principal.


![](https://paper-attachments.dropbox.com/s_3EB164AEBE23197C4F8586483D72E967BACFEA471F935A2A9F1D6620D4C73D53_1577672419208_4192.png)



Propiedad align-content

Esta propiedad sólo aplica cuando dispones de varias líneas de elementos en el contenedor flexbox. El efecto que conseguiremos será una alineación y separación de las filas en el eje secundario.


Items Flexbox


Propiedad flex-grow

La propiedad flex-grow sirve para decir cómo deben crecer los elementos incluidos en el contenedor.


![](https://paper-attachments.dropbox.com/s_3EB164AEBE23197C4F8586483D72E967BACFEA471F935A2A9F1D6620D4C73D53_1577675183732_image.png)

