# Tipos de Datos Primitivos de JavaScript

En JavaScript `JS` existen varios tipos de datos primitivos, que son los bloques fundamentales para construir estructuras de datos mas complejas (`Objects`, `Arrays`, `Maps`, `Sets`, `Matrices`):

## String

`string` representa secuencias de caracteres. Se pueden definir usando comillas simples, dobles o invertidas. Es un conjunto de "elementos" de valores enteros sin signo de 16 bits. Cada carácter del `String` ocupa una posición en la cadena, es decir, el primer carácter se encuentra en el índice `0`, el segundo se encuentra en el índice `1` y así sucesivamente.

```javascript
let nombre = 'Lenin';
```



## Boolean

`boolean` representa un valor de `true` (`1`) o `false` (`0`).

```javascript
let mayorDeEdad = true;
```



## Number

`number` representa valores numéricos ya sean enteros o decimales. Es un valor en formato binario de 64 bits de doble precisión IEEE 754 (números entre -(253-1) y (253-1)). Tiene tres valores simbólicos: +Infinity, -Infinity y NaN.

```javascript
let edad = 18;
```



## BigInt

`BigInt` representa enteros más grandes de lo que puede manejar el tipo de dato `number`. Se crea agregando `n` al final del numero entero.

```javascript
let edad = 18;
```



## Symbol

`Symbol` Representa un valor único e inmutable. Se crea utilizando la función global `Symbol()`. 

```javascript
let simbolo = Symbol('description')
```



## Null

`Null` Representa la ausencia intencionada de cualquier valor. Tiene exactamente un valor `Null`.

```javascript
let valorNulo = null;
```



## Undefined

`Undefined` Representa una variable que ha sido declarada pero no inicializada. Una variable que no se le ha asignado un valor entonces toma toma el valor `Undefined`.

```javascript
let valorIndefinido;
```

