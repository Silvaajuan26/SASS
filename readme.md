# SASS
 
## CSS PLANO (DESVENTAJAS)

- Una de las desventajas del uso de CSS plano es que no es muy factible para proyectos de amplia codificacion, ya que se englobaria miles de lineas de codigo en un solo archivo .css lo que dificultaria en tareas como dar mantenimiento, solucion de error, modificaciones... 

## QUE ES UN PROCESADOR

- Los procesadores son herramientas que resuelven exactamente todas las desventajas que tiene el usar el CSS plano que mencione anteriormente, como la capacidad de mantenimiento y la organizacion de las hojas de estilo.

## SASS (VENTAJAS)

- Una de las ventajas del uso de SASS es que permite generar de manera automatica hojas de estilos, insertando caracteristicas como la definicion de variables, funciones, selectores, etc. 


## VARIABLES

- Las variables son definidas para poder almacenar datos que podemos usar a lo largo de todas las lineas de codigo (estas se denotan con el signo $).

```
$containerColor: rgb(255, 6, 151);
```



## ANIDAMIENTO (SELECTORES)

- Los anidamientos con selectores permite definir variables de una forma mas organizada ya que podemos poner selectores dentro de otros selectores.

```
.container {
  width: 100%;
  padding: 10px;

  .header {
    background-color: black;

    h1 {
      color: #000;
    }

    p {
      color: #666;
    }
  }
```

## ANIDAMIENTO AMPERSAND(&)

- Al igual que el anterior, con la diferencia de que al estar definiendo codigo anidado y usamos el $ podemos continuar el uso del selector en el cual estamos trabajando, paa no tener ue repetirlo de nuevo.

```
a.MyStyle {
  color: red;
  &:hover {  (que seria igual a: a.MyStyle:hover)
    background-color: #000;
  }
}

```

## IMPORTACION (MODULARIDAD)(PARTIAL)
 
 - Partial es una de las cosas que nos ofrece el SASS, ya que nos permite crear hojas de estilos en pequenos archivos que posteriormente podemos importar a nuestra hoja de estilo principal.

 ```
 @import 'header';
 ```