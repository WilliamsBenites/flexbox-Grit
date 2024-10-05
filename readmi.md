# FLEXBOX

- Un modelo de layout que fue introducido por W3C
- Incorpora el concepto de cajas flexibles
- Todo flebox tiene 2 ejes (eje principal y eje secundario)
- Eje Principal (Main Axis) y Eje secundario (cross axis)
- Flexbox mantiene las casas flexibles va a tratar q todas las cajas esten en una fila, modificando el tamaño
- Flex items son

# TERMINOLOGIA 
-Flex Container
-Flex Item
-Main Axis
-Cross Axis
-Main Star
-Main End


## CSS  

-width: 500px;: El contenedor tendrá un ancho de 500 píxeles.
-height: 500px;: Tendrá una altura de 500 píxeles.
-border: 1px solid white;: Tendrá un borde blanco de 1 píxel.
-margin: 0 auto;: Esto centra el contenedor horizontalmente en la página.
-display: flex;: Activa el modelo de flexbox, que permite organizar los elementos dentro del contenedor de manera flexible.
-flex-wrap: wrap;: Si hay más elementos de los que caben en una fila, se "envuelven" a la siguiente fila.

# EJE PRINCIPAL (MAIN AXIS)
Inicia de (izquierda) y termina en (derecha)

- Justify-content : Propiedad que aplica al eje principal (MAIN AXIS) se aplica en el padre

- Es una propiedad que se utiliza en contenedores flexibles (flexbox) para alinear los elementos a lo largo del eje principal (que normalmente es horizontal).

- Valores : ||  space-between || space-around || space-evely || flex-star || flex-end || center ||

-flex-start: Alinea los elementos al inicio del contenedor (a la izquierda en un diseño de izquierda a derecha).

-flex-end: Alinea los elementos al final del contenedor (a la derecha).

-center: Centra los elementos en el medio del contenedor.

-space-between: Distribuye los elementos de manera que el primer elemento esté al principio, el último al final y el espacio entre los demás elementos sea igual.

-space-around: Distribuye los elementos dejando espacio igual alrededor de cada uno. Esto significa que habrá espacio extra a los lados de los elementos.

-space-evenly: Distribuye los elementos con espacio igual entre ellos y también en los bordes del contenedor.



## EJE SECUNDARIO (CROSS AXIS)
 Inicia de (arriba) y termina (abajo)
 - Align-items : Propiedd que aplica al eje secundario(CROSS AXIS)

 - Es una propiedad que se utiliza en contenedores flexibles (flexbox) para alinear los elementos a lo largo del eje transversal (que normalmente es vertical).

¿Dónde se aplica?
-Se aplica al contenedor padre y afecta a todos los elementos hijos dentro de él.

baseline: Alinea los elementos de acuerdo a la línea base del texto (la línea donde se sientan las letras).

stretch: (Valor predeterminado) Estira los elementos para que ocupen todo el espacio disponible en el contenedor a lo largo del eje transversal.


- Valores : flex-start || flex-end || center

--align-content:flex-star;--

- Esto puede ser confuso, pero align-content determina el espacio entre las líneas, mientras que align-items determina como los elementos en su conjunto están alineados dentro del contenedor. Cuando hay solo una línea, align-content no tiene efecto.
 
# CAMBIO EJE
 Esta propiedad CSS define la dirección de los elementos en el contenedor, y acepta los siguientes valores:

- flex-direction:valor:

-VALORES: 
- row: Elementos son colocados en la misma dirección del texto.
- row-reverse: Elementos son colocados en la dirección opuesta al texto.
- column: Elementos se colocan de arriba hacia abajo.
- column-reverse: Elementos se colocan de abajo hacia arriba.

## PROPIEDAD (ORDER)
A veces, invertir el orden de una fila o columna de un contenedor no es suficiente. En esos casos, nosotros podemos aplicar la propiedad ORDER a elementos individuales. Por defecto, los elementos tienen un valor 0, pero nosotros podemos usar esta propiedad para establecerlo a un número entero positivo o negativo.

```CSS
.yellow{
    order: 1
}
```

### FLEX-FLOW
-Las dos propiedades flex-direction y flex-wrap son usadas a menudo en conjunto con la propiedad abreviada flex-flow, la cual fue creada para combinarlas. Esta propiedad abreviada, acepta un valor de cada una separada por un espacio.

Por ejemplo, puedes usar flex-flow para establecer filas y envolverlas.
- flex-flow:column wrap

# GRID

- Grid container: contenedor o Elementos padre
- Grid items: elementos hijos
- Grid lines: Las lineas horizontales y verticales (5 lineas verticales/ 4 lineas horizontales)
- Grid tracks: las filas y columnas (3 trackas/ 4 tracks verticales)
- Grid area: cualquier rectangulo limitado por grid lineas ( si o si debe ser rectangulo)
- Grid celda: Cada rectangulo entre dos tracks (interseccion de tracks)