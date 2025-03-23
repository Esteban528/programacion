# Python

Python es un lenguaje simple, completo y flexible por lo que tiene muchisimas ventajas. Antes de empezar es importante destacar que es un lenguaje de programación interpretado y principalmente imperativo (Aunque incluye otros paradigmas como POO y programación funcional con lambdas).

Antes de iniciar es importante familiarizarse con algunos conceptos clave. Una vez terminada esta sección se invita al lector a elegir como empezar, se recomienda ver algún curso en la [Sección de cursos](#Cursos) para adentrarse en el tema y luego tomar un [Libro](#Libros) o un [Tutorial](#Recursos) y empezar a profundizar en los conceptos.

> [!TIP]  
> Los recursos que incluyan `python docs` se refiere a la documentación oficial de python, por lo que sino tienes experiencia con documentación es posible que tengas que ver los otros recursos.

## Conceptos clave:

1. **Intérprete**: Python no necesita convertir todo el código en un programa antes de ejecutarlo. En cambio, lee y ejecuta cada línea una por una.

2. **Versiones**: La versión recomendada es **Python 3**. Para ver qué versión tienes instalada, escribe en la terminal:

   ```bash
   python --version
   ```

3. **Código más fácil de leer**: En Python, no es necesario indicar si una variable es un número o un texto. Simplemente se escribe y Python lo entiende.

4. **Uso de espacios en lugar de llaves**: En muchos lenguajes se usan `{}` para agrupar partes del código, pero en Python se usan espacios o tabulaciones obligatorias para hacerlo más claro.

5. **Cómo ejecutar un programa**: Si escribes un programa en un archivo con extensión `.py`, puedes ejecutarlo con:

   ```bash
   python mi_programa.py
   ```

6. **Herramientas adicionales**: Python tiene muchas funciones y herramientas listas para usar, y se pueden agregar más con `pip install`.

7. **Diferentes formas de programar**: Se puede escribir código de varias maneras, como siguiendo pasos uno tras otro (estructurado), organizándolo en objetos (orientado a objetos) o usando funciones matemáticas (funcional).

8. **Pruebas rápidas sin necesidad de archivos**: Puedes escribir código directamente en la terminal de Python sin necesidad de crear un archivo, simplemente ejecutando `python`.

# Recursos principales

> [!NOTE]
> Esto es un espacio de recursos no académico sobre referencias técnicas útiles del lenguaje, por lo que no es necesario estudiarlo como primera opción.

- [Libreria estándar de python](https://docs.python.org/es/3.13/library/index.html)
- [UV - Gestor de proyectos y dependencias](https://github.com/astral-sh/uv)

# Introducción

## Instalación

- [Instalación de python](https://www.python.org/downloads/)

## Recursos

- [Introducción a python en WINDOWS - Microsoft](https://learn.microsoft.com/es-es/windows/python/beginners)
- [Tutorial de python - python docs tutorial](https://docs.python.org/es/3.13/tutorial/index.html) _Recomendado_
- [El manual de python](https://www.freecodecamp.org/espanol/news/el-manual-de-python/)

### Libros

- [Aprende python en un fin de semana (Comprar el libro)](https://www.amazon.com/-/es/Aprende-Python-fin-semana-Spanish/dp/1719884838)
- [Aprende python en un fin de semana (Anna's archive)](https://annas-archive.org/md5/8a2dca284f5c3215cd5cd72146af8eee)

## Cursos

- [Python en 4 horas - FreeCode Camp](https://www.freecodecamp.org/espanol/news/aprende-a-programar-en-python-desde-cero-curso-completo-gratis/)
- [Curso de google - Lectura](https://developers.google.com/edu/python/introduction?hl=es-419)

# Fundamentos

- [Guia básica de funciones](https://www.freecodecamp.org/espanol/news/guia-de-funciones-de-python-con-ejemplos/)
- [Operadores](https://ellibrodepython.com/operadores-python)
- [Bucles - datacamp](https://www.datacamp.com/es/tutorial/loops-python-tutorial)
- [Bucles - learnpython.org](https://www.learnpython.org/es/Loops)
- [Guia completa de funciones](https://ellibrodepython.com/funciones-python)

# Estructuras de datos

- [Estructuras de datos - DataCamp](https://www.datacamp.com/es/tutorial/data-structures-guide-python)
- [Estructuras de datos - python docs](https://docs.python.org/es/3.13/tutorial/datastructures.html)

# Paradigmas de programación

- [Programacion orientada a objetos](https://ellibrodepython.com/programacion-orientada-a-objetos-python)
- [Clases - Python docs](https://docs.python.org/es/3.13/tutorial/classes.html)

- [Programación funcional](https://ellibrodepython.com/programacion-funcional-python)
- [Programación funcional - Python docs](https://docs.python.org/es/3.8/howto/functional.html)

# Paquetes

> [!NOTE] Paquetes y dependencias
> Un paquete o dependencia en un lenguaje de programación es un conjunto de código listo para usar que alguien más ha creado para facilitar el desarrollo de programas.
> En lugar de escribir todo desde cero, puedes instalar y usar estos paquetes para agregar funcionalidades a tu programa, como trabajar con bases de datos, generar gráficos o hacer cálculos matemáticos avanzados.

- [Introducción a los modulos y los entornos virtuales (Venv) - python docs tutorial](https://docs.python.org/es/dev/tutorial/venv.html)
- [Tutorial de pip](https://www.datacamp.com/es/tutorial/pip-python-package-manager)
- [Instalacion de modulos - python docs](https://docs.python.org/es/3.13/installing/index.html)

# Enfoques

Una vez se terminó la introducción a python es hora de buscar un enfoque en el cual empezar a desarrollar aplicaciones en este lenguaje de programación.

- [Awesome python](https://github.com/vinta/awesome-python)

## Desarrollo web

### Frameworks

#### Flask
Flask es un framework ligero y fácil de usar para crear aplicaciones web en Python.

Está diseñado para ser simple y flexible, permitiendo a los desarrolladores construir sitios web y API sin necesidad de configuraciones complejas. A diferencia de otros frameworks más grandes como Django, Flask ofrece solo lo esencial, dejando que el programador agregue las herramientas que necesite.

Algunas características clave de Flask:

- Permite crear servidores web con pocas líneas de código.

- Soporta plantillas HTML con Jinja2.

- Es compatible con bases de datos mediante extensiones.

- Es ideal para proyectos pequeños y medianos.

Recursos

- [Sitio oficial](https://flask.palletsprojects.com/en/stable/)
- [Curso gratuito de flask - codigofacilito](https://codigofacilito.com/cursos/flask)
- [Curso Desarrollo de Aplicaciones Web - CodigoEspinoza](https://www.youtube.com/watch?v=UZIGXkAfAXA&ab_channel=C%C3%B3digoEspinoza-AutomatizatuVida)

#### Django
Django es un framework de Python diseñado para crear aplicaciones web de manera rápida y eficiente. Es más completo que Flask, ya que incluye muchas herramientas listas para usar, como autenticación de usuarios, gestión de bases de datos y administración de contenido.

Django sigue el principio "baterías incluidas", lo que significa que proporciona todo lo necesario para desarrollar una aplicación sin depender de muchas librerías externas. Además, usa el patrón Modelo-Vista-Controlador (MVC), aunque en su documentación se le llama Modelo-Vista-Template (MVT).
Características principales de Django:

- Permite crear aplicaciones web de forma rápida y escalable.

- Incluye un sistema de autenticación y administración de usuarios.

- Tiene un ORM (mapeo objeto-relacional) para manejar bases de datos sin escribir SQL directamente.

- Ofrece un panel de administración automático.

Recursos

- [Sitio oficial](https://www.djangoproject.com/)
- [Tutorial django - Mozilla web docs](https://developer.mozilla.org/es/docs/Learn_web_development/Extensions/Server-side/Django)
- [Curso gratuito django - codigofacilito](https://codigofacilito.com/cursos/django)
- [Django para principiantes - FaztCode](https://www.youtube.com/watch?v=T1intZyhXDU&ab_channel=Fazt)_Recomendado_

## Análisis de datos

- [Exploración y análisis de datos con python - microsoft learn](https://learn.microsoft.com/es-es/training/modules/explore-analyze-data-with-python/)
- [Primeros pasos](https://openwebinars.net/blog/analisis-de-datos-con-python-primeros-pasos-y-consejos/)
- [Data analysis course - freecodecamp](https://www.freecodecamp.org/learn/data-analysis-with-python/)

## Scripting

- [Introducción al scripting y automatizacion - Microsoft learn](https://learn.microsoft.com/es-es/windows/python/scripting)
- [Python scripting - redhat blog](https://www.redhat.com/en/blog/python-scripting-intro)

## Ciberseguridad

La mayoria de recursos en este campo son muy autodidactas o de pago, asi que queda a decisión del usuario

- [Introducción a la ciberseguridad con python](https://ciberseguridad.com/guias/prevencion-proteccion/python/)
- [Python Introducción](https://geekflare.com/es/python-in-cybersecurity/)

## Videojuegos

#### PyGame

- [Curso gratis pygame - codigofacilito](https://codigofacilito.com/cursos/pygame)
- [Curso completo pygame - Codigo espinoza](https://www.youtube.com/watch?v=BUcSWQxY0MI&ab_channel=C%C3%B3digoEspinoza-DesarrollodeVideoJuegos)
