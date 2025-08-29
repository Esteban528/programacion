# Lenguajes en esta guia:

## Lenguaje C

- [Lenguaje C completo](./langs/c.md)

## Javascript

- [Javascript completo](./langs/js.md)

## Python
- [Python completo](./langs/python.md)

## Java
- [Java completo](./langs/java.md)

# Lenguajes de Programación: Definición, Fundamentos y Clasificación Técnica
*Importante leer sino estás familiarizad@ con la definición*

Un **lenguaje de programación** es un **lenguaje formal** diseñado para expresar algoritmos y estructuras de datos de manera precisa, permitiendo que una computadora pueda **interpretar, compilar y ejecutar** dichas instrucciones.

A diferencia de los lenguajes naturales, los lenguajes de programación poseen una **sintaxis estrictamente definida** y una **semántica formal**, lo que garantiza que el significado de un programa sea inequívoco. En términos computacionales, un lenguaje de programación es un **medio de especificación** que conecta el **modelo mental del programador** con el **modelo computacional subyacente** (máquina de Turing, arquitectura de Von Neumann, o modelos alternativos).

---

## Componentes Fundamentales de un Lenguaje de Programación

1. **Sintaxis:**

   * Conjunto de reglas gramaticales que determinan la **estructura válida** de un programa.
   * Se describe mediante **gramáticas formales**, frecuentemente en notación BNF (*Backus–Naur Form*) o EBNF.
   * Ejemplo: En C, `int x = 10;` es una sentencia válida; `int = x 10;` no lo es.

2. **Semántica:**

   * Define el **significado** de las construcciones sintácticas.
   * Se divide en:

     * **Semántica estática:** Reglas que pueden verificarse en tiempo de compilación (tipado, alcance de variables).
     * **Semántica dinámica:** Comportamiento durante la ejecución (efectos sobre memoria, flujo de control, llamadas a funciones).
   * Ejemplo: `x = x + 1;` en C implica leer el valor actual de `x`, sumarle 1 y escribirlo de nuevo en memoria.

3. **Pragmática:**

   * Relacionada con el **uso real** del lenguaje, buenas prácticas y convenciones.
   * Ejemplo: preferir `for-each` en Java cuando se itera sobre colecciones en lugar de un `for` con índices.

4. **Bibliotecas y APIs:**

   * Extienden el lenguaje base con colecciones de funciones, módulos o paquetes reutilizables.
   * Son clave en la productividad, ya que permiten enfocarse en la lógica de negocio en lugar de reinventar algoritmos básicos.

5. **Entorno de Ejecución y Desarrollo:**

   * Incluye **compiladores, intérpretes, entornos de ejecución (VMs)** e **IDEs**.
   * Ejemplo: la **JVM** (Java Virtual Machine) ejecuta bytecode Java, proporcionando portabilidad y seguridad.

---

## Clasificación de los Lenguajes de Programación

### 1. Por Nivel de Abstracción

* **Lenguajes de bajo nivel:**

  * Cercanos al hardware.
  * Ejemplo: **Lenguaje ensamblador**, donde cada instrucción corresponde casi directamente a una instrucción máquina.
* **Lenguajes de alto nivel:**

  * Orientados a la resolución de problemas.
  * Más legibles y expresivos.
  * Ejemplo: **Python, Java, C#**.

> **Observación:** Cuanto más bajo el nivel, mayor control sobre hardware pero menor productividad; cuanto más alto, mayor abstracción pero con pérdida de control fino.

---

### 2. Por Paradigma de Programación

* **Imperativo:** Descripción explícita de pasos a ejecutar (C, Fortran).
* **Declarativo:** Enfoque en *qué* resultado se desea (SQL, Prolog).
* **Orientado a Objetos:** Encapsulación en clases y objetos (Java, C++, C#).
* **Funcional:** Computación como evaluación de funciones (Haskell, Lisp, Scala).
* **Lógico:** Computación como deducción y resolución lógica (Prolog).

---

### 3. Por Propósito

* **De propósito general:** Aplicables a diversos dominios (C, Java, Python).
* **De propósito específico (DSL, *Domain-Specific Languages*):** Diseñados para un área concreta.

  * Ejemplo: **SQL** para bases de datos, **VHDL** para descripción de hardware, **R** para estadística.

---

### 4. Por Forma de Ejecución

* **Lenguajes compilados:**

  * El código fuente se traduce a **código máquina** completo antes de ejecutarse.
  * Ejemplo: **C, C++**.
* **Lenguajes interpretados:**

  * El código se ejecuta instrucción por instrucción en un **intérprete**.
  * Ejemplo: **Python, JavaScript**.
* **Lenguajes híbridos (compilación intermedia):**

  * Se compilan a un bytecode portable que luego es interpretado o compilado en tiempo de ejecución.
  * Ejemplo: **Java (JVM), C# (CLR/.NET)**.

---

## Ejemplos de Lenguajes Relevantes y su Enfoque Técnico

* **C:** Bajo nivel, eficiente, control sobre memoria, ampliamente usado en sistemas operativos y compiladores.
* **C++:** Extiende C con orientación a objetos y metaprogramación. Usado en videojuegos, motores gráficos, software crítico.
* **Java:** Orientado a objetos, portable gracias a la JVM, con un ecosistema robusto para aplicaciones empresariales y móviles.
* **Python:** Interpretado, multiparadigma (imperativo, funcional, orientado a objetos), famoso por su simplicidad y uso en ciencia de datos.
* **JavaScript:** Lenguaje interpretado, esencial en desarrollo web. Evolucionó con Node.js(Bun, deno, etc) para backend.
* **Go (Golang):** Compilado, eficiente en concurrencia, adoptado para sistemas distribuidos y servicios en la nube.
* **Rust:** Compilado, bajo nivel pero seguro, orientado a concurrencia sin *data races*.
* **Swift:** Compilado, optimizado para ecosistema Apple, moderno y seguro.
* **Haskell:** Funcional puro, con evaluación perezosa y tipado estático fuerte.

---

## Consideraciones sobre Elección de Lenguaje

La selección del lenguaje depende de:

* **Rendimiento requerido** (ej. C en sistemas embebidos).
* **Productividad y rapidez de desarrollo** (ej. Python en prototipos de IA).
* **Robustez y escalabilidad** (ej. Java en sistemas empresariales).
* **Concurrencia masiva** (ej. Erlang o Go en telecomunicaciones y microservicios).
* **Seguridad de memoria** (ej. Rust en sistemas críticos).


Un lenguaje de programación no es solo un conjunto de instrucciones para controlar una máquina; es una **abstracción formal que conecta teoría computacional, modelos de ejecución y aplicaciones prácticas**.

La comprensión de sus **componentes formales (sintaxis, semántica, pragmática)** y de su **clasificación técnica** permite al programador elegir con mayor criterio el lenguaje adecuado para cada dominio de aplicación, equilibrando factores como eficiencia, expresividad, seguridad y productividad.

---
