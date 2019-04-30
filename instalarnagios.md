
# Proyecto IDP NAGIOS #
=======================
## INSTALACIÓN NAGIOS ##

###PASO 1 Prerrequisitos###
Nuestro proyecto esta echo en linux,para la utilización del software de monitorización nagios en este sistema operativo necesitaremos lo siguiente

	- Apache
	- PHP
	- GCC:librerias de desarrollo y compilación>
	- GD:librerías de desarrollo

  
![Por tanto comenzamos con la instalación de **APACHE** mediante el comando apt-get install](imagenes/instalacionNAGIOS-1.png)
  

![Instalamos **PHP** mediante el comando apt-get install](imagenes/instalacionNAGIOS-2.png)

  
![Instalamos **GCC** mediante el comando apt-get install](imagenes/instalacionNAGIOS-3.png)

Instalamos **GD** (version 7.10) Mediante el comando **sudo apt-get install libgd2-xpm-dev**

###PASO 2 Crear informacion de cuenta de usuario###

A partir de aqui todo lo tenemos que hacer como root, lo primero que haremos sera lo siguiente:

![Creamos una nueva cuenta de usuario llamada "nagios"](imagenes/instalacionNAGIOS-4.png)

![Le asignamos contraseña a dicho usuario](imagenes/instalacionNAGIOS-5.png)

Antes de la version 6.01 debemos crear un grupo llamado nagios, pero como nosotros utilizamos la versión 7.10 ya ubuntu nos crea el grupo directamente.

![Como ya tenemos el grupo creado procedemos a meter directamente el usuario que creamos enates en el grupo nagios](imagenes/instalacionNAGIOS-6.png)

![Creamos el grupo nagcmd ya que tambien nos hara falta y meteremos al usuario dentro de este](imagenes/instalacionNAGIOS-7.png)

![Metemos al usuario de apache **www-data** en el grupo nagcmd, esto lo hacemos por que la aplicación necesita estar dentro de este grupo para hacer sus gestiones](imagenes/instalacionNAGIOS-8.png)

###PASO 3 Compilación e instalación de Nagios en Ubuntu###

![Procedemos a descargarnos los paquetes nagios, en nuestro caso los almacenaremos en /home/alumnonagios](instalacionNAGIOS-9.png)

![Los paquetes que hemos descargados estan comprimidos, por tanto procedemos a descomprimirlos](instalacionNAGIOS-10.png)

![Ejecutamos el scrip de configuración de Nagios indicandole el nombre del grupo que creamos anteriormente](imagenes/instalacionNAGIOS-11.png)

![Compilamos el código fuente de Nagios](imagenes/instalacionNAGIOS-12.png)

![Instalamos los archivos binarios de Nagios](imagenes/instalacionNAGIOS-13.png)

![A continuación instalamos otros scripts y configuraciones que nos serviran mas tarde(instalamos script de inicio)](imagenes/instalacionNAGIOS-14.png)

![Instalamos ejemplos de ficheros de configuración](imagenes/instalacionNAGIOS-15.png)

![Damos permisos al directorio de comandos externos](imagenes/instalacionNAGIOS-16.png)

###PASO 4 Personalización de la configuración###

![Una vez instalado Nagios en nuestro sistema Ubuntu lo que nos queda por hacer es la configuración, en primer lugar modificaremos la dirección de e-mail que usaremos para las notificaciones de Nagios, para esto abriremos el siguiente fichero mediante un editor de texto(/usr/local/nagios/etc/objects/contacts.cfg)](imagenes/instalacionNAGIOS-17.png)