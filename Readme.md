## Proyecto de Entrada/Salida en ensamblador M68000
Consiste en crear un controlador de Entrada/Salida para una DUART utilizando el ensamblador del procesador 68k de Motorola 

## Autores
- Álvaro Cabo [@alvarocabo](https://github.com/alvarocabo)
- Pablo Fernández [@pablofdegracia](https://github.com/pablofdegracia)

### Índice
1. [Disclaimer](#Disclaimer)
2. [Descripción del proyecto](#Descripción)
3. [Modo de trabajo](#modo-de-trabajo)

## Disclaimer
La publicación de nuestro proyecto tiene como objetivo *dar a los futuros estudiantes las guías que hemos echado en falta a la hora de realizar el trabajo*. 
> En caso de copia del proyecto saltará el sistema de copias.

- Calificación del proyecto

<img src="https://user-images.githubusercontent.com/74014545/183302730-742d07aa-06ed-4ab4-95bd-3b871a0789ae.png" width="350" height="150"/>


## Descripción

Toda la información del proyecto se encuentra en la [documentación](https://github.com/alvarocabo/UPM/blob/main/Proyecto%20Arquitectura/doc/manual%2068000.pdf) proporcionada para este por parte de la universidad.

En él encontará un manual con la sintaxis del 68k, como las instrucciones de instalación del simulador BSVC en cualquier distribución de linux *(Muy recomendable desde mi experiencia)*

* En este repositorio existe un apartado de [Utilidades](https://github.com/alvarocabo/UPM/tree/main/Proyecto%20Arquitectura/Utilidades) que incluye elementos de creación nuestra para facilitar el testing, además de ejemplos de programas creados en ensamblador.

* El archivo *codigo_pruebas.s* contiene pruebas realidas por el usuario @svg153 y que han sido adaptadas para funcionar con la librería auxiliar, en su [repositorio](https://github.com/svg153/AC_proyecto.2015b) puede encontrar tanto las pruebas originales como su modo de empleo, que consiste en importar el archivo al final de nuestro es_int.s y hacer JMP a la prueba que necesitemos.
> Tener en cuenta que el numero de prueba no coincide con las actuales

## Modo de trabajo

* Para trabajar este proyecto utilizamos un entorno Ubuntu en el que instalamos el simulador siguiendo las instrucciones del manual.
* Para compilar los archivos y depurar utilizabamos el script [Garquiscript.sh](https://github.com/alvarocabo/UPM/blob/main/Proyecto%20Arquitectura/Utilidades/garquiscript.sh) del usuario [@MrGarri](https://github.com/MrGarri/Garquiscript)

**IMP**: Para depurar recomendamos usar el PPAL que viene en la documentación para SCAN y además usar el comando PEA (CADENA DE CHARS) para depurar el PRINT

- Ejemplo de una prueba de PRINT:

<img src="https://user-images.githubusercontent.com/74014545/183303857-c3bdf85a-1586-45be-9f1f-a42b2bb1a276.png" width="450" height="100"/>

<img src="https://user-images.githubusercontent.com/74014545/183303877-beb9f562-228f-4b95-ad33-8187b6306763.png" width="450" height="100"/>

Por último, recomendamos usar el archivo adicional que permite descargar el gestor de prácticas después de cada corrección para una mejor depuración de código.

