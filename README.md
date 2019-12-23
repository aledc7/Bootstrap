


<p align="left">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/bootstrap-logo.png" width="300"
</p>    





[![aledc.tk](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/aledc.com.svg)](https://aledc.tk)
[![License](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/mit-license.svg)](https://aledc.tk)
[![GitHub release](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/release.svg)](https://aledc.tk)
[![Dependencies](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/dependencias-none.svg)](https://aledc.tk)



# Ejemplos de Bootstrap y uso común

Este repositorio agrupa la mayoría de los elementos de bootstrap.  
Si bien esta misma info se encuentra disponible en la documentacion oficial, aqui está toda en una sola página, lo cual resulta útil para una rápida referencia y uso, ya que cada ejemplo tiene el código.







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
__mx-5__  = Margen para todo el eje de las X, o sea, izquierda y derecha, de 5 rems.  
__my-3__  = Margen para todo el eje de las Y, o sea, arriba y abajo, de 3rem.
__m-3__  =  Al poner solo la m sin indicador del area, el margen será hacia los 4 lados

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

Tambien existe la posibilidad de asignar  __mx-auto__  o __my-auto__  para no asignar un valor,  pero en estos casos es requisito asignarle un style="width: 100px;"  
```php
<p class="mx-auto" style="width: 200px;"> texto</p>
````



### Ejemplo de Padding:

la lógica de los Paddings es exactamente la misma que la de margenes, solo se reemplaza la letra __m__ por la letra __p__  



__pt-2__  = Padding Top 2rem (32px)   
__pb-1__  = Padding Bottom 1rem (16px)   
__pl-3__  = Padding Left 3rem (48px)   
__pr-4__  = Padding Right 4rem.     
__px-5__  = Padding para todo el eje de las X, o sea, izquierda y derecha, de 5 rems.  
__py-3__  = Padding para todo el eje de las Y, o sea, arriba y abajo, de 3rem.
__p-3__  =  Al poner solo la m sin indicador del area, el padding será hacia los 4 lados


> También es posible combinar estos Paddings con los puntos de ruptura de bootsrap, de manera que un margen se aplique unicamente a una determinada resolución: 

__sm__ = Small,        mayor o igual a 576px    
__md__ = Medium,       mayor o igual a 768px  
__lg__ = Large,        mayor o igual a 992px  
__xl__ = Extra large,  mayor o igual a 1200px

> Combinado entonces el Padding, con el area, mas la resolución de pantalla, quedaría así:

__pt-sm-2__  = Padding Top 2rem (32px) solo se aplicara a una resolución mayor o igual a 576px     
__pb-md-1__  = Padding Bottom 1rem (16px) solo se aplicara a una resolución mayor o igual a 768px   
__pl-lg-3__  = Padding Left 3rem (48px) solo se aplicara a una resolución mayor o igual a 992px   
__pr-xl-4__  = Padding Right 4rem. solo se aplicara a una resolución mayor o igual a 1200px  



### Alertas


Creando divs de alertas

<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/1.png" width="1024"
</p>



```php
<!-- Alertas -->

    <div class="my-4"></div>

    <div class="container">
      <div class="col-12">
        <div class="alert alert-primary" role="alert">
          A simple primary alert—check it out!
        </div>
        <div class="alert alert-secondary" role="alert">
          A simple secondary alert—check it out!
        </div>
        <div class="alert alert-success" role="alert">
          A simple success alert—check it out!
        </div>
        <div class="alert alert-danger" role="alert">
          A simple danger alert—check it out!
        </div>
        <div class="alert alert-warning" role="alert">
          A simple warning alert—check it out!
        </div>
        <div class="alert alert-info" role="alert">
          A simple info alert—check it out!
        </div>
        <div class="alert alert-light" role="alert">
          A simple light alert—check it out!
        </div>
        <div class="alert alert-dark" role="alert">
          A simple dark alert—check it out!
        </div>
      </div>
    </div>

    <div class="my-4"></div>

```

<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/2.png" width="1024"
</p>

```php


    <div class="container">
      <div class="col-12">
        <div class="alert alert-primary" role="alert">
          A simple primary alert with
          <a href="#" class="alert-link">an example link</a>. Give it a click if
          you like.
        </div>
        <div class="alert alert-secondary" role="alert">
          A simple secondary alert with
          <a href="#" class="alert-link">an example link</a>. Give it a click if
          you like.
        </div>
        <div class="alert alert-success" role="alert">
          A simple success alert with
          <a href="#" class="alert-link">an example link</a>. Give it a click if
          you like.
        </div>
        <div class="alert alert-danger" role="alert">
          A simple danger alert with
          <a href="#" class="alert-link">an example link</a>. Give it a click if
          you like.
        </div>
        <div class="alert alert-warning" role="alert">
          A simple warning alert with
          <a href="#" class="alert-link">an example link</a>. Give it a click if
          you like.
        </div>
        <div class="alert alert-info" role="alert">
          A simple info alert with
          <a href="#" class="alert-link">an example link</a>. Give it a click if
          you like.
        </div>
        <div class="alert alert-light" role="alert">
          A simple light alert with
          <a href="#" class="alert-link">an example link</a>. Give it a click if
          you like.
        </div>
        <div class="alert alert-dark" role="alert">
          A simple dark alert with
          <a href="#" class="alert-link">an example link</a>. Give it a click if
          you like.
        </div>
      </div>
    </div>

````
<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/3.png" width="1024"
</p>

```php
    <div class="container">
      <div class="col-12">
        <div class="alert alert-success" role="alert">
          <h4 class="alert-heading">Well done!</h4>
          <p>
            Aww yeah, you successfully read this important alert message. This
            example text is going to run a bit longer so that you can see how
            spacing within an alert works with this kind of content.
          </p>
          <hr />
          <p class="mb-0">
            Whenever you need to, be sure to use margin utilities to keep things
            nice and tidy.
          </p>
        </div>
      </div>
    </div>

    <div class="container">
      <div class="col-12">
        <div
          class="alert alert-warning alert-dismissible fade show"
          role="alert"
        >
          <strong>Hola!!</strong> Tenes que completar todos los campos para
          poder guardar!
          <button
            type="button"
            class="close"
            data-dismiss="alert"
            aria-label="Close"
          >
            <span aria-hidden="true">&times;</span>
          </button>
        </div>
      </div>
    </div>

````




<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/4.png" width="1024"
</p>

```php
    <div class="text-center my-5">
      <h2>Badges</h2>
    </div>

    <div class="container">
      <div class="col-12">
        <h1>Example heading <span class="badge badge-primary">New</span></h1>
        <h2>Example heading <span class="badge badge-info">New</span></h2>
        <h3>Example heading <span class="badge badge-danger">New</span></h3>
        <h4>Example heading <span class="badge badge-success">New</span></h4>
        <h5>Example heading <span class="badge badge-warning">New</span></h5>
        <h6>Example heading <span class="badge badge-secondary">New</span></h6>
        <h6>Example heading <span class="badge badge-light">New</span></h6>
      </div>
    </div>

````



<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/5.png" width="1024"
</p>
  
```php

    <div class="text-center my-5">
      <h2>Notifications</h2>
    </div>

    <div class="container">
      <div class="col-12">
        <button type="button" class="btn btn-primary">
          Notifications <span class="badge badge-success">1</span>
        </button>
        <button type="button" class="btn btn-info">
          Notifications <span class="badge badge-primary">2</span>
        </button>
        <button type="button" class="btn btn-danger">
          Notifications <span class="badge badge-info">3</span>
        </button>
        <button type="button" class="btn btn-success">
          Notifications <span class="badge badge-warning">4</span>
        </button>
        <button type="button" class="btn btn-warning">
          Notifications <span class="badge badge-secondary">5</span>
        </button>
        <button type="button" class="btn btn-secondary">
          Notifications <span class="badge badge-warning">6</span>
        </button>
      </div>
    </div>

````




<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/6.png" width="1024"
</p>
  
```php

    <div class="text-center my-5">
      <h2>Badges pequenas</h2>
    </div>

    <div class="container">
      <div class="col-12">
        <span class="badge badge-primary">Primary</span>
        <span class="badge badge-secondary">Secondary</span>
        <span class="badge badge-success">Success</span>
        <span class="badge badge-danger">Danger</span>
        <span class="badge badge-warning">Warning</span>
        <span class="badge badge-info">Info</span>
        <span class="badge badge-light">Light</span>
        <span class="badge badge-dark">Dark</span>
      </div>
    </div>
````




<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/7.png" width="1024"
</p>
  
  

```php

    <div class="text-center my-5">
      <h2>Badges Pills</h2>
    </div>

    <div class="container">
      <div class="col-12">
        <span class="badge badge-pill badge-primary">Primary</span>
        <span class="badge badge-pill badge-secondary">Secondary</span>
        <span class="badge badge-pill badge-success">Success</span>
        <span class="badge badge-pill badge-danger">Danger</span>
        <span class="badge badge-pill badge-warning">Warning</span>
        <span class="badge badge-pill badge-info">Info</span>
        <span class="badge badge-pill badge-light">Light</span>
        <span class="badge badge-pill badge-dark">Dark</span>
      </div>
    </div>
    <hr />
````

<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/8.png" width="1024"
</p>
  
```php
  <div class="container">
    <div class="col-12">
      <button type="button" class="btn btn-primary">Primary</button>
      <button type="button" class="btn btn-secondary">Secondary</button>
      <button type="button" class="btn btn-success">Success</button>
      <button type="button" class="btn btn-danger">Danger</button>
      <button type="button" class="btn btn-warning">Warning</button>
      <button type="button" class="btn btn-info">Info</button>
      <button type="button" class="btn btn-light">Light</button>
      <button type="button" class="btn btn-dark">Dark</button>

      <button type="button" class="btn btn-link">Link</button>
    </div>
  </div>
```


<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/9.png" width="1024"
</p>
  
```php
  <div class="container">
    <div class="col-12">
      <button type="button" class="btn btn-outline-primary">Primary</button>
      <button type="button" class="btn btn-outline-secondary">
        Secondary
      </button>
      <button type="button" class="btn btn-outline-success">Success</button>
      <button type="button" class="btn btn-outline-danger">Danger</button>
      <button type="button" class="btn btn-outline-warning">Warning</button>
      <button type="button" class="btn btn-outline-info">Info</button>
      <button type="button" class="btn btn-outline-light">Light</button>
      <button type="button" class="btn btn-outline-dark">Dark</button>
    </div>
  </div>
```
  
<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/10.png" width="1024"
</p>
  
```php
<div class="container">
    <div class="col-12">
      <button type="button" class="btn btn-primary btn-sm">Primary</button>
      <button type="button" class="btn btn-secondary btn-sm">
        Secondary
      </button>
      <button type="button" class="btn btn-success btn-sm">Success</button>
      <button type="button" class="btn btn-danger btn-sm">Danger</button>
      <button type="button" class="btn btn-warning btn-sm">Warning</button>
      <button type="button" class="btn btn-info btn-sm">Info</button>
      <button type="button" class="btn btn-light btn-sm">Light</button>
      <button type="button" class="btn btn-dark btn-sm">Dark</button>
      <button type="button" class="btn btn-link btn-sm">Link</button>
    </div>
  </div>
````

  
  
<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/11.png" width="1024"
</p>
  
```php
<div class="container">
    <div class="col-12">
      <button type="button" class="btn btn-primary btn-sm">Primary</button>
      <button type="button" class="btn btn-secondary btn-sm">
        Secondary
      </button>
      <button type="button" class="btn btn-success btn-sm">Success</button>
      <button type="button" class="btn btn-danger btn-sm">Danger</button>
      <button type="button" class="btn btn-warning btn-sm">Warning</button>
      <button type="button" class="btn btn-info btn-sm">Info</button>
      <button type="button" class="btn btn-light btn-sm">Light</button>
      <button type="button" class="btn btn-dark btn-sm">Dark</button>
      <button type="button" class="btn btn-link btn-sm">Link</button>
    </div>
  </div>
````
  
<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/12.png" width="1024"
</p>
  
```php
  <div class="container">
    <div class="col-12">
      <button type="button" class="btn btn-primary btn-lg btn-block">
        aledc.tk
      </button>
      <button type="button" class="btn btn-secondary btn-lg btn-block">
        aledc.tk
      </button>
    </div>
  </div>
````

  
<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/13.png" width="1024"
</p>
  
```php
<div class="container">
    <div class="col-12">
      <div class="btn-group btn-group-toggle" data-toggle="buttons">
        <label class="btn btn-secondary active">
          <input type="radio" name="options" id="option1" checked /> Active
        </label>
        <label class="btn btn-secondary">
          <input type="radio" name="options" id="option2" /> Grupo
        </label>
        <label class="btn btn-secondary">
          <input type="radio" name="options" id="option3" /> De
        </label>
        <label class="btn btn-secondary">
          <input type="radio" name="options" id="option3" /> varios
        </label>
        <label class="btn btn-secondary">
          <input type="radio" name="options" id="option3" /> Botones
        </label>
      </div>
    </div>
  </div>
````

  
  
<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/14.png" width="1024"
</p>
 
```php
  <div class="container">
    <div class="col-12">
      <div class="btn-toolbar" role="toolbar" aria-label="Toolbar with button groups">
        <div class="btn-group mr-2" role="group" aria-label="First group">
          <button type="button" class="btn btn-primary">1</button>
          <button type="button" class="btn btn-secondary">2</button>
          <button type="button" class="btn btn-alert">3</button>
          <button type="button" class="btn btn-warning">4</button>
        </div>
        <div class="btn-group mr-2" role="group" aria-label="Second group">
          <button type="button" class="btn btn-danger">5</button>
          <button type="button" class="btn btn-success">6</button>
          <button type="button" class="btn btn-secondary">7</button>
        </div>
        <div class="btn-group" role="group" aria-label="Third group">
          <button type="button" class="btn btn-secondary">8</button>
        </div>
      </div>
    </div>
  </div>
````


  
  
<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/15.png" width="1024"
</p>
  
```php
<div class="container">
    <div class="col-12">
      <div class="btn-toolbar mb-3" role="toolbar" aria-label="Toolbar with button groups">
        <div class="btn-group mr-2" role="group" aria-label="First group">
          <button type="button" class="btn btn-secondary">1</button>
          <button type="button" class="btn btn-secondary">2</button>
          <button type="button" class="btn btn-secondary">3</button>
          <button type="button" class="btn btn-secondary">4</button>
        </div>
        <div class="input-group">
          <div class="input-group-prepend">
            <div class="input-group-text" id="btnGroupAddon">@</div>
          </div>
          <input type="text" class="form-control" placeholder="Input group example" aria-label="Input group example"
            aria-describedby="btnGroupAddon" />
        </div>
      </div>

      <div class="btn-toolbar justify-content-between" role="toolbar" aria-label="Toolbar with button groups">
        <div class="btn-group" role="group" aria-label="First group">
          <button type="button" class="btn btn-secondary">1</button>
          <button type="button" class="btn btn-secondary">2</button>
          <button type="button" class="btn btn-secondary">3</button>
          <button type="button" class="btn btn-secondary">4</button>
        </div>
        <div class="input-group">
          <div class="input-group-prepend">
            <div class="input-group-text" id="btnGroupAddon2">@</div>
          </div>
          <input type="text" class="form-control" placeholder="Input group example" aria-label="Input group example"
            aria-describedby="btnGroupAddon2" />
        </div>
      </div>
    </div>
  </div>
````
  
  
<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/16.png" width="1024"
</p>
  
```php
<div class="container">
    <div class="col-12">
      <div class="btn-group" role="group" aria-label="Button group with nested dropdown">
        <button type="button" class="btn btn-secondary">1</button>
        <button type="button" class="btn btn-secondary">2</button>

        <div class="btn-group" role="group">
          <button id="btnGroupDrop1" type="button" class="btn btn-secondary dropdown-toggle" data-toggle="dropdown"
            aria-haspopup="true" aria-expanded="false">
            Dropdown
          </button>
          <div class="dropdown-menu" aria-labelledby="btnGroupDrop1">
            <a class="dropdown-item" href="#">Dropdown link</a>
            <a class="dropdown-item" href="#">Dropdown link</a>
          </div>
        </div>
      </div>
    </div>
  </div>
````
  
<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/17.png" width="1024"
</p>


```php
<div class="container">
    <div class="col-12">
      <div class="btn-group btn-group-toggle btn-group-vertical" data-toggle="buttons">
        <label class="btn btn-secondary active">
          <input type="radio" name="options" id="option1" checked /> Active
        </label>
        <label class="btn btn-secondary">
          <input type="radio" name="options" id="option2" /> Grupo
        </label>
        <label class="btn btn-secondary">
          <input type="radio" name="options" id="option3" /> De
        </label>
        <label class="btn btn-secondary">
          <input type="radio" name="options" id="option3" /> varios
        </label>
        <label class="btn btn-secondary">
          <input type="radio" name="options" id="option3" /> Botones
        </label>
      </div>
    </div>
  </div>
````



<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/18.png" width="1024"
</p>
  
```php
<div class="container">
    <div class="row">
      <div class="col-4">
        <div class="card" style="width: 18rem;">
          <img src="./img/car2.jpeg" class="card-img-top" alt="..." />
          <div class="card-body">
            <h5 class="card-title">Card title</h5>
            <p class="card-text">
              Some quick example text to build on the card title and make up
              the bulk of the card's content.
            </p>
            <a href="#" class="btn btn-primary">Go somewhere</a>
          </div>
        </div>
      </div>

      <div class="col-4">
        <div class="card" style="width: 18rem;">
          <img src="./img/car.jpeg" class="card-img-top" alt="..." />
          <div class="card-body">
            <h5 class="card-title">Card title</h5>
            <p class="card-text">
              Some quick example text to build on the card title and make up
              the bulk of the card's content.
            </p>
            <a href="#" class="btn btn-primary">Go somewhere</a>
          </div>
        </div>
      </div>

      <div class="col-4">
        <div class="card" style="width: 18rem;">
          <img src="./img/car2.jpeg" class="card-img-top" alt="..." />
          <div class="card-body">
            <h5 class="card-title">Card title</h5>
            <p class="card-text">
              Some quick example text to build on the card title and make up
              the bulk of the card's content.
            </p>
            <a href="#" class="btn btn-primary">Go somewhere</a>
          </div>
        </div>
      </div>
    </div>
  </div>
````

  
<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/19.png" width="1024"
</p>
  
```php
  <div class="container">
    <div class="row">
      <div class="col-6">
        <div class="card mb-3" style="max-width: 540px;">
          <div class="row no-gutters">
            <div class="col-md-4">
              <img src="./img/car2.jpeg" class="card-img" alt="..." />
            </div>
            <div class="col-md-8">
              <div class="card-body">
                <h5 class="card-title">Card title</h5>
                <p class="card-text">
                  This is a wider card with supporting text below as a natural
                  lead-in to additional content. This content is a little bit
                  longer.
                </p>
                <p class="card-text">
                  <small class="text-muted">Last updated 3 mins ago</small>
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="col-6">
        <div class="card mb-3" style="max-width: 540px;">
          <div class="row no-gutters">
            <div class="col-md-4">
              <img src="./img/car.jpeg" class="card-img" alt="..." />
            </div>
            <div class="col-md-8">
              <div class="card-body">
                <h5 class="card-title">Card title</h5>
                <p class="card-text">
                  This is a wider card with supporting text below as a natural
                  lead-in to additional content. This content is a little bit
                  longer.
                </p>
                <p class="card-text">
                  <small class="text-muted">Last updated 3 mins ago</small>
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
````
  
  
<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/20.png" width="1024"
</p>
  
```php
 <div class="container">
    <div class="row">
      <div class="col-3">
        <div class="card text-white bg-primary mb-3" style="max-width: 18rem;">
          <div class="card-header">Header</div>
          <div class="card-body">
            <h5 class="card-title">Primary card title</h5>
            <p class="card-text">
              Some quick example text to build on the card title and make up
              the bulk of the card's content.
            </p>
          </div>
        </div>
      </div>

      <div class="col-3">
        <div class="card text-white bg-secondary mb-3" style="max-width: 18rem;">
          <div class="card-header">Header</div>
          <div class="card-body">
            <h5 class="card-title">Secondary card title</h5>
            <p class="card-text">
              Some quick example text to build on the card title and make up
              the bulk of the card's content.
            </p>
          </div>
        </div>
      </div>

      <div class="col-3">
        <div class="card text-white bg-success mb-3" style="max-width: 18rem;">
          <div class="card-header">Header</div>
          <div class="card-body">
            <h5 class="card-title">Success card title</h5>
            <p class="card-text">
              Some quick example text to build on the card title and make up
              the bulk of the card's content.
            </p>
          </div>
        </div>
      </div>

      <div class="col-3">
        <div class="card text-white bg-danger mb-3" style="max-width: 18rem;">
          <div class="card-header">Header</div>
          <div class="card-body">
            <h5 class="card-title">Danger card title</h5>
            <p class="card-text">
              Some quick example text to build on the card title and make up
              the bulk of the card's content.
            </p>
          </div>
        </div>
      </div>
    </div>

    <div class="row">
      <div class="col-3">
        <div class="card text-white bg-info mb-3" style="max-width: 18rem;">
          <div class="card-header">Header</div>
          <div class="card-body">
            <h5 class="card-title">Info card title</h5>
            <p class="card-text">
              Some quick example text to build on the card title and make up
              the bulk of the card's content.
            </p>
          </div>
        </div>
      </div>

      <div class="col-3">
        <div class="card bg-light mb-3" style="max-width: 18rem;">
          <div class="card-header">Header</div>
          <div class="card-body">
            <h5 class="card-title">Light card title</h5>
            <p class="card-text">
              Some quick example text to build on the card title and make up
              the bulk of the card's content.
            </p>
          </div>
        </div>
      </div>

      <div class="col-3">
        <div class="card text-white bg-dark mb-3" style="max-width: 18rem;">
          <div class="card-header">Header</div>
          <div class="card-body">
            <h5 class="card-title">Dark card title</h5>
            <p class="card-text">
              Some quick example text to build on the card title and make up
              the bulk of the card's content.
            </p>
          </div>
        </div>
      </div>

      <div class="col-3">
        <div class="card text-white bg-warning mb-3" style="max-width: 18rem;">
          <div class="card-header">Header</div>
          <div class="card-body">
            <h5 class="card-title">Warning card title</h5>
            <p class="card-text">
              Some quick example text to build on the card title and make up
              the bulk of the card's content.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
````

  

<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/21.png" width="1024"
</p>
  
```php
<div class="container">
    <div class="row">
      <div class="col-3">
        <div class="card border-primary mb-3" style="max-width: 18rem;">
          <div class="card-header">Header</div>
          <div class="card-body text-primary">
            <h5 class="card-title">Primary card title</h5>
            <p class="card-text">
              Some quick example text to build on the card title and make up
              the bulk of the card's content.
            </p>
          </div>
        </div>
      </div>

      <div class="col-3">
        <div class="card border-dark mb-3" style="max-width: 18rem;">
          <div class="card-header">Header</div>
          <div class="card-body text-dark">
            <h5 class="card-title">Dark card title</h5>
            <p class="card-text">
              Some quick example text to build on the card title and make up
              the bulk of the card's content.
            </p>
          </div>
        </div>
      </div>

      <div class="col-3">
        <div class="card border-light mb-3" style="max-width: 18rem;">
          <div class="card-header">Header</div>
          <div class="card-body">
            <h5 class="card-title">Light card title</h5>
            <p class="card-text">
              Some quick example text to build on the card title and make up
              the bulk of the card's content.
            </p>
          </div>
        </div>
      </div>

      <div class="col-3">
        <div class="card border-info mb-3" style="max-width: 18rem;">
          <div class="card-header">Header</div>
          <div class="card-body text-info">
            <h5 class="card-title">Info card title</h5>
            <p class="card-text">
              Some quick example text to build on the card title and make up
              the bulk of the card's content.
            </p>
          </div>
        </div>
      </div>
    </div>

    <div class="row">
      <div class="col-3">
        <div class="card border-danger mb-3" style="max-width: 18rem;">
          <div class="card-header">Header</div>
          <div class="card-body text-danger">
            <h5 class="card-title">Danger card title</h5>
            <p class="card-text">
              Some quick example text to build on the card title and make up
              the bulk of the card's content.
            </p>
          </div>
        </div>
      </div>

      <div class="col-3">
        <div class="card border-secondary mb-3" style="max-width: 18rem;">
          <div class="card-header">Header</div>
          <div class="card-body text-secondary">
            <h5 class="card-title">Secondary card title</h5>
            <p class="card-text">
              Some quick example text to build on the card title and make up
              the bulk of the card's content.
            </p>
          </div>
        </div>
      </div>

      <div class="col-3">
        <div class="card border-success mb-3" style="max-width: 18rem;">
          <div class="card-header">Header</div>
          <div class="card-body text-success">
            <h5 class="card-title">Success card title</h5>
            <p class="card-text">
              Some quick example text to build on the card title and make up
              the bulk of the card's content.
            </p>
          </div>
        </div>
      </div>

      <div class="col-3">
        <div class="card border-warning mb-3" style="max-width: 18rem;">
          <div class="card-header">Header</div>
          <div class="card-body text-warning">
            <h5 class="card-title">Warning card title</h5>
            <p class="card-text">
              Some quick example text to build on the card title and make up
              the bulk of the card's content.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
````

  
<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/22.png" width="1024"
</p>
  
```php
<div class="container">
    <div class="row">
      <div class="col-4">
        <div class="card border-success mb-3" style="max-width: 18rem;">
          <div class="card-header bg-transparent border-success">Header</div>
          <div class="card-body text-success">
            <h5 class="card-title">Success card title</h5>
            <p class="card-text">
              Some quick example text to build on the card title and make up
              the bulk of the card's content.
            </p>
          </div>
          <div class="card-footer bg-transparent border-success">Footer</div>
        </div>
      </div>
      <div class="col-4">
        <div class="card border-danger mb-3" style="max-width: 18rem;">
          <div class="card-header bg-transparent border-danger">Header</div>
          <div class="card-body text-danger">
            <h5 class="card-title">Danger card title</h5>
            <p class="card-text">
              Some quick example text to build on the card title and make up
              the bulk of the card's content.
            </p>
          </div>
          <div class="card-footer bg-transparent border-danger">Footer</div>
        </div>
      </div>

      <div class="col-4">
        <div class="card border-primary mb-3" style="max-width: 18rem;">
          <div class="card-header bg-transparent border-primary">Header</div>
          <div class="card-body text-primary">
            <h5 class="card-title">Danger card title</h5>
            <p class="card-text">
              Some quick example text to build on the card title and make up
              the bulk of the card's content.
            </p>
          </div>
          <div class="card-footer bg-transparent border-primary">Footer</div>
        </div>
      </div>
    </div>
  </div>
````

  
  
<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/23.png" width="1024"
</p>
  
```php
<div class="container">
    <div class="row">
      <div class="col-4">
        <div class="card border-success mb-3" style="max-width: 18rem;">
          <div class="card-header bg-transparent border-success">Header</div>
          <div class="card-body text-success">
            <h5 class="card-title">Success card title</h5>
            <p class="card-text">
              Some quick example text to build on the card title and make up
              the bulk of the card's content.
            </p>
          </div>
          <div class="card-footer bg-transparent border-success">Footer</div>
        </div>
      </div>
      <div class="col-4">
        <div class="card border-danger mb-3" style="max-width: 18rem;">
          <div class="card-header bg-transparent border-danger">Header</div>
          <div class="card-body text-danger">
            <h5 class="card-title">Danger card title</h5>
            <p class="card-text">
              Some quick example text to build on the card title and make up
              the bulk of the card's content.
            </p>
          </div>
          <div class="card-footer bg-transparent border-danger">Footer</div>
        </div>
      </div>

      <div class="col-4">
        <div class="card border-primary mb-3" style="max-width: 18rem;">
          <div class="card-header bg-transparent border-primary">Header</div>
          <div class="card-body text-primary">
            <h5 class="card-title">Danger card title</h5>
            <p class="card-text">
              Some quick example text to build on the card title and make up
              the bulk of the card's content.
            </p>
          </div>
          <div class="card-footer bg-transparent border-primary">Footer</div>
        </div>
      </div>
    </div>
  </div>

  <hr />

  <div class="text-center my-5">
    <h2>Collapse Elementos</h2>
  </div>


  <div class="container">
    <div class="col-12">
      <p>
        <a class="btn btn-primary" data-toggle="collapse" href="#multiCollapseExample1" role="button"
          aria-expanded="false" aria-controls="multiCollapseExample1">Mostrar Primer Elemento</a>
        <button class="btn btn-primary" type="button" data-toggle="collapse" data-target="#multiCollapseExample2"
          aria-expanded="false" aria-controls="multiCollapseExample2">Mostrar Segundi Elemento</button>
        <button class="btn btn-primary" type="button" data-toggle="collapse" data-target=".multi-collapse"
          aria-expanded="false" aria-controls="multiCollapseExample1 multiCollapseExample2">Mostrar Ambos
          Elementos</button>
      </p>
      <div class="row">
        <div class="col">
          <div class="collapse multi-collapse" id="multiCollapseExample1">
            <div class="card card-body">
              Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry richardson ad squid. Nihil anim
              keffiyeh helvetica, craft beer labore wes anderson cred nesciunt sapiente ea proident.
            </div>
          </div>
        </div>
        <div class="col">
          <div class="collapse multi-collapse" id="multiCollapseExample2">
            <div class="card card-body">
              Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry richardson ad squid. Nihil anim
              keffiyeh helvetica, craft beer labore wes anderson cred nesciunt sapiente ea proident.
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
````

## NavBar

El nanbar puede ser alineado a la izquierda, centro o derecha modificando la siguiente clase.     

__ml-auto__  = alinea a la derecha  (aunque tenga la L de left, al parecer bootstrap lo usa al reves)   
__mr-auto__ = alinea a la izquierda.   
__m-auto__ = alinea al centro si no se le pone ni L ni R.   



```php
<ul class="navbar-nav ml-auto">
````
<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/24.png" width="1024"
</p>
  
  
```php
<ul class="navbar-nav mr-auto">
````  
<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/25.png" width="1024"
</p>
 
 
```php
<ul class="navbar-nav m-auto">
```` 
<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/26.png" width="1024"
</p>  




```php
<nav class="navbar navbar-expand-lg navbar-light bg-light">
    <a class="navbar-brand" href="#">Navbar</a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent"
      aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse" id="navbarSupportedContent">
    
    
      <ul class="navbar-nav ml-auto">
        <li class="nav-item active">
          <a class="nav-link" href="landing.html">Inicio <span class="sr-only">(current)</span></a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="contacto.html">Contacto</a>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown"
            aria-haspopup="true" aria-expanded="false">
            Dropdown
          </a>
          <div class="dropdown-menu" aria-labelledby="navbarDropdown">
            <a class="dropdown-item" href="#">Action</a>
            <a class="dropdown-item" href="#">Another action</a>
            <div class="dropdown-divider"></div>
            <a class="dropdown-item" href="#">Something else here</a>
          </div>
        </li>
        <li class="nav-item">
          <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</a>
        </li>
      </ul>
      <form class="form-inline my-2 my-lg-0">
        <input class="form-control mr-sm-2" type="search" placeholder="Search" aria-label="Search" />
        <button class="btn btn-outline-success my-2 my-sm-0" type="submit">
          Search
        </button>
      </form>
    </div>
  </nav>
````

## Logo en el Navbar

<p align="center">
  <img align="center" src="https://raw.githubusercontent.com/aledc7/Bootstrap/master/resources/27.png" width="1024"
</p>  

Para agregar el logo de la companía o el producto al NavBar puede hacerse de la siguiente manera:   

```php
# Luego del nav principal...
<nav class="container navbar navbar-expand-lg navbar-light bg-dark fixed-top">
    
      # Agregar esta etiqueta "A" y dentro incluir una imagen, preferentemente en SVG. 
      <a class="navbar-brand" href="#">
        <img src="./img/Logo-overport.svg" width="40" height="40" class="d-inline-block align-top" alt="">
      </a>
      
      # Luego Aqui el nombre de la compania.
      <div class="align-self-center text-white">
        OVERPORT
      </div>
````


## Fijar el NavBar en el TOP o en el Bottom de la página.

Generalmente se querrá que el NavBar quede fijo en el Header de la página, esto se logra con las clases:  
__fixed-top__  Para alinear en el header.  
__fixed-bottom__  Para alinear en el footer.   

ambas clases deben agregarse en el __nav__ principal del navbar.     

__fixed-top__   
````php
<nav class="container navbar navbar-expand-lg navbar-light bg-dark fixed-top">
````

__fixed-bottom__   
````php
<nav class="container navbar navbar-expand-lg navbar-light bg-dark fixed-bottom">
`````
También existe la posibilidad de dejar el header movil, pero que se detenga al llegar al tope de la página, este comportamiento se lo conoce como __"Sticky"__   
 Es posible aplicar este comportamiento tanto en el header (___stycky-top__) como en el footer (__sticky_bottom__)   

__sticky-top__   
````php
<nav class="container navbar navbar-expand-lg navbar-light bg-dark sticky-top">
`````










  






