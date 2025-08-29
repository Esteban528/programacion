# Programación Orientada a Objetos en Java

## 1. Classes and Objects
En Java, una **clase** es un molde o plantilla que define atributos (datos) y métodos (comportamientos).  
Un **objeto** es una instancia de una clase creada en tiempo de ejecución.

```java
class Persona {
    String nombre;
    void saludar() { System.out.println("Hola"); }
}

Persona p = new Persona(); // objeto
````

---

## 2. Attributes and Methods

* **Atributos:** Variables declaradas dentro de una clase que representan el estado del objeto.
* **Métodos:** Funciones dentro de la clase que definen su comportamiento.

---

## 3. Access Specifiers

Controlan la **visibilidad** de atributos y métodos:

* `public`: accesible desde cualquier lugar.
* `private`: accesible solo dentro de la clase.
* `protected`: accesible en el mismo paquete y por herencia.
* (default): accesible solo dentro del mismo paquete.

---

## 4. Static Keyword

* **Atributos estáticos:** compartidos por todas las instancias de la clase.
* **Métodos estáticos:** se pueden usar sin crear objetos.

```java
class Util {
    static int contador = 0;
    static void mostrar() { ... }
}
```

---

## 5. Final Keyword

* **Clase `final`:** no se puede heredar.
* **Método `final`:** no se puede sobrescribir.
* **Variable `final`:** es constante, no se puede reasignar.

---

## 6. Nested Classes

Clases definidas dentro de otra clase. Se usan para agrupar lógicamente código y mejorar encapsulación.
Pueden ser **estáticas** o **internas** (inner classes).

---

## 7. Packages

Mecanismo para organizar clases en módulos lógicos y evitar colisiones de nombres.
Ejemplo: `java.util`, `java.io`.

---

## 8. More about OOP

Principios fundamentales:

* **Abstracción:** ocultar detalles innecesarios.
* **Encapsulación:** proteger datos dentro de una clase.
* **Herencia:** reutilizar código mediante jerarquías.
* **Polimorfismo:** múltiples formas de un mismo método o comportamiento.

---

## 9. Object Lifecycle

Un objeto pasa por varias etapas:

1. Creación (`new`).
2. Uso (métodos, atributos).
3. Destrucción (colector de basura de Java).

---

## 10. Inheritance

Permite que una clase (subclase) herede atributos y métodos de otra (superclase).
Se usa `extends`.

```java
class Animal { void comer() {} }
class Perro extends Animal { void ladrar() {} }
```

---

## 11. Abstraction

Proceso de ocultar detalles de implementación y mostrar solo lo esencial.
Se logra con **clases abstractas** y **interfaces**.

---

## 12. Method Chaining

Técnica que permite llamar varios métodos seguidos porque cada uno devuelve el objeto actual (`this`).

```java
obj.metodo1().metodo2().metodo3();
```

---

## 13. Encapsulation

Consiste en declarar atributos como `private` y proporcionar métodos **getters y setters** para controlar el acceso.

---

## 14. Interfaces

Definen un contrato que las clases deben implementar. Solo contienen métodos abstractos (Java 7) o también métodos `default` y `static` (Java 8+).

---

## 15. Enums

Tipo especial para representar un conjunto fijo de constantes con nombre.

```java
enum Dia { LUNES, MARTES, MIERCOLES }
```

---

## 16. Record

Introducido en Java 16. Permite crear clases inmutables y concisas para representar datos.

```java
record Punto(int x, int y) {}
```

---

## 17. Method Overloading / Overriding

* **Overloading:** varios métodos con el mismo nombre pero diferente firma.
* **Overriding:** redefinir un método heredado de la superclase.

---

## 18. Initializer Block

Bloques de código en una clase que se ejecutan al crear objetos.

* **Bloques de instancia `{}`**
* **Bloques estáticos `static {}`**

---

## 19. Static vs Dynamic Binding

* **Static binding (en tiempo de compilación):** métodos `private`, `static` o `final`.
* **Dynamic binding (en tiempo de ejecución):** métodos sobrescritos dependen del objeto real.

---

## 20. Pass by Value / Pass by Reference

En Java:

* Siempre es **pass by value** (se copia el valor).
* En objetos, se pasa la **referencia por valor**, por lo que ambos apuntan al mismo objeto, pero no se puede cambiar la referencia original.

---
