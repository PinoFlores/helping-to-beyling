# 4. Los datos y sus tipos


## Que son los datos primitivos?

En javascript los datos primitivos son los datos que no son objectos y no tienen metodos.

En javascript existen 6 tipos de datos primitivos.

- undefined
- boolean
- number
- string
- bigint
- symbol


### undefined

Representa una variable a la que no se le ha asignado un valor, un funcion que no devuelve nada y tratamos de asignar su retorno a una variable.

Si traducimos `undefined` al castellano, significa indefinida.

```js

var total;
console.log(total);

// Output: undefined
```

### boolean

Representa un valor negativo o positivo: `true` o `false`. 

**Caso de uso**: 
    - puede representar si un usuario esta conectado o no.
    - si una contrasena esta valida o no.
    - si un servicio esta activo o no.



```js
var isEnabled = true; // algo que esta habilidato.
var isOnline = false; // un usuario que no esta en linea.
```


### number

El tipo `number` representa un rango completo de numeros, incluyendo los negativos, positivos y decimales.



**Caso de uso**: 
    - puede representar la distancia de algo
    - puede representar la cantidad de algo
    - puede representar la ubicacion de un punto en el espacio
    - o cualquier magnitud



```js
var temperatura = 25; // la temperatura del ambiente
var balance = 20000; // el balance de una cuenta
var duracion = 36000; // la duracion de un evento en milisegundos
```



### string

Las cadenas o `string` representa un texto.

**Caso de uso**: 
    - simple: representa cualquier texto.


```js
var nombre = "Juana"; // el nombre de una persona
var direccion = "Cerca de aqui, lejos de alla."; // la direccion de alguien
```



## null

Este es un tipo de datos primitivo especial en javascript. Y su definiion general seria la siguiente:

- representa a ausencia intencional de cualquier valor.

```js
var referencia = null;
```



## function

Es un tipo de dato estructural pero sin datos.

Representa una accion.

**Caso de uso**: 
    - enviarUnEmail
    - retirarDinero
    - validarCredenciales


Hay una seccion mas adelante donde hablamos a detalle de este tema, de momento quedate con esa idea.



## object

Este es un tipo de datos estructural que contiene propiedades hijas dentro de el.

Veamos a un objecto como lo veriamos en el mundo real.

Si hablamos de un coche pues lo describiriamos en funcion de sus propiuedades.

- color
- precio
- velocidad
- altura
- numero de plazas
- funciones


Y si hablamos de algo mas abstracto como una cuenta bancaria, la describiramos en funcion de:

- propietario
- tipo
- numero

Y si hablamos de un objecto tipo cadena de texto:

- su logitud
- capacidad de convertirse en mayuscula
- etc





```js
var cuentaBancaria = {
	tipo: "corrente",
    numero: 1234567,
    propietatio : {
    	nombre : "Pepito"
    },
    ingresarDinero : function(monto) {
    	//
    }
}
```

Como podemos ver a simple vista, parece que un objecto es la coleccion tanto de tipos primitivos, de funciones a como de mas objectos. Pues si asi es.


Los objectos tiene propiedades:
	- datos 
	- acciones



## Importante

Anteriormente hemos dicho que los datos de tipo primitivos no tienen propiedades, verdad? Entonces, por que es esto posible? (hablando del codigo siguiente).

```js
    "Hello World".toUpperCase();
```


Si bien hemos dicho que un dato primitivo es un dato que no es un objeto y por lo tanto no tiene propiedades. El lenguaje nos provee de implementaciones de cada uno de eso datos primitivos en forma de objectos a los que se les conoce como wrappers. 

A este proceso se le conoce como Coercion.


## Resumen

Entonces estos son todos los tipos de datos que existen en js.

- undefined
- null
- boolean
- number
- string
- bigint
- symbol
- function
- object