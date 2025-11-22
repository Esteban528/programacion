# Lenguajes de programación

Los lenguajes de programación son la forma en la que nosotros le damos órdenes al computador. Al final todo termina convertido en binario, pero según el tipo de lenguaje esa conversión puede ser más cercana al hardware o más amigable para el programador. Por eso se suelen dividir en lenguajes de bajo nivel y lenguajes de alto nivel según su abstracción.

Los de bajo nivel, como ensamblador o incluso C(realmente es de alto nivel, pero permite el desarrollo de soluciones de baja abstracción con el hardware), están mucho más cerca de cómo funciona la máquina por dentro. Te dan control total, pero son más difíciles de escribir y entender porque te obligan a pensar casi como el hardware. En cambio, los lenguajes de alto nivel —como Python, Java o JavaScript— están hechos para ser más cómodos de leer y trabajar, aunque oculten muchos detalles del sistema y se concentran en la pieza de software que se va a desarrollar.

También se clasifican según cómo se ejecutan: compilados o interpretados.
Un lenguaje compilado convierte todo el código a instrucciones de máquina antes de ejecutarse, lo que hace que los programas sean más rápidos y eficientes; aquí entran C, C++, Go, Rust, etc. Por otro lado, los lenguajes interpretados ejecutan el código línea por línea mediante un intérprete, lo que facilita probar cosas rápido y moverse más ágil, aunque generalmente sacrifican rendimiento; ejemplos serían Python o JavaScript.

Ningún enfoque es mejor que otro; simplemente están pensados para necesidades distintas. Cada uno tiene su lugar dependiendo del tipo de proyecto y del control o rendimiento que se necesite.

# Primer lenguaje

Al terminar las bases para iniciar en la programación tenemos que escoger nuestro primer lenguaje, el cual nos va a servir para continuar con los siguientes temas de estudio y con el que vamos a adquirir experiencia para hacer nuestro primer programa.

Para empezar voy a recomendar 3 lenguajes y sus ventajas.


> [!CAUTION]
> Recuerda instalar un editor de código para poder empezar a programar, segun el lenguaje que elijas puedes escoger entre algo como [Visual Studio Code](https://code.visualstudio.com/), un [IDE](https://aws.amazon.com/es/what-is/ide/) u otro que prefieras

*Estos lenguajes son para empezar, despues segun su panorama favorito deberá escoger el que más se ajuste con su enfoque*

# - [Python](./beginner/python.md)

Ejemplo:
```py
# Funcion
def saludar(nombre):
    if nombre == "":
        return "No ingresaste un nombre."
    else:
        return f"Hola, {nombre}!"

# Programa principal
print("=== Programa de saludo ===")
nombre = input("Escribe tu nombre: ")

mensaje = saludar(nombre)
print(mensaje)

# Ahora un ciclo:
print("\nContando del 1 al 5:")
for i in range(1, 6):
    print(i)
```

**Ventajas**
* Sintaxis simple que separa bloques de código con identación
* Un lenguaje de propósito general con un ecosistema muy amplio
* Similar al pseudocódigo

**Desventajas**
* Es lento (comparado a otros lenguajes de proposito general)
* Puede permitir malas prácticas (muy permisivo).
* Ecosistema fragmentado


## - [C](./beginner/c.md)

Ejemplo:

```c
#include <stdio.h>

// funcion
void saludar(const char *nombre) {
    if (nombre[0] == '\0') {
        printf("No ingresaste un nombre.\n");
    } else {
        printf("Hola, %s!\n", nombre);
    }
}

int main() {
    char nombre[50];

    printf("=== Programa de saludo ===\n");
    printf("Escribe tu nombre: ");
    fgets(nombre, sizeof(nombre), stdin);

    // eliminar salto de línea
    for (int i = 0; nombre[i]; i++)
        if (nombre[i] == '\n') nombre[i] = '\0';

    saludar(nombre);

    // ciclo:
    printf("\nContando del 1 al 5:\n");
    for (int i = 1; i <= 5; i++) {
        printf("%d\n", i);
    }

    return 0;
}
```

**Ventajas**

* Excelente para aprender cómo funciona la memoria y los fundamentos del sistema operativo.
* Base de muchos lenguajes modernos: C++, Java, C#, Go y más.
* Rápido, eficiente y muy útil para comprender bajo nivel.
* Todo lo que aprendes aquí te acompaña toda la carrera.

**Desventajas**

* Gestión manual de memoria: más difícil para principiantes.
* Sintaxis más compleja que Python.
* Más fácil cometer errores difíciles de detectar (segmentation faults, overflows…).

## - [JavaScript](./beginner/javascript.md)

Ejemplo:

```js
// Función
function saludar(nombre) {
    if (nombre === "") {
        return "No ingresaste un nombre.";
    } else {
        return `Hola, ${nombre}!`;
    }
}

// Programa principal (Node.js)
const readline = require("readline").createInterface({
    input: process.stdin,
    output: process.stdout
});

console.log("=== Programa de saludo ===");
readline.question("Escribe tu nombre: ", (nombre) => {
    const mensaje = saludar(nombre);
    console.log(mensaje);

    // Ahora un ciclo:
    console.log("\nContando del 1 al 5:");
    for (let i = 1; i <= 5; i++) {
        console.log(i);
    }

    readline.close();
});
```

**Ventajas**

* El lenguaje más usado en la web: frontend, backend, apps móviles, etc.
* Muy fácil empezar: corre en cualquier navegador o con Node.js.
* Sintaxis flexible y amigable para principiantes.
* Gran ecosistema y comunidad enorme.

**Desventajas**

* Puede permitir malas prácticas (muy permisivo).
* Muchas formas diferentes de hacer lo mismo → confusión inicial.
* La asincronía puede ser difícil al principio.

---

[Inicio](../README.md) 
