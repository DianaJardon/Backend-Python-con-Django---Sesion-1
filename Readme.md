## Backend(Python) con Django - Sesion 1

<span style="color: cyan">Para generar un entorno virtual seguimos los siguientes pasos:</span>

1. Pipenv administra las dependencias por proyecto, por lo que es mejor usar Pipenv dentro del directorio de su proyecto. Para instalar paquetes, cambie al directorio de su proyecto y ejecute:
   
       $ cd project 
       $ pipenv install requests

  ![Aliados](img/1.PNG)

2. Esto generará dos archivos 
   
   ![Aliados](img/2.PNG)
   
   el archivo pipfile mostrara los paquetes que vayamos instalando (django, python 3.10. En este caso)
   
   ![aliados](img/3.PNG)

<span style="color: cyan">Para generar el proyecto:</span>

1.     $ django-admin startproject nameProject

        ![aliados](img/4.PNG)

        Genera un archivo manage.py (Para ver el arbol de directorios los visializamos en en el VSC)

        ![aliados](img/5.PNG)

2. Configurar zona horaria según su ubicaicón [List of tz database time zones - Wikipedia ](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones). En el archivo settings.py
   
   ![aliados](img/6.PNG)

3. Correr el proyecto (detener el proyecto Ctrl + C)
   
       $ python manage.py runserver 0:8000

4. Realizar migraciones
   
       python manage.py migrate

        ![aliados](img/7.PNG)

5.     Vamos a una nueva pestaña de nuestro navegador, y colocamos *localhost:8000*
   
   ![aliados](img/8.PNG)

6. Administrador
   
   ![aliados](img/9.PNG)

7. Crear un usuario
   
       $ winpty python manage.py createsuperuser

        ![aliados](img/10.PNG)

    Coloque antes el winpty en caso de recibir este mensaje al crear el usuario con la     siguiente sentencia:

     $ python manage.py createsuperuser
    Superuser creation skipped due to not running in a TTY. You can run `manage.py createsuperuser` in your project to create one manually.
    
    

8. Volver a correr el servidor y colocamos nuestros datos del usuario que acabamos de crear y entraremos al adm
![aliados](img/11.PNG)

<span style="color: cyan">Crear aplicación</span>

    $ python manage.py startapp app1

![aliados](img/12.PNG)
<span style="color: cyan">Generar tres app</span>

![aliados](img/13.PNG)