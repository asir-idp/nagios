# Proyecto IDP NAGIOS

## Monitorizacion grafica del nagios desde una maquina servidora real a una maquina cliente real


Nos conectamos desde nuestra maquina cliente a la ip de la maquina servidora en este caso **10.1.1.154** para descargarnos el programa de version cliente para poder monitorizar desde nuestra maquina servidora al PC cliente


En primer lugar introducimos la ip "10.1.1.154" para poder acceder a Nagios.
![](monitorizacion_nagios/1.PNG)

Ahora empezamos la intalación de nagios.
![](monitorizacion_nagios/2.PNG)

Introducimos los datos de nuestra cuenta (nombre de usuario, contraseña, email) y le damos a "finish install" (instalar).
![](monitorizacion_nagios/3.PNG)

Esperamos a que finalice la instalacion.
![](monitorizacion_nagios/4.PNG)

Una vez finalizada la instalación nos da las credenciales con las cuales deberemos acceder a nuestra cuenta. Acto seguido le damos a "iniciar sesión en nagios xi"
![](monitorizacion_nagios/5.PNG)

Ahora accedemos a nuestra cuenta con el usuario y la contraseña que nos facilitaron anteriormente. 
![](monitorizacion_nagios/6.PNG)

Ya estamos dentro de Nagios xi. 
![](monitorizacion_nagios/7.PNG)

Ahora dentro de la página principal pinchamos en "ejecutar un asistente".
![](monitorizacion_nagios/8.PNG)

Ahora nos van a mostrar los diferentes asistentes que hay, nosotros como vamos a monitorizar un windows, tenemos que seleccionar la opción que pone "Windows Desktop".
![](monitorizacion_nagios/9.PNG)

Buscamos la dirección ip del servidor al que nos vamos a conectar, y la introducimos en la casilla de "Dirección IP".
![](monitorizacion_nagios/10.PNG)

Una vez hayamos puesto la dirección ip, descargamos "64-Bit Agente", que es la opción de 64 bits.
![](monitorizacion_nagios/11.PNG)

Ahora procedemos a instalarlo.
![](monitorizacion_nagios/12.PNG)

Luego ponemos la opción "Generic".
![](monitorizacion_nagios/13.PNG)

Ahora nos dice que elijamos el tipo de configuración. Nosotros vamos a elegir la opción "Typical".
![](monitorizacion_nagios/14.PNG)

Le damos a "next" (siguiente).
![](monitorizacion_nagios/15.PNG)

Acto seguido en la casilla de "Password", escribimos nuestra contraseña, que en este caso es "idp1234$".
![](monitorizacion_nagios/16.PNG)

Ahora hacemos clic en "install" y empezará nuestra instalación.
![](monitorizacion_nagios/17.PNG)

Una vez finalizada la instalación le damos a "finish" para completar la instalación de manera correcta.
![](monitorizacion_nagios/18.PNG)

Ahora procedemos a monitorizar el equipo utilizando un programa de benchmarks (heaven benchmarks) para meterle rendimiento al PC Cliente y que nos salten los avisos que configuramos anteriormente

En la primera vemos que no ocurre nada ya que tienen que pasar unos segundos hasta la primera monitorizacion de los componentes del pc cliente 
![](monitorizacion_nagios/19.png)

Aqui ya vemos como el uso de la CPU salta al 52% - Disco duro al 24% y el uso de la RAM al 22%
![](monitorizacion_nagios/20.png)

Y aqui unos minutos mas tarde vemos como el consumo de la CPU - RAM - Disco duro suben de rendimiento
![](monitorizacion_nagios/21.png)
