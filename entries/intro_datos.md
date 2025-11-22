# Introducción a los datos

Entender como funcionan los datos es crucial en informática por lo que es importante no saltar esta sección.

- [Qué son los datos - IBM](https://www.ibm.com/es-es/think/topics/data)

Los computadores son máquinas que funcionan internamente mediante instrucciones binarias. Cuando hablamos de datos, debemos entender que todo puede representarse como números y secuencias de bits. Un bit es la unidad mínima de información y solo puede tomar dos valores: 0 o 1.

Actualmente, la mayoría de los computadores operan con arquitecturas de 64 bits, lo que significa que pueden procesar instrucciones de 64 bits de longitud. Como todos los datos se construyen a partir de bits, es importante entender que no son infinitos: cada máquina tiene una capacidad máxima determinada por su arquitectura.

Tamaños comunes:

* 1 byte = 8 bits
* 1 Kilobyte = 1000 bytes
* 1 Megabyte = 1000 Kilobytes 10⁶bytes
* 1 gigabyte = 1000 megabytes 10⁹bytes
* 1 terabyte = 1000 gigabytes 10¹²bytes

Los lenguajes de programación al usar datos, distribuyen su tamaño según el tipo de dato, y este tiene un tamaño según el lenguaje de programación:

Tipos primitivos:

* int/integer = números enteros que representan valores enteros. *Más ligeros*
* float = números decimales de precisión simple.
* double = números decimales de doble precisión.
* char = representan caracteres. (Internamente se guardan en números para poder ser usados medante bits) 
* string = secuencias de valores tipo `char` para formar cadenas de textos
* bool = se componen de 2 estados; `true` y `false`

Tipos compuestos:
* arrays = colecciones de elementos del mismo tipo de forma secuencial en memoria. (Útiles como listas)
* struct = conjuntos de datos agrupados bajo un mismo tipo
* object = son `struct`s que soportan métodos
* maps = colecciones de pares (clave/valor)

Recurso recomendado
- [Tipos de datos - TodoCode](https://www.youtube.com/watch?v=_lNtSsEcnwc)

---
[Inicio](../README.md) [Siguiente](./intro_primerlang.md)
