# <center>**PROYECTO II**</center>
![Logo UMG](/Imagenes/LOGO.png)
1. Sayan Danery Aguirre Guzmàn   |     *7690-17-7987*

2. Jitzon Aldahir Mendez Gonzalez   |    *7690-17-8955*

3. Nelson Steven Cifuentes Chilin   |    *7690-17-2711*


### <CENTER>*SEGURIDAD Y AUDITORIA DE SISTEMAS | 15/10/2021*</CENTER>
### <CENTER>*ING. MELVIN CALÍ*</CENTER>
#
# <a name="Active Directory"></a>Active Directory

El proyecto consiste en la creacion de una red que cumpla por lo menos con el siguiente diagrama de red:

![Active Directory](/Imagenes/ActiveDirectory.png)

*1. Red privada (Intranet)*
1. DNS
2. DHCP
3. Servidor de base de datos instalada en Unix
4. Directorio de activos
1. Politicas de usuarios, roles y/o perfiles
5. La red debe contar con al menos los siguientes sistemas operativos (Windows, Gnu/Linux, 
Unix y BSD)
6. Otros que considere necesarios

#

**DIAGRAMA DE INFRAESTRUCTURA**

![Diagrama de Infraestructura](/Imagenes/Diagrama.jpeg)

**INFRAESTRUCTURA FÍSICA**

![Infraestructura Física](/Imagenes/Infraestructura.png)
- Ilustración de la configuración de los dispositivos
1.	Red LAN
2.	Red de Invitados
3.	Servidor DNS y Active Directory
4.	Firewall

*NOTA:* Para todos los dispositivos se utilizo la contraseña: _Temporal01_ esto con fin de demostración, pero se recomienda crear una politica de cambio de contraseña en el primer inicio de sesión.

## *Configuración de Firewall*

Se utilizo Neth Server que dentro de nuestra infraestructura de red está haciendo la función de firewall principal. Neth Server basado en Linux Centos el cual es de uso gratuito. El documento del proyecto no especifica el uso de un firewall, pero se añadió por motivos de seguridad.

*Login Neth Server:*

![Login](/Imagenes/Login.png)

*Dashboard:*

![Dashboard](/Imagenes/Dashboard.png)

*Nombre del Firewall:*

![Nombre Firewall](/Imagenes/NombreFirewall.png)

*Servicios Generales del Firewall:*

![Dashboard](/Imagenes/ServiciosGeneralesF.png)

*Servicios de Red:*

![S. Red](/Imagenes/ServiciosdeRed.png)

*DHCP:*

![DHCP](/Imagenes/DHCP.png)

El DHCP es el encargado de asignar las direcciones a los dispositivos que se conectan a la red. Recomendación dejar desactivada la función de DHCP por despacho de direcciones automáticas.

*DNS:*

![DNS](/Imagenes/DNS.png)

Es el encargado de crear los nombres de dominio para relacionar los nombres con sus direcciones IP.

*Redes:*

![Redes](/Imagenes/REDES.png)

Se crearon 3 Redes. La red verde con la dirección 192.168.10.1 es la Red LAN. La red roja con la dirección 192.168.1.200 es la red WAN que es la que esta conectada con el proveedor de internet. La red azul con la dirección 192.168.0.1 es la red de invitados encargada de proveer internet por medio de wifi a los dispositivos de los invitados.

*Servicios Activos del Firewall:*

![Activos](/Imagenes/ServiciosActivosFirewall.png)

Nota: Se modifico el puerto SMTP el cual estaba en el puerto genérico 25, se cambió al puerto 587.

*Host:*

![Host](/Imagenes/Host.png)

En esta pestaña se le agrega un nombre de referencia a los dispositivos según la ip.

*Host Groups:*

![Host Groups](/Imagenes/HostGroups.png)

Se crean los grupos en donde agrupamos los dispositivos creados anteriormente.

*Firewall Rules:*

![Rules](/Imagenes/FirewallRules.png)

Se crean las reglas de firewall que pueden ser de bloqueo, acceso o restricción. En este caso se le Acepto que los grupos de it, admon y las redes green y blue tuvieran acceso a la red roja que es la red WAN quien da acceso al Internet. En el caso del grupo de celulares que esta como DROP no se le permitió el acceso a la red.
