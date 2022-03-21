## Backend(Python) con Django - Sesion 1

<span style="color: cyan">Para generar un entorno virtual seguimos los siguientes pasos:</span>

1. Pipenv administra las dependencias por proyecto, por lo que es mejor usar Pipenv dentro del directorio de su proyecto. Para instalar paquetes, cambie al directorio de su proyecto y ejecute:
   
       $ cd project 
       $ pipenv install requests

        ![](C:\Users\diana\AppData\Roaming\marktext\images\2022-03-20-14-50-41-image.png)

2. Esto generará dos archivos 
   
   ![](C:\Users\diana\AppData\Roaming\marktext\images\2022-03-20-14-57-00-image.png)
   
   el archivo pipfile mostrara los paquetes que vayamos instalando (django, python 3.10. En este caso)
   
   ![](C:\Users\diana\AppData\Roaming\marktext\images\2022-03-20-15-01-16-image.png)

<span style="color: cyan">Para generar el proyecto:</span>

1.     $ django-admin startproject nameProject

        ![](C:\Users\diana\AppData\Roaming\marktext\images\2022-03-20-15-05-42-image.png)

        Genera un archivo manage.py (Para ver el arbol de directorios los visializamos en             en el VSC)

        ![](C:\Users\diana\AppData\Roaming\marktext\images\2022-03-20-15-26-38-image.png)

2. Configurar zona horaria según su ubicaicón [List of tz database time zones - Wikipedia ](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones). En el archivo settings.py
   
   ![](C:\Users\diana\AppData\Roaming\marktext\images\2022-03-20-16-04-15-image.png)

3. Correr el proyecto (detener el proyecto Ctrl + C)
   
       $ python manage.py runserver 0:8000

4. Realizar migraciones
   
       python manage.py migrate

        ![](C:\Users\diana\AppData\Roaming\marktext\images\2022-03-20-16-10-41-image.png)

5.     Vamos a una nueva pestaña de nuestro navegador, y colocamos *localhost:8000*
   
   ![](C:\Users\diana\AppData\Roaming\marktext\images\2022-03-20-16-17-36-image.png)

6. Administrador
   
   ![](C:\Users\diana\AppData\Roaming\marktext\images\2022-03-20-16-18-57-image.png)

7. Crear un usuario
   
       $ winpty python manage.py createsuperuser

        ![](C:\Users\diana\AppData\Roaming\marktext\images\2022-03-20-16-23-16-image.png)

    Coloque antes el winpty en caso de recibir este mensaje al crear el usuario con la     siguiente sentencia:

     $ python manage.py createsuperuser
    Superuser creation skipped due to not running in a TTY. You can run `manage.py createsuperuser` in your project to create one manually.
    
    

8. Volver a correr el servidor y colocamos nuestros datos del usuario que acabamos de crear y entraremos al adm![](C:\Users\diana\AppData\Roaming\marktext\images\2022-03-20-16-26-47-image.png)

<span style="color: cyan">Crear aplicación</span>

    $ python manage.py startapp app1

![](C:\Users\diana\AppData\Roaming\marktext\images\2022-03-20-16-31-41-image.png)

<span style="color: cyan">Generar tres app</span>

![](C:\Users\diana\AppData\Roaming\marktext\images\2022-03-21-12-19-59-image.png)
