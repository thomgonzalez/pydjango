# pydjango
Development environment 

Herramientas de instalación y gestión.
--------------------------------------

# Pip
Es un sistema usado para instalar y gestionar paquetes de software desarrollados en Python. Una lista de todos los paquetes que gestiona el manejador, se pueden encontrar en el índex de paquetes de Python (PyPI). 

Como instalar esta herramienta en los diferentes sistemas operativos: 

Mac y Linux
```git
$ easy_install pip
```
Windows
```git
c:\Python27\Scripts\easy_install.exe pip
```

# Virtualenv
Es una herramienta que nos permite crear entornos virtuales para Python. Proporcionándonos un gran número de posibilidades, que van desde realizar test, probar la integración de un módulo con distintas versiones, hasta realizar despliegues web. 
Una vez que Pip haya sido instalado en la máquina, instalar cualquier otro módulo del índex de paquetes de Python será mucho más
fácil. 

Mac y Linux
```git
$ pip install virtualenv
```
Windows
```git
c:\Python27\Scripts\pip.exe install virtualenv
```
Crear un ambiente de desarrollo virtual.
```git
$ virtualenv --no-site-packages test
```
# Django
Django es un framework para aplicaciones web gratuito y open source, escrito en Python. Es un WEB framework - un conjunto de componentes que te ayudan a desarrollar sitios web más fácil y rápidamente.

Una vez que tengamos listo nuestro ambiente virtual, podemos proceder e instalar Django de la siguiente manera: 
```git
$ pip install django
```

Como usar Django
----------------
Lo primero que necesitamos hacer es crear un nuevo proyecto, para ello vamos a usar la siguiente línea de comando: 
```git
django-admin.py startproject test_web
```
Correr el servidor para comprobar que nuestro proyecto se pueda navegar en un explorador. Lo hacemos con el siguiente comando 'runserver': 
```git
$ python manage.py runserver
```

Para detener el servidor lo único que tenemos que hacer es presionar Ctrl + C. 
Por último, veamos como desactivar el ambiente virtual de desarrollo. Para detener o desactivar el ambiente lo único que tenemos que hacer es tipear el siguiente comando: 

```git
$ deactivate
```

Crear app Django.
```git
python manage.py startapp principal
```
Migraciones
-----------
Las migraciones son la forma en que Django propaga los cambios que hace a sus modelos (agregando un campo, eliminando un modelo, etc.) en su esquema de base de datos. Están diseñados para ser en su mayoría automáticos, pero necesitará saber cuándo realizar migraciones, cuándo ejecutarlos y los problemas comunes con los que se puede encontrar.

```git
$ python manage.py migrate
Operations to perform:
  Synchronize unmigrated apps: staticfiles, messages
  Apply all migrations: admin, auth, sessions, contenttypes
Synchronizing apps without migrations:
  Creating tables...
    Running deferred SQL...
  Installing custom SQL...
Running migrations:
  Rendering model states... DONE
  Applying contenttypes.0001_initial... OK
  Applying auth.0001_initial... OK
  Applying admin.0001_initial... OK
  Applying contenttypes.0002_remove_content_type_name... OK
  Applying auth.0002_alter_permission_name_max_length... OK
  Applying auth.0003_alter_user_email_max_length... OK
  Applying auth.0004_alter_user_username_opts... OK
  Applying auth.0005_alter_user_last_login_null... OK
  Applying auth.0006_require_contenttypes_0002... OK
  Applying sessions.0001_initial... OK
  ```
Creando un usuario del admin
----------------------------
Primero tendremos que crear un usuario que pueda iniciar sesión en el sitio administrativo. Ejecute el siguiente comando:
```git
$ python manage.py createsuperuser

Username (leave blank to use 'thomgonzalez'): admin
Email address: email@dominio.com
Password:
Password (again):
Superuser created successfully.
```
