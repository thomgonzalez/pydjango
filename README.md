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
