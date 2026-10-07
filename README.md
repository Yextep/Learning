# Learning

Colección de ejercicios y pequeños programas para aprender C. El material está organizado en [`C/`](C/), con 28 carpetas numeradas de `Assignment-01` a `Assignment-28`. Cada ejercicio tiene su propio README con el planteamiento y, en la mayoría de los casos, uno o más archivos de código.

## Contenido

| Ejercicios | Temas presentes en el material |
| --- | --- |
| 01–06 | Salida por terminal, tipos de datos, entrada de usuario, operaciones aritméticas y condiciones |
| 07–09 | Fórmula cuadrática, comprobación de rangos y argumentos de línea de comandos |
| 10–13 | Arrays, bucles, cálculo de promedios, simulación de monedas y arrays bidimensionales |
| 14–19 | Punteros, direcciones de memoria, funciones, cadenas terminadas en cero y reserva dinámica de memoria |
| 20–23 | Estructuras, arrays de estructuras y acceso a miembros mediante punteros |
| 24–25 | Operaciones de archivo mediante `open`, `write` y `close` |
| 26 | Ejemplo de programación de sockets que conecta una shell a un puerto TCP |
| 27–28 | Bibliotecas compartidas, interceptación de funciones y ejemplos de técnicas de rootkits de espacio de usuario |

El ejercicio 18 presenta sus ejemplos de código dentro de su [`README`](C/Assignment-18/README.md). El ejercicio 3 incluye una solución adicional en `assignment3-extra.c`.

## Organización

```text
C/
├── Readme.md
├── Assignment-01/
│   ├── README.md
│   └── helloworld.c
├── Assignment-02/
│   ├── README.md
│   └── assignment2.c
├── ...
└── Assignment-28/
    ├── README.md
    └── assignment28.c
```

La [introducción existente a C](C/Readme.md) recomienda intentar cada tarea antes de consultar la solución.

## Requisitos y compilación

Necesitas un compilador de C, como GCC o Clang. Los ejercicios que emplean cabeceras POSIX/Linux, sockets o carga dinámica de bibliotecas requieren un entorno que proporcione esas interfaces.

Cada ejemplo se compila por separado; el repositorio no incluye un sistema de compilación común. Desde la raíz del repositorio, este primer ejercicio puede compilarse y ejecutarse así:

```bash
gcc -Wall -Wextra C/Assignment-01/helloworld.c -o /tmp/learning-hello
/tmp/learning-hello
```

Salida esperada:

```text
Hello, World!
```

Otro ejemplo muestra argumentos de línea de comandos:

```bash
gcc -Wall -Wextra C/Assignment-09/assignment9.c -o /tmp/learning-greeting
/tmp/learning-greeting Ana Garcia
```

Consulta el README de cada carpeta para conocer el enunciado y las particularidades del ejercicio. Los ejemplos de bibliotecas compartidas necesitan opciones de compilación distintas de las usadas para un ejecutable simple.

## Alcance del material

La introducción de `C/Readme.md` presenta este repositorio como aprendizaje entre pares y advierte que los ejemplos no deben asumirse correctos o robustos. Algunos programas tienen limitaciones en la validación de entradas y la portabilidad, por lo que conviene leer el código y las advertencias del compilador.

Los ejercicios de sockets y de interceptación de funciones incluyen comportamientos que afectan al sistema o exponen una shell. Su estudio y ejecución corresponden a un laboratorio aislado y autorizado, de acuerdo con el enfoque educativo indicado en el material.
