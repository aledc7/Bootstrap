# Bootstrap
[![aledc.tk](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/aledc.com.svg)](https://aledc.tk)
[![License](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/mit-license.svg)](https://aledc.tk)
[![GitHub release](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/release.svg)](https://aledc.tk)
[![Dependencies](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/dependencias-none.svg)](https://aledc.tk)



# Ejemplos de Bootstrap y uso común






Comencemos con el sitema de Grilla de Bootstrap, que divide la pantalla en 12 posiciones, entonces definimos como trabajar.

## Grip Option y sus puntos de quiebre

__col-__     = Extra small,  menor que 576px   
__col-sm-__  = Small,        mayor o igual a 576px  
__col-md-__  = Medium,       mayor o igual a 768px  
__col-lg-__  = Large,        mayor o igual a 992px  
__col-xl-__  = Extra large,  mayor o igual a 1200px  


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



## Alineamieto Vertical con aling-items

Existe una clase para alinear los items de toda una fila para que se alinean arriba, al centro o abajo, esta clase debe ir siempre junto con la clase row y estas son sus tres variantes:

__align-items-start__   : Alineación en la parte superior del renglon.  

__align-items-center__  : Alineación en la parte media del renglon.  

__align-items-end__     : Alineación en la parte inferior del renglon. 

Ejemplos de 3 rows, uno con cada alineamiento:

```php

# Row alineada en la parte superior
<div class="row align-items-start">
  <div class="col-12 col-sm-6 col-md-4 borde1">
    <p>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Molestias
      culpa dolores cum magnam, vel pariatur consequatur qui et, possimus
      totam doloribus, reprehenderit sunt in accusamus doloremque aliquid
      voluptate. A, velit.
    </p>
</div>

# Row alineada en la parte central
<div class="row align-items-center">
  <div class="col-12 col-sm-6 col-md-4 borde2">
    <p>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Molestias
      culpa dolores cum magnam, vel pariatur consequatur qui et, possimus
      totam doloribus, reprehenderit sunt in accusamus doloremque aliquid
      voluptate. A, velit.
    </p>
</div>


# Row alineada en la parte inferior
<div class="row align-items-end">
  <div class="col-12 col-sm-6 col-md-4 borde3">
    <p>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Molestias
      culpa dolores cum magnam, vel pariatur consequatur qui et, possimus
      totam doloribus, reprehenderit sunt in accusamus doloremque aliquid
      voluptate. A, velit.
    </p>
</div>

````

 
 En caso de que necesitemos un alineamiento individual dentro de una misma celda, se deberá usar __align-self__ con las tres mismas variantes de __start, center y end__  y colocarse ya no en el row, sino dentro de la etiqueta de cada DIV que esté queriendo alinear.   
 
 
 Aqui un ejemplo de una linea con 3 divs alineados de forma individual:
 
 ```php
 
 <div class="row">
        <div class="align-self-start">
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Molestias
            culpa dolores cum magnam, vel pariatur consequatur qui et, possimus
            totam doloribus, reprehenderit sunt in accusamus doloremque aliquid
            voluptate. A, velit.
          </p>
        </div>

        <div class="align-self-center">
          <p>Lorem ipsum dolor sit, amet consectetur</p>
        </div>

        <div class="align-self-end">
          <p>Lorem ipsum dolor sit, amet consectetur</p>
        </div>
      </div>
 ````

## Alineamiento Horizontal

Disponemos de las siguientes clases para alinear horizontalmente cualquier contenido:

__justify-content-start__  = alinea a la izquierda.  
__justify-content-center__ = alinea al centro de la fila.  
__ustify-content-end__ = alinea a la derecha.  
__justify-content-around__ = Deja espacio alrededor de los elementos.  
__justify-content-between__ =  divide los elementos y tira la mitad a la izquierda y la otra mitad a la derecha.  





```php
<div class="container">
          <div class="row justify-content-start">
            <div class="col-4 ">
              Una de dos columnas
            </div>
            <div class="col-4 ">
              Una de dos columnas
            </div>
          </div>
          <div class="row justify-content-center ">
            <div class="col-4 ">
              Una de dos columnas
            </div>
            <div class="col-4 ">
              Una de dos columnas
            </div>
          </div>
          <div class="row justify-content-end ">
            <div class="col-4 ">
              Una de dos columnas
            </div>
            <div class="col-4 ">
              Una de dos columnas
            </div>
          </div>
          <div class="row justify-content-around ">
            <div class="col-4 ">
              Una de dos columnas
            </div>
            <div class="col-4 ">
              Una de dos columnas
            </div>
          </div>
          <div class="row justify-content-between ">
            <div class="col-4 ">
              Una de dos columnas
            </div>
            <div class="col-4 ">
              Una de dos columnas
            </div>
          </div>
        </div>
 ````
 ddd
 
 
 
 
 











