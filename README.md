


<p align="left">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/bootstrap-logo.png" width="300"
</p>    





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


> Primeramente se debe saber que siempre que vayamos a usar Bootstrap, debemos definir un contenedor, existen dos tipos:

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



## Alineamieto Horizontal con aling-items



<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/align_horizontal.png" width="700"
</p>

> Existe una clase para alinear los items de toda una fila para que se alinean arriba, al centro o abajo, esta clase debe ir siempre junto con la clase row y estas son sus tres variantes:

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

 
 > En caso de que necesitemos un alineamiento individual dentro de una misma celda, se deberá usar __align-self__ con las tres mismas variantes de __start, center y end__  y colocarse ya no en el row, sino dentro de la etiqueta de cada DIV que esté queriendo alinear.   
 
 
 > Aqui un ejemplo de una linea con 3 divs alineados de forma individual:
 
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

## Alineamiento Vertical

> La imágen de abajo muestra cinco filas con dos divs cada uno.  Cada renglon tiene un tipo de alineacion que afecta la alineación de cada div.

<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/align_vertical.png" width="700"
</p>
      

> Disponemos de las siguientes clases para alinear horizontalmente cualquier contenido:

__justify-content-start__  = alinea a la izquierda.  
__justify-content-center__ = alinea al centro de la fila.  
__justify-content-end__ = alinea a la derecha.  
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



## no-gutters


Esta clase elimina los pequeños espaciados que tienen los elementos naturalmente, debe usarse siempre con un __row__    

```php
<div class="row no-gutters">
      
</div>
`````

## Tipografias

 
> Clases para titulos y distintas tipografías:

__H1 al H6__   = Son los titulos similar a los tags de HTML pero con una fuente mas delicada.

__display-1  al display-4__ = Son titulos exageradamente GRANDES!

__lead__   = Esta clase es similar a una etiqueta __p__  solo apenas mas grande la fuente.


### Alineación de texto

> Las clases disponibles para parrafos son:

__text-left   
text-center   
text-right__  



## Bloque de texto con referencias

<blockquote class="blockquote">
  <p class="mb-0">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>
  <footer class="blockquote-footer">Someone famous in <cite title="Source Title">Source Title</cite></footer>
</blockquote>



## Listas list-inline

> Esta clase permite poner una lista una al lado de la otra, en lugar de una abajo de la otra.
> Puede ser útil para generar encabezados.  

```php
<ul class="list-inline">
  <li class="list-inline-item">Lorem ipsum</li>
  <li class="list-inline-item">Phasellus iaculis</li>
  <li class="list-inline-item">Nulla volutpat</li>
</ul>
````


## Lista list-unstyled  (sin estilo)

```php
<ul class="list-unstyled">
  <li>Lorem ipsum dolor sit amet</li>
  <li>Consectetur adipiscing elit</li>
  <li>Integer molestie lorem at massa</li>
  <li>Facilisis in pretium nisl aliquet</li>
  <li>Nulla volutpat aliquam velit
    <ul>
      <li>Phasellus iaculis neque</li>
      <li>Purus sodales ultricies</li>
      <li>Vestibulum laoreet porttitor sem</li>
      <li>Ac tristique libero volutpat at</li>
    </ul>
  </li>
  <li>Faucibus porta lacus fringilla vel</li>
  <li>Aenean sit amet erat nunc</li>
  <li>Eget porttitor lorem</li>
</ul>
            
````

## Colores de fuentes


<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/colores.png" width="350"
</p>
      

```php
<div class="container-fluid">
            <div class="row justify-content-center">
              <div class="col-2 borde0">
                  <p class="text-primary">.text-primary</p>
                  <p class="text-secondary">.text-secondary</p>
                  <p class="text-success">.text-success</p>
                  <p class="text-danger">.text-danger</p>
                  <p class="text-warning">.text-warning</p>
                  <p class="text-info">.text-info</p>
                  <p class="text-light bg-dark">.text-light</p>
                  <p class="text-dark">.text-dark</p>
                  <p class="text-body">.text-body</p>
                  <p class="text-muted">.text-muted</p>
                  <p class="text-white bg-dark">.text-white</p>
                  <p class="text-black-50">.text-black-50</p>
                  <p class="text-white-50 bg-dark">.text-white-50</p>
              </div>
            </div>
          </div>
````





## Fondos

<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/fondos.png" width="350"
</p>
      
      
      
```php
<div class="container-fluid">
  <div class="row justify-content-center">
    <div class="col-2 borde0">
        <div class="p-3 mb-2 bg-primary text-white">.bg-primary</div>
        <div class="p-3 mb-2 bg-secondary text-white">.bg-secondary</div>
        <div class="p-3 mb-2 bg-success text-white">.bg-success</div>
        <div class="p-3 mb-2 bg-danger text-white">.bg-danger</div>
        <div class="p-3 mb-2 bg-warning text-dark">.bg-warning</div>
        <div class="p-3 mb-2 bg-info text-white">.bg-info</div>
        <div class="p-3 mb-2 bg-light text-dark">.bg-light</div>
        <div class="p-3 mb-2 bg-dark text-white">.bg-dark</div>
        <div class="p-3 mb-2 bg-white text-dark">.bg-white</div>
        <div class="p-3 mb-2 bg-transparent text-dark">.bg-transparent</div>
    </div>
  </div>
</div>
````
 
 
 
 


## Margenes y Padding

> Para agregar margenes, se utuliza la letra __m__ mientras que para agregar paddin se utiliza la __p__   
> Luego esta letra __m__  o __p__  se combina con el sector al que se le quiera aplicar.   

t top   
b bottom   
l left  
r right   
x para todo el eje x   
y para todo el eje y   

> Finalmente se le agrega el numero de la unidad que se le quiera dar de margen, va desde el 0 al 5, e incuso auto .      
La medida que usa bootstrap es __rem__ ,  un rem equivale a 16px . 


### Ejemplo de Margenes:   

__mt-2__  = Margin Top 2rem (32px)   
__mb-1__  = Margin Bottom 1rem (16px)   
__ml-3__  = Margin Left 3rem (48px)   
__mr-4__  = Margin Right 4rem.     
__mx-5__ = Margen para todo el eje de las X, o sea, izquierda y derecha, de 5 rems.  
__my-3__ = Margen para todo el eje de las Y, o sea, arriba y abajo, de 3rem.

> También es posible combinar estos margenes con los puntos de ruptura de bootsrap, de manera que un margen se aplique unicamente a una determinada resolución: 

__sm__ = Small,        mayor o igual a 576px    
__md__ = Medium,       mayor o igual a 768px  
__lg__ = Large,        mayor o igual a 992px  
__xl__ = Extra large,  mayor o igual a 1200px

> Combinado entonces el margen, con el area, mas la resolución de pantalla, quedaría así:

__mt-sm-2__  = Margin Top 2rem (32px) solo se aplicara a una resolución mayor o igual a 576px     
__mb-md-1__  = Margin Bottom 1rem (16px) solo se aplicara a una resolución mayor o igual a 768px   
__ml-lg-3__  = Margin Left 3rem (48px) solo se aplicara a una resolución mayor o igual a 992px   
__mr-xl-4__  = Margin Right 4rem. solo se aplicara a una resolución mayor o igual a 1200px  
