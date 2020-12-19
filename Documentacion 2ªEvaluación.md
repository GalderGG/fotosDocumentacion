# Documentación 2ª evaluación

**¿Qué es y para qué sirve EC2?**

Es un servicio web de AWS que proporciona capacidad informática en la nube de forma segura.

**Imagen de cómo está creada la instancia y cómo has accedido a ella mediante un cliente ssh**

![](https://github.com/GalderGG/fotosDocumentacion/blob/master/13.png?raw=true)

![](https://github.com/GalderGG/fotosDocumentacion/blob/master/15.png?raw=true)

![](https://github.com/GalderGG/fotosDocumentacion/blob/master/16.png?raw=true)

<hr>

**Imagen del estado de cada aplicación lanzada. En el caso de apache2, comprobación de apache lanzado en el navegador**

APACHE:<br>
![](https://github.com/GalderGG/fotosDocumentacion/blob/master/29.png?raw=true)<br>
![](https://github.com/GalderGG/fotosDocumentacion/blob/master/35.png?raw=true)

Para poder verlo tenemos que habilitar el puerto 80<br>
![](https://github.com/GalderGG/fotosDocumentacion/blob/master/20.png?raw=true)

MYSQL:<br>
![](https://github.com/GalderGG/fotosDocumentacion/blob/master/24.png?raw=true)

PHP:<br>
![](https://github.com/GalderGG/fotosDocumentacion/blob/master/26.png?raw=true)

FTP:<br>
![](https://github.com/GalderGG/fotosDocumentacion/blob/master/28.png?raw=true)

<hr>

**¿Qué es y para qué sirve una IP Elástica?**<br>

Una dirección IP elástica es una dirección IP estatica pública y sirve para tener acceso desde Internet.

**Imagen de cómo has asociado la IP elástica a tu instancia**<br>
Lo primero tenemos que hacer es asignarnos un IP elastica<br>
![](https://github.com/GalderGG/fotosDocumentacion/blob/master/31.png?raw=true)

Una vez que tenemos la IP elastica asignada tenemos que asociarla con la instancia<br>
![](https://github.com/GalderGG/fotosDocumentacion/blob/master/33.png?raw=true)

<hr>

**¿Qué es y para qué sirve el DNS?**

Es un sistema de bases de datos distribuidas en la red con la función principal de traducir la solicitud de ciertos nombres a IPs y al reves.

**Indica cuales son y para qué se usan los diferentes tipos de registros DNS** <br>

A = Este registro se usa para traducir nombres de servidores de alojamiento a direcciones IPv4.

AAAA = Este registro se usa en IPv6 para traducir nombres de hosts a direcciones IPv6.

CNAME = Se usa para crear nombres de servidores de alojamiento adicionales, o alias, para los servidores de alojamiento de un dominio. 

NS = Define la asociación que existe entre un nombre de dominio y los servidores de nombres que almacenan la información de dicho dominio.

MX = Asocia un nombre de dominio a una lista de servidores de intercambio de correo para ese dominio. 

TXT = Los registros TXT contienen información de texto de fuentes externas a tu dominio y que puedes añadir a su configuración.

PTR = Funciona a la inversa del registro A, traduciendo IPs en nombres de dominio. Se usa en el archivo de configuración de la zona DNS inversa.

SOA = Proporciona información sobre el servidor DNS primario de la zona.

SRV = Service record.

**Imagen de los registros DNS de tu sitio en Guebs y explicación de los registros de tu dominio**
![](https://github.com/GalderGG/fotosDocumentacion/blob/master/34.png?raw=true)

1.- La IP del dominio

2.- Es el nombre asociado a la dirección de mail

3.- Sirve para dar seguridad al correo electrónico.

<hr>

**¿Cuántos servidores DNS existen?**

Hay muchos servidores DNS pero los trece principales son los siguientes:<br>
a.root-servers.net<br>
b.root-servers.net<br>
c.root-servers.net<br>
d.root-servers.net<br>
e.root-servers.net<br>
f.root-servers.net<br>
g.root-servers.net<br>
h.root-servers.net<br>
i.root-servers.net<br>
j.root-servers.net<br>
k.root-servers.net<br>
l.root-servers.net<br>
m.root-servers.net<br>

**¿Cuántas redirecciones DNS son posibles?**

Todas las que haga falta hasta que encuentre respuesta.

**¿Qué son los servidores DNS Raíz?**

Son el primer paso en la resolución de los nombres de host legibles en direcciones IP que se utilizan en la comunicación entre los hosts de Internet.

**¿Para qué montar un servidor si simplemente escribiendo en un fichero la relación IP/Nombre el sistema ya funcionaría?**

Porque de esa manera solo funcionaria en nuestro equipo y nos interesa que funcione en todos.

**Según lo expuesto, y si en tu configuración de red del sistema operativo solamente posees un servidor DNS, entonces: ¿cuál sería el proceso para encontrar la IP de la dirección web: http://www.debian.org/distrib/netinst?**

1.- El primer paso es mirar si lo tiene guardado en la cache, de ser asi simplemente devuelve la IP.

2.- Si no lo encuentra hace una peticion Servidor DNS primario.

3.- En caso de que no lo tenga preguntara hasta que lo encuentre o llegue al servidor root.

4.- El servidor root le respondera con con la dirección IP del dominio superior .org.

5.- Ahora que el DNS Primario tiene la dirección IP hara la peticion a debian.org.

6.- Por ultimo el DNS Primario nos respondera con la IP solicitada.

**¿Es posible si dispones de una conexión a Internet con IP dinámica ofrecer servicios en Internet? Es decir, si quieres ofrecer los servicios SND, no dispones de IP estática, esto es, cada vez que te conectas a Internet tu IP, aunque a veces sea la misma, no siempre es la misma.**

Si que es posible pero no es viable, porque cada vez que nos conectasemos a Internet nuestra IP cambiaria, tendriamos que especificar cada vez que cambiamos la IP.

**¿Qué es ICANN?**

Es una corporacion que se ocupa de que a cada dominio se le asigne la dirección IP correcta y, de este modo, no se repita.
