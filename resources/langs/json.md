JSON (JavaScript Object Notation) es un formato ligero de intercambio de datos, fácil de leer y escribir tanto para humanos como para máquinas. Imagina que necesitas enviar información de una aplicación a otra, por ejemplo, datos de un usuario como su nombre, edad y correo electrónico. JSON te permite empaquetar esta información de forma ordenada para que la otra aplicación, incluso si está escrita en un lenguaje diferente, pueda entenderla.

**1. Estructura Básica:**

JSON se basa en dos estructuras principales:

- **Pares clave-valor:** La información se organiza en pares, donde la "clave" es una cadena de texto (siempre entre comillas dobles) que describe el dato, y el "valor" es el dato en sí. Piensa en ello como un diccionario: `"nombre": "Juan"`. Aquí, "nombre" es la clave y "Juan" es el valor.

- **Colecciones:** JSON utiliza dos tipos de colecciones para agrupar datos:

  - **Objetos:** Se representan con llaves `{}` y contienen una lista de pares clave-valor separados por comas. Un objeto puede representar una entidad, como un usuario:

    ```json
    {
      "nombre": "Juan",
      "edad": 30,
      "correo": "juan@ejemplo.com"
    }
    ```

  - **Arrays (arreglos):** Se representan con corchetes `[]` y contienen una lista ordenada de valores, separados por comas. Los valores pueden ser de cualquier tipo de dato JSON, incluso otros objetos o arrays.

    ```json
    [
      "manzana",
      "banana",
      "naranja"
    ]

     [
         {"nombre": "Juan", "edad":30},
         {"nombre": "Ana", "edad":25}
     ]


    ```

**2. Tipos de Datos:**

JSON soporta los siguientes tipos de datos:

- **String (cadena de texto):** Siempre entre comillas dobles. Ejemplo: `"Hola Mundo"`.
- **Number (número):** Puede ser entero o decimal. Ejemplo: `10`, `3.14`.
- **Boolean (booleano):** `true` o `false`.
- **Null (nulo):** Representa la ausencia de valor.
- **Array (arreglo):** Como se explicó anteriormente.
- **Object (objeto):** Como se explicó anteriormente.

**3. Ejemplo Complejo:**

Veamos un ejemplo que combina objetos y arrays para representar información más compleja:

```json
{
  "nombre": "Juan",
  "edad": 30,
  "direccion": {
    "calle": "Principal",
    "numero": 123
  },
  "telefonos": [
    { "tipo": "casa", "numero": "555-1234" },
    { "tipo": "movil", "numero": "555-5678" }
  ]
}
```

En este ejemplo, "direccion" y "telefonos" son claves cuyos valores son un objeto y un array, respectivamente.

**4. Usos Comunes:**

- **APIs (Interfaces de Programación de Aplicaciones):** JSON es el formato estándar para el intercambio de datos entre aplicaciones web.
- **Configuración:** Muchos programas utilizan archivos JSON para almacenar configuraciones.
- **Almacenamiento de datos:** Bases de datos NoSQL como MongoDB utilizan JSON para almacenar documentos.

**5. Herramientas:**

Existen muchas herramientas online para validar y formatear JSON, lo que facilita su lectura y depuración. Busca "JSON validator" o "JSON formatter" en tu buscador.
