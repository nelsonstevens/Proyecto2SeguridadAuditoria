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

#### DISTRIBUCION DE LAS DIRECCIONES IP.

*PERIMETROS FIREWALL:*  

* WAN          192.168.1.200 
* LAN          192.168.10.1
* INVITADOS    192.168.0.1

-DMZ: no fue accesible colocarla por falta de recursos, por lo que nos basamos del lado de la LAN-

*SRV-DOMINIO (UMG-SRVDNSAD)*

* LAN          192.168.10.254

*USUARIOS:*

LAN
* UMG-Sayan
* UMG-Jitzon
* UMG-Nelson

INVITADOS

* UMG-Sayan2
* UMG-Jitzon2
* UMG-Nelson2

*SERVERS*

* FRW
* AD

*GRUPOS*                
* IT
* VENTAS
* ADMON

*RANGOS DE IP:*

DHCP                 
* LAN         192.168.10.100-150
* INVITADOS   192.168.0.100-150

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

## *Configuración del Servidor de Dominio o Active Directory*

Se instalo el Windows server 2019 con las siguientes características:

![Caracteristicas](/Imagenes/CaracteristicasPC.png)

* _Nombre del Dominio:_ **umg.local**

* _Dirección:_ **192.168.10**

*Usuarios y equipos de Active Directory*

![Usuarios y Equipos](/Imagenes/UsuariosEquipos.png)

Se creo estructura simple en el dominio umg.local, con una unidad organizativa principal llamada UMG donde se despliegan los grupos organizativos Admon, IT, Ventas basados en los departamentos correspondientes. Dentro de cada grupo organizativo se crearon dos usuarios, como por ejemplo los que muestra la imagen Tecnico uno y Tecnico dos.

*Administrador de DNS*

![Admin DNS](/Imagenes/AdminDNS.png)

El servidor de DNS al configurarse este ya posee una estructura definida en donde se desglosan la zona directa, zona inversa, puntos de confianza y reenviadores de condiciones.

*Zona de Busqueda Directa*

![Zona de Busqueda Directa](/Imagenes/ZonadeBusquedaDirecta.png)

Aquí se creo la zona de nombre umg.local (la zona del dominio)

*Zona de Busqueda Inversa*

![Zona de Busqueda Inversa](/Imagenes/ZonadeBusquedaInversa.png)

Se le ingreso la IP y automáticamente el sistema genera la IP inversa, esto se hace como protocolo o estándar.

### **Políticas Generales de los Usuarios (GPO)**

Dentro las políticas GPO se tiene contemplado:
* El bloqueo de los puertos USB
* Ocultar el panel de control
* Establecer el titulo de explorador de internet
* Bloquear el ingreso al CMD
* Bloqueo de instalación de programas sin tener un usuario administrador
* Bloqueo de navegación a ciertas páginas
* entre otros.

### **Antivirus**

Para la seguridad del antivirus se tiene contemplado el uso de una consola ESET

![Antivirus](/Imagenes/Antivirus.jpg)

### **Servidor de Actualizaciones WSUS**

Se contempló utilizar Windows Server Update Services (también llamado WSUS), el cual provee actualizaciones de seguridad para los sistemas operativos Microsoft. Mediante Windows Server Update Services.

![WSUS](/Imagenes/WSUS.png)

