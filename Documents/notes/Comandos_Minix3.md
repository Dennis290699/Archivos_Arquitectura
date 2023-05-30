<div align="center">
  <h1 id="Comandos_Minix3">Comandos Minix</h1>
</div>

<p>
MINIX es un sistema operativo basado en Unix, por lo que muchos de los comandos disponibles en MINIX son similares a los que se encuentran en otros sistemas Unix y Linux. Aquí tienes una breve descripción de algunos comandos comunes en MINIX:

- `ls`: Lista los archivos y directorios en el directorio actual.
- `cd`: Cambia el directorio actual a otro directorio especificado.
- `mkdir`: Crea un nuevo directorio.
- `rm`: Elimina archivos y directorios.
- `cp`: Copia archivos y directorios.
- `mv`: Mueve o renombra archivos y directorios.
- `cat`: Muestra el contenido de un archivo en la salida estándar.
- `vi`: Un editor de texto en modo texto que te permite crear y editar archivos de texto.
- `chmod`: Cambia los permisos de archivos y directorios.
- `chown`: Cambia el propietario de archivos y directorios.
- `ps`: Muestra los procesos en ejecución en el sistema.
- `kill`: Envía una señal a un proceso para terminarlo.
- `ifconfig`: Muestra y configura la información de red, como direcciones IP y configuración de interfaces de red.
- `ping`: Envía paquetes de prueba a una dirección IP para verificar la conectividad de red.
- `ssh`: Inicia una sesión remota segura en otro sistema utilizando el protocolo SSH (Secure Shell).
- `scp`: Copia archivos de forma segura entre sistemas a través del protocolo SSH.

Estos son solo algunos de los comandos disponibles en MINIX. Existen muchos otros comandos que ofrecen diversas funcionalidades y permiten administrar y trabajar con el sistema operativo. Puedes consultar la documentación oficial de MINIX para obtener más información sobre los comandos y su uso específico en MINIX.

## Crear directorio y archivos en MINIX3

1. Crear el directorio "DennisTrujillo":

   ```
   mkdir DennisTrujillo
   ```

2. Ingresar al directorio "DennisTrujillo":

   ```
   cd DennisTrujillo
   ```

3. Verificar la ruta actual:

   ```
   pwd
   ```

4. Listar los archivos en el directorio:

   ```
   ls
   ```

5. Crear el archivo "Archivo1.txt":

   ```
   touch Archivo1.txt
   ```

6. Listar los archivos para verificar la creación:

   ```
   ls
   ```

7. Crear el archivo "Archivo2.txt":

   ```
   touch Archivo2.txt
   ```

8. Listar los archivos para verificar la creación:

   ```
   ls
   ```

9. Abrir el archivo "Archivo1.txt" con el editor Vi:

   ```
   vi Archivo1.txt
   ```

10. Dentro de Vi, presionar la tecla "i" para entrar en el modo de inserción. Luego, escribir el texto "Estoy dentro del Archivo1". Presionar la tecla "Esc" y luego escribir ":wq" para guardar y salir del editor. Para visualizar basta volver escribir el comando del punto 10 Presionar "Esc" y luego escribir ":wq" para salir del editor.

11. Guardar la información de red en el archivo "Archivo3.txt":

    ```
    ifconfig > Archivo3.txt
    ```

12. Verificar la ruta actual:

    ```
    pwd
    ```

13. Listar los archivos para verificar la creación de "Archivo3.txt":

    ```
    ls
    ```

14. Eliminar el archivo "Archivo2.txt":

    ```
    rm Archivo2.txt
    ```

15. Listar los archivos para verificar la eliminación de "Archivo2.txt":

    ```
    ls
    ```

16. Mover el archivo "Archivo3.txt" y cambiarle el nombre a "Archivo2.txt":

    ```
    mv Archivo3.txt Archivo2.txt
    ```

17. Listar los archivos para verificar la modificación:

    ```
    ls
    ```
