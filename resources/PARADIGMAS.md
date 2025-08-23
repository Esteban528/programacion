# Paradigmas de Programación

En informática, un **paradigma de programación** es un modelo conceptual que define cómo se estructuran y ejecutan los programas. No se trata únicamente de “estilos” de codificación, sino de formas de **abstracción computacional** que determinan cómo expresamos algoritmos, manipulamos datos y controlamos el flujo de ejecución.

Los paradigmas se pueden clasificar de varias formas (por ejemplo, *imperativos vs. declarativos*), pero aquí analizaremos los principales con un enfoque técnico.
Un programador experto suele **mezclar paradigmas** según el contexto, usando la herramienta más adecuada para cada problema.

---

## 1. Programación Imperativa

* **Definición:**
  Se centra en **describir el estado del programa** y cómo cambia a través de **instrucciones secuenciales**. Un programa imperativo es esencialmente una lista ordenada de comandos que modifican memoria y controlan el flujo.

* **Características Clave:**

  * Uso explícito de **variables** como contenedores de estado.
  * Dependencia del **orden de ejecución**.
  * Control de flujo mediante estructuras (`if`, `while`, `for`, `goto`).
  * **Efectos secundarios** frecuentes.

* **Ventajas:**

  * Similitud con el hardware (máquina de Turing, Von Neumann).
  * Eficiencia en tiempo de ejecución.
  * Alta optimización por compiladores.

* **Desventajas:**

  * Dificultad de razonar sobre el estado global en programas grandes.
  * Código menos modular y propenso a errores de mutación.

* **Ejemplo (C):**

```c
#include <stdio.h>

int main() {
    int suma = 0;
    for (int i = 1; i <= 10; i++) {
        suma += i; // Mutación del estado
    }
    printf("Suma: %d\n", suma);
    return 0;
}
```

---

## 2. Programación Declarativa

* **Definición:**
  Describe el **qué** debe hacerse, no el **cómo** hacerlo. El control de flujo se delega al motor de ejecución (intérprete, motor de reglas, planificador, etc.).

* **Subparadigmas principales:**

  * **Funcional** → Computación como evaluación de funciones matemáticas.
  * **Lógica** → Computación como deducción de hechos y reglas.
  * **Lenguajes de consultas** → Especificación de propiedades (SQL, Datalog).

* **Ventajas:**

  * Alta expresividad y abstracción.
  * Menor probabilidad de errores de control de flujo.
  * Ideal para optimización automática.

* **Desventajas:**

  * Menor control explícito del rendimiento.
  * Curva de aprendizaje más pronunciada.

* **Ejemplo (SQL):**

```sql
SELECT SUM(numero)
FROM numeros
WHERE numero BETWEEN 1 AND 10;
```

Aquí el *qué* (sumar entre 1 y 10) está claro, pero el *cómo* (iteraciones, índices, ejecución) queda en manos del motor de base de datos.

---

## 3. Programación Orientada a Objetos (OOP)

* **Definición:**
  Modelo que organiza el software en torno a **objetos**, instancias de **clases** que encapsulan datos (*estado*) y comportamiento (*métodos*).

* **Principios Clásicos:**

  * **Encapsulación** → Ocultamiento de detalles internos.
  * **Abstracción** → Representación de entidades complejas con interfaces simples.
  * **Herencia** → Reutilización jerárquica de código.
  * **Polimorfismo** → Intercambiabilidad de objetos mediante interfaces comunes.

* **Ventajas:**

  * Modularidad y reusabilidad.
  * Cercanía al modelado de dominios del mundo real.
  * Favorece patrones de diseño y arquitecturas escalables.

* **Desventajas:**

  * Complejidad en jerarquías profundas.
  * Overhead en tiempo de ejecución (dispatch dinámico).
  * Posible abuso de herencia (antipatrones).

* **Ejemplo (Java):**

```java
class Perro {
    private String nombre;
    private String raza;

    public Perro(String nombre, String raza) {
        this.nombre = nombre;
        this.raza = raza;
    }

    public void ladrar() {
        System.out.println("Guau!");
    }

    public static void main(String[] args) {
        Perro p = new Perro("Fido", "Labrador");
        p.ladrar();
    }
}
```

---

## 4. Programación Funcional

* **Definición:**
  Computación como **evaluación de funciones puras**, evitando estado mutable y efectos secundarios.
  Inspirada en el **λ-cálculo** de Church (1930s).

* **Características Técnicas:**

  * **Inmutabilidad** de datos.
  * **Funciones puras** (misma entrada → misma salida).
  * **Funciones de orden superior** (reciben y devuelven funciones).
  * Uso extensivo de **recursión** sobre bucles.

* **Ventajas:**

  * Código más predecible y fácil de razonar.
  * Ideal para programación concurrente (sin mutación compartida).
  * Expresividad matemática.

* **Desventajas:**

  * Rendimiento afectado por inmutabilidad en algunos casos.
  * Curva de aprendizaje elevada (Haskell, OCaml, Erlang).
  * Paradigma menos natural para problemas muy procedimentales.

* **Ejemplo (Haskell):**

```haskell
dobles :: [Int] -> [Int]
dobles = map (*2)

main :: IO ()
main = print (dobles [1,2,3,4])
```

---

## 5. Programación Lógica

* **Definición:**
  Basada en **lógica matemática** (cláusulas de Horn, resolución). Los programas son conjuntos de hechos y reglas, y la ejecución se da por **búsqueda y unificación**.

* **Ventajas:**

  * Expresividad declarativa muy alta.
  * Excelente para sistemas expertos e inteligencia artificial simbólica.
  * Permite razonamiento automático.

* **Desventajas:**

  * Bajo rendimiento en problemas intensivos en cómputo.
  * Difícil de integrar con paradigmas imperativos.
  * Menos popular en la industria actual.

* **Ejemplo (Prolog):**

```prolog
padre(juan, maria).
padre(juan, pedro).

hermano(X, Y) :- padre(Z, X), padre(Z, Y), X \= Y.

?- hermano(maria, pedro).
```

---

## Comparativa General

| Paradigma   | Nivel de Abstracción | Estado Mutable  | Expresividad | Casos de Uso                    |
| ----------- | -------------------- | --------------- | ------------ | ------------------------------- |
| Imperativo  | Bajo                 | Sí              | Medio        | Sistemas embebidos, drivers     |
| Declarativo | Alto                 | No (idealmente) | Alto         | Consultas, IA, reglas           |
| OOP         | Medio-Alto           | Sí              | Alto         | Software empresarial, UI        |
| Funcional   | Alto                 | No              | Muy alto     | Concurrente, Big Data, IA       |
| Lógico      | Muy alto             | No              | Muy alto     | Sistemas expertos, razonamiento |

---

**Ningún paradigma es universalmente mejor**:

* El **imperativo** es cercano al hardware y eficiente.
* El **declarativo** favorece expresividad y optimización automática.
* El **OOP** organiza la complejidad en dominios reales.
* El **funcional** promueve corrección y concurrencia.
* El **lógico** destaca en inferencia y sistemas expertos.


---
