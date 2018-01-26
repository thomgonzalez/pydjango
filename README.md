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

