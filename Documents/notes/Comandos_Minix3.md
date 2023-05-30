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

## Errores con el editor Vi en MINIX3
El siguiente boque se detallara como resolver el error en el caso de no encontrar la ruta del editor Vi. Tomar en cuenta que esto se llevara a acabo Post-Instalacion  dentro de VirtualBox. Tomado desde la guia oficial <a href="https://wiki.minix3.org/doku.php?id=usersguide:installingbinarypackages">Click Aqui</a>.

## Instalación de paquetes binarios

### Pkgin

Pkgin es el administrador de paquetes binarios para MINIX 3. Esta página describe cómo usarlo.

### Usando Pkgin

1. Actualización de Pkgin
Este paso se puede volver a ejecutar para actualizar la lista de paquetes.

   ```
   pkgin update
   ```
   Este paso se puede volver a ejecutar para actualizar la lista de paquetes.

2. Si desea instalar un paquete, puede ejecutar:

   ```
   pkgin install git-base
   ```

   ```
   pkgin install binutils
   ```

   ```
   pkgin install clang
   ```
3. Más de uno a la vez:
 
   ```
   pkgin in perl python27
   ```

4. Además, hay una manera de instalar todo:

   ```
   pkgin_all
   ```
   NOTA: Asegúrese de tener suficiente espacio libre si instala todos los paquetes. Probablemente necesitará al menos 25 GB. Pkgin estimará el espacio necesario cuando te pida confirmación.

En caso de persistir los errores consultar la guia de usuario ofiicial <a href="https://wiki.minix3.org/doku.php?id=usersguide:start">Click Aqui</a>.

## Ejemplo practico en MINIX3

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

## Resultados del ejemplo practico en MINIX3

Al finalizar el proceso descrito, los resultados que obtendrás serán los siguientes:

1. Al ejecutar el comando `ls` después de crear el directorio "DennisTrujillo", deberías ver lo siguiente:

   ```
   Archivo1.txt  Archivo2.txt
   ```

2. Después de abrir y editar el archivo "Archivo1.txt" con Vi, el contenido del archivo será:

   ```
   Estoy dentro del Archivo1
   ```

3. Al ejecutar el comando `ls` después de crear el archivo "Archivo2.txt", deberías ver lo siguiente:

   ```
   Archivo1.txt  Archivo2.txt
   ```

4. Al utilizar el comando `ifconfig > Archivo3.txt`, se creará un archivo llamado "Archivo3.txt" que contiene la información de la red.

5. Después de ejecutar el comando `ls`, verás lo siguiente:

   ```
   Archivo1.txt  Archivo2.txt  Archivo3.txt
   ```

6. Al eliminar el archivo "Archivo2.txt" con el comando `rm Archivo2.txt`, ya no estará presente en la lista de archivos al ejecutar `ls`.

7. Luego de usar el comando `mv Archivo3.txt Archivo2.txt`, el archivo "Archivo3.txt" se renombrará a "Archivo2.txt".

8. Al ejecutar `ls` nuevamente, verás lo siguiente:

   ```
   Archivo1.txt  Archivo2.txt
   ```

En resumen, al finalizar el proceso, tendrás el directorio "DennisTrujillo" con el archivo "Archivo1.txt" que contiene el texto "Estoy dentro del Archivo1", y el archivo "Archivo2.txt" que contiene la información de la red.