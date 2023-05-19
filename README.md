<div align="center">
  <h1 style="text-align: center;">Notas</h1>
</div>

## Novedades de actualizacion

- <a href="#archivos-bat">Archivos_bat</a>

<details>
  <summary>Explicacion</summary>
 <pre>
  <h2>
    El fragmento de código realiza una serie de acciones en un entorno de línea de comandos. Aquí está lo que hace paso a paso:

    1. `cd Desktop`: Cambia el directorio actual al escritorio.
    2. `mkdir Dennis_290699`: Crea un nuevo directorio llamado "Dennis_290699" en el escritorio.
    3. `cd Dennis_290699`: Cambia el directorio actual al nuevo directorio "Dennis_290699".
    4. `copy con nuevo_archivo.bat`: Crea un nuevo archivo llamado "nuevo_archivo.bat" utilizando el comando "copy con". Esto abrirá una nueva línea de comandos donde puedes ingresar texto para el archivo.
    5. A continuación, hay una serie de comandos dentro del archivo "nuevo_archivo.bat" recién creado:
       - `@echo off`: Desactiva la visualización de los comandos en la consola mientras se ejecutan.
       - `echo Ejecutando System Info...`: Imprime el texto "Ejecutando System Info..." en la consola.
       - `systeminfo > con`: Ejecuta el comando "systeminfo" y redirige la salida al archivo llamado "con".
       - `echo Ejecutando ipconfig...`: Imprime el texto "Ejecutando ipconfig..." en la consola.
       - `ipconfig >> con`: Ejecuta el comando "ipconfig" y agrega la salida al final del archivo "con".
       - `echo Ejecutando Excel...`: Imprime el texto "Ejecutando Excel..." en la consola.
       - `start excel`: Abre Microsoft Excel en una nueva ventana.
       - `echo Ejecutando Word...`: Imprime el texto "Ejecutando Word..." en la consola.
       - `start winword`: Abre Microsoft Word en una nueva ventana.
       - `@pause`: Pausa la ejecución del archivo hasta que se presione una tecla.
    6. `nuevo_archivo.bat`: Ejecuta el archivo "nuevo_archivo.bat" recién creado.
    7. `echo echo Hola Mundo >> nuevo_archivo.bat`: Agrega el comando "echo Hola Mundo" al final del archivo "nuevo_archivo.bat".

    En resumen, el código crea un nuevo directorio en el escritorio, crea un archivo de lote (batch file) en ese directorio, agrega una serie de comandos al archivo de lote para ejecutar el comando "systeminfo", "ipconfig" y abrir Microsoft Excel y Word, y luego ejecuta el archivo de lote. También agrega una línea adicional al archivo de lote que imprimirá "Hola Mundo" cuando se ejecute nuevamente.
  </h2>
</pre>

</details>

<div align="center">
  <h1 id="archivos-bat">Archivos.bat</h1>
</div>

