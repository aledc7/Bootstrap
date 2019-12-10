# Bootstrap
[![aledc.tk](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/aledc.com.svg)](https://aledc.tk)
[![License](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/mit-license.svg)](https://aledc.tk)
[![GitHub release](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/release.svg)](https://aledc.tk)
[![Dependencies](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/dependencias-none.svg)](https://aledc.tk)



# Ejemplos de Bootstrap y uso comun


Comencemos con el sitema de Grilla de Bootstrap, que divide la pantalla en 12 posiciones, entonces definimos como trabajar.

Primeramente se debe saber que siempre que vayamos a usar Bootstrap, debemos definir un contenedor, existen dos tipos:

Primer tipo:

__"container"__ :    Esta clase dejará margenes para todos los elementos que contenga

```php

# Todos los elementos dentro de este Row tendrán un margen tanto izquierdo como derecho   
<div class="container">
      <div class="row align-items-center">
        <div class="col-12 col-sm-6 col-md-4">
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Molestias
            culpa dolores cum magnam, vel pariatur consequatur qui et, possimus
            totam doloribus, reprehenderit sunt in accusamus doloremque aliquid
            voluptate. A, velit.
          </p>
        </div>

        <div class="col-12 col-sm-6 col-md-4">
          <p>Lorem ipsum dolor sit, amet consectetur</p>
        </div>

        <div class="col-12 col-sm-12 col-md-4">
          <p>Lorem ipsum dolor sit, amet consectetur</p>
        </div>
      </div>
    </div>
````

Segundo tipo:

__container-fluid__  :  A diferencia de la clase container, esta deja menos espacio a los costados.  



## Alineamieto 

Existe una clase para alinear los items de una fila (row), para que se alinean arriba, al centro o abajo, esta clase debe ir siempre junto con la clase row y estas son las tres clases:

__row align-items-start__   : Alineación en la parte superior del renglon.  

__row align-items-center__  : Alineación en la parte media del renglon.  

__row align-items-end__     : Alineación en la parte inferior del renglon.  











