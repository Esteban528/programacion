## Paradigmas de Programación: Una Guía Completa y Sencilla con Ejemplos en Lenguajes Idóneos

Los paradigmas de programación son enfoques fundamentales para la construcción de software. Representan diferentes maneras de pensar y estructurar el código. Cada paradigma tiene sus fortalezas y debilidades, haciéndolo más adecuado para ciertos tipos de aplicaciones. Exploremos los paradigmas más importantes con ejemplos claros en lenguajes que mejor los representan.

**1. Programación Imperativa (C):**

- **Concepto:** Describe paso a paso _cómo_ realizar una tarea, modificando el estado del programa a través de instrucciones secuenciales.

- **Características:**

  - Uso de variables, asignaciones y secuencias de instrucciones.
  - Control de flujo con `if-else`, `for` y `while`.
  - Modificación directa del estado.

- **Ejemplo (C):**

```c
#include <stdio.h>

int main() {
  int suma = 0;
  for (int i = 1; i <= 10; i++) {
    suma += i;
  }
  printf("Suma: %d\n", suma);
  return 0;
}
```

**2. Programación Declarativa (SQL):**

- **Concepto:** Especifica _qué_ resultado se desea obtener sin detallar los pasos exactos.

- **Características:**

  - Énfasis en la descripción del resultado.
  - Uso de consultas y expresiones.
  - Minimiza los efectos secundarios.

- **Ejemplo (SQL):**

```sql
SELECT SUM(numero)
FROM tabla_numeros
WHERE numero BETWEEN 1 AND 10;
```

**3. Programación Orientada a Objetos (Java):**

- **Concepto:** Organiza el código en torno a "objetos" que encapsulan datos (atributos) y comportamiento (métodos).

- **Características:**

  - Abstracción, encapsulación, herencia y polimorfismo.
  - Creación de clases y objetos.
  - Interacción entre objetos mediante mensajes.

- **Ejemplo (Java):**

```java
public class Perro {
    String nombre;
    String raza;

    public Perro(String nombre, String raza) {
        this.nombre = nombre;
        this.raza = raza;
    }

    public void ladrar() {
        System.out.println("Guau!");
    }

    public static void main(String[] args) {
        Perro miPerro = new Perro("Fido", "Labrador");
        miPerro.ladrar();
    }
}
```

**4. Programación Funcional (Haskell):**

- **Concepto:** Trata la computación como la evaluación de funciones matemáticas, evitando cambios de estado y datos mutables.

- **Características:**

  - Funciones puras sin efectos secundarios.
  - Funciones de orden superior.
  - Inmutabilidad.

- **Ejemplo (Haskell):**

```haskell
dobles :: [Int] -> [Int]
dobles = map (*2)

main :: IO ()
main = print (dobles [1, 2, 3, 4])
```

**5. Programación Lógica (Prolog):**

- **Concepto:** Se basa en la lógica formal y la deducción. Define reglas y hechos, y el sistema infiere nuevas conclusiones.

- **Ejemplo (Prolog):**

```prolog
% Hechos
padre(juan, maria).
padre(juan, pedro).

% Regla
hermano(X, Y) :- padre(Z, X), padre(Z, Y), X \= Y.

% Consulta: ¿Son María y Pedro hermanos?
?- hermano(maria, pedro).
```

Cada paradigma ofrece una perspectiva única. La elección del paradigma adecuado depende del problema, las preferencias del programador y las restricciones del proyecto. Comprender las diferencias entre estos paradigmas es clave para un desarrollo de software eficiente y mantenible. Utilizar el lenguaje más adecuado para cada paradigma ayuda a ilustrar sus principios y ventajas de manera más efectiva.
