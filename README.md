# Cisco-Packet-Tracer
compilation of my projects on cisco packet tracer

PROYECTO DE RED FUNCIONAL CON SERVICIO DE REDUNDANCIA.
REQUERIMIENTOS
Segmentar físicamente la red.
Segmentar lógicamente (subnetting).
Vlan de datos.
Vlan de voz.
Vlan de administración.
Port security al menos dos acciones.
DHCP AGREGAR DNS Y TIEMPO DE CONCESIÓN.
(Necesitamos un router para DHCP que reparta ips a cada router por vlan, si tenemos un
máximo de 4 vlans podemos usar un servidor, en caso de usar por router hay que hacer uso de
IPHELPER, investigar su uso.)
Crear al menos dos servicios en un servidor.
(Necesitamos un VTP server, cliente y transparente aunque raramente se usa el transparente.)
Desarrollar modos VTP en su topología.
Crear dos usuarios para SSH (Admin, usuario restringido).
Enrutamiento (Estático y/o dinámico).
SEGMENTACIÓN FÍSICA DE LA RED.
La segmentación física en redes implica dividir la infraestructura física de la red en segmentos
separados y distintos. Esto se hace mediante la separación física de dispositivos de red, como
switches, routers y cables, para crear redes más pequeñas y manejables.
La segmentación física puede incluir la creación de subredes separadas utilizando dispositivos de
red dedicados, como switches VLAN-capaces, que permiten aislar tráfico en diferentes puertos o
VLANs físicamente separadas. También puede implicar el uso de routers para dividir la red en
dominios de broadcast separados o la implementación de firewalls físicos para controlar el flujo de
datos entre segmentos.
SEGMENTACIÓN LÓGICA (SUBNETTING).
Implica separar los equipos de forma orientada a un mundo real, a modo de acomodar salones u
oficinas.
La segmentación lógica es una técnica utilizada en redes de computadoras para dividir el tráfico de
red en segmentos más pequeños, basados en protocolos o servicios específicos. Implica separar el
Manual de Proyecto 2
flujo de datos en capas superiores del modelo OSI, como la capa de aplicación o la capa de
transporte.
Esta técnica se usa para mejorar el rendimiento, la seguridad y la gestión de la red. Al dividir la red
en segmentos lógicos, se pueden aplicar políticas de seguridad y administración de forma más
eficiente, permitiendo un control más preciso sobre cómo fluyen y se manejan los datos.
VLAN DE DATOS, VOZ Y ADMINISTRACIÓN.
VLAN de datos: Está destinada al tráfico de datos generales. Incluye dispositivos como
computadoras, servidores y dispositivos de almacenamiento conectados a la red para
intercambiar información, correos electrónicos, navegación web, entre otros.
VLAN de voz: Se dedica al tráfico de voz sobre IP (VoIP). Aquí se incluyen dispositivos como
teléfonos IP y sistemas de comunicación de voz. Al separar el tráfico de voz, se puede priorizar
para garantizar calidad y baja latencia en las llamadas.
VLAN de administración: Esta VLAN es para los dispositivos de administración de red, como
switches, routers, puntos de acceso inalámbrico, cámaras de seguridad IP, etc. La segmentación
permite un control más seguro y eficiente de estos dispositivos.
PORT SECURITY
Cuando se habilita el port security en un switch, se pueden configurar reglas para cada puerto, como
la cantidad máxima de direcciones MAC permitidas, las direcciones MAC específicas que pueden
acceder al puerto o la acción a tomar si se detectan direcciones MAC no autorizadas (como
deshabilitar el puerto o enviar una notificación).
Cuando un dispositivo se conecta a una red que utiliza DHCP, el servidor DHCP puede proporcionar
la dirección de uno o más servidores DNS. Estos servidores DNS traducen nombres de dominio a
direcciones IP, permitiendo a los dispositivos acceder a recursos en la red utilizando nombres en
lugar de direcciones IP.
El tiempo de concesión es el período durante el cual un dispositivo tiene asignada una dirección IP
por el servidor DHCP. Este tiempo se especifica en la configuración del servidor DHCP y puede variar
desde unos minutos hasta días o más. Al finalizar el tiempo de concesión, el dispositivo debe renovar
su asignación de dirección IP o liberarla.
SERVICIOS DE SERVIDOR.
1. Servidor DHCP: Puedes configurar un servidor DHCP en un router o switch para asignar
direcciones IP automáticamente a dispositivos en la red.
2. Servidor DNS: Puedes utilizar un servidor DNS para resolver nombres de dominio en
direcciones IP. Puedes configurar esta función en un router o utilizar un servidor dedicado.
Manual de Proyecto 3
3. Servidor Web: Puedes simular un servidor web utilizando un PC o un servidor, configurando
aplicaciones como HTTP Server o FTP Server en el dispositivo para permitir el acceso a páginas
web o transferencias de archivos.
4. Servidor de Archivos: Puedes configurar un PC o un servidor para compartir archivos en la red,
permitiendo a otros dispositivos acceder y almacenar datos en ese servidor.
5. Servidor de Correo Electrónico: Puedes simular un servidor de correo electrónico utilizando un
PC o un servidor y configurando aplicaciones de servidor de correo electrónico como SMTP o
POP3.
VTP EN SU TOPOLOGÍA.
VTP (Protocolo de Trunking VLAN) es utilizado para propagar automáticamente la información de
configuración de VLAN a través de una red. En Packet Tracer, se puede configurar VTP en switches
para propagar información sobre VLAN de manera centralizada.
vtp mode [server/client/transparent] .
SSH (CREACIÓN DE USUARIOS Y CONFIGURACIÓN DE PERMISOS).
En Packet Tracer, la configuración detallada de SSH, la creación de usuarios y la gestión de
permisos no es tan completa como en entornos de red reales o en simuladores más avanzados.
En Packet Tracer, la limitación de la configuración de SSH y la gestión de usuarios se debe a que es
una herramienta de simulación diseñada para ofrecer un entorno básico y educativo de redes. Por lo
tanto, no todas las funcionalidades avanzadas de dispositivos reales están disponibles. Algunas de
las limitaciones incluyen:
1. Complejidad de las características: Herramientas de simulación como Packet Tracer están
diseñadas para proporcionar una representación simplificada de dispositivos de red. Funciones
avanzadas como la gestión de usuarios, la autenticación detallada y las configuraciones
complejas de seguridad (como autorización granular) pueden no estar completamente
implementadas o disponibles.
2. Dispositivos compatibles: No todos los dispositivos en Packet Tracer admiten SSH. En
versiones anteriores, por ejemplo, se incluían modelos de switches y routers específicos que
permitían la configuración de SSH. En versiones más recientes como la 7.9, puede variar, y
algunos switches y routers pueden admitir la configuración de SSH, mientras que otros no.
3. Limitaciones de simulación: Packet Tracer no proporciona todas las funcionalidades que
encontrarías en un entorno de red real. Algunas configuraciones avanzadas, detalles específicos
o características de dispositivos pueden no estar disponibles para ser configuradas o probadas.
ENRUTAMIENTO.
El enrutamiento, ya sea estático o dinámico, se refiere a cómo se determina la mejor ruta para enviar
datos a través de una red. 
Manual de Proyecto 4
Enrutamiento Estático:
Configuración manual: En el enrutamiento estático, los administradores de red configuran
manualmente las rutas en los dispositivos de red. Esto significa que cada ruta debe ser
introducida y mantenida manualmente en cada dispositivo.
Rutas estáticas: Se especifica la ruta exacta hacia una red específica, indicando el próximo
salto (próximo router) que debe utilizarse para alcanzar esa red.
Menos adaptable: No se ajusta automáticamente a cambios en la topología de la red. Si hay
cambios en la red, como la caída de un enlace, el administrador debe actualizar manualmente
las rutas.
Enrutamiento Dinámico:
Automatización: Utiliza protocolos de enrutamiento para intercambiar información de manera
automática entre los dispositivos de red. Los routers intercambian información sobre la red para
determinar la mejor ruta.
Actualización automática: Se ajusta a cambios en la red de manera automática. Cuando se
produce un cambio en la topología de la red, como la caída de un enlace, los routers
intercambian información y recalculan las rutas automáticamente.
Más escalable: Ideal para redes grandes y en constante cambio, ya que reduce la carga
administrativa al adaptarse automáticamente a cambios en la red.
Dada la red, su distancia y pequeña complejidad, usaremos el enrutamiento dinámico ya que es más
adecuado para redes más grandes y dinámicas, donde la automatización y la adaptabilidad son
esenciales.
Se estará trabajando la siguiente dirección de IP:
192.168.20.0/24 para la Data.
10.10.10.0/24 para voz.
192.200.100.0 para IP’s publicas.
PASOS A REALIZAR
1. Diseño de la red
2. Configuraciones básicas para todos los dispositivos aplicando ssh en los routers y los switches.
3. VLANs configurando a todos los equipos y agregando modo trunk en los puertos 12 y 13.
4. Switchport-security.
5. Subnnetting e Ip addressing.
6. OSPF en los routers y switches.
7. IP Statica para el cuarto de servidores.
Manual de Proyecto 5
8. DHCP Sserver configuraciones.
9. Inter-VLAN routing en los switches plus ip dhcp helper addresses.
10. Configuraciones de red inalambrica.
11. Configuración del servicio de telefonía.
12. ACL para SSH.
13. PAT + Access Control List.
14. Site-to-Site IPsec VPN + ACL.
REQUERIMIENTOS
Herramienta de trabajo.- Se usará la herramienta de trabajo Cisco Packet Tracer para diseñar e
implementar las soluciones de Red.
Diseño Jerarquico.- Se usará un diseño jerarquico para proveer redundancia en cada nivel.
ISPs .- Se espera que la red este conectada en almenos 2 IPS’s para proveer redundancia y
permitir la conexión entre cada Router.
Esta arquitectura ofrece tanto redundancia como capacidad de gestión de tráfico para asegurar
la disponibilidad y el rendimiento de la red, lo que es crucial, especialmente en entornos
empresariales donde la conectividad ininterrumpida es fundamental.
Agregación o consolidación de tráfico: Recibe el tráfico de múltiples ubicaciones o
proveedores y lo canaliza hacia un servidor o red central para procesamiento adicional.
Mayor capacidad de procesamiento: Puede manejar grandes volúmenes de tráfico
provenientes de diferentes ubicaciones o proveedores antes de enviarlos a su destino
final.
Redundancia: Si uno de los proveedores de internet falla, el otro puede mantener la
conexión activa, asegurando que la red no se interrumpa por completo.
Balanceo de carga: Distribuir el tráfico entre los proveedores para mantener un mejor
rendimiento o evitar la congestión en una sola conexión.
WIFI.- Cada departeamento necesita de una red inalambrica para permitir la conexión entre
usuarios.
VoIP.- Cada departamente tendra que tener telefonos IP y tendrán que poder comunicarse entre
ellos.
VLAN.- Cada departamento tendrá que estar en su respectiva VLAN y diferente sub-red ajena a
los demás departamentos.
SUBNETTING .- Asignar el numero correcto de direcciones para cada departamento.
CONFIGURACIONES BÁSICAS.- Configurar cosas básicas como el hostname, contraseñas,
mensajes de banner, encriptar contraseñar y deshabilitar IP domain lookup.
Inter-VLAN Routing.- Los dispositivos de cada departamento deben de poder comunicarse unos
con otros con el respectivo switch de capa 3 configurado para ese propósito.
Manual de Proyecto 6
Core Switches.- Los switches de capa 3 se espera que hagan tanto las funcionalidades de
routing como switching y se les asignara una dirección IP.
DHCP Server.- Todos los dispositivos en la red (excepto los telefonos) obtendran una IP de
forma dinamica del servidor dedicado a DHCP.
Cisco Router.- Exigentemente el router debe soportar el servicio de telefonía.
Static Addressing.- Los dispositivos en el “cuarto” de servidor tendrán direcciones IP estáticas.
Servicio de Telefonía.- Se configurará el VoIP en el gateway router.
Routing Protocol.- Se usará OSPF como protocolo de enrutamiento para anunciar rutas tanto
en los routers como en los switches multicapa.
Security Port.- Se buscara que solo un dispositivo este conectado a un puerto de switch,
además se usará el método sticky para obtener las direcciones MAC y poder ofrecer un mejor
modo de violación en modo de shutdown.
SSH.- Se configurará el SSH en todos los routers y los switches correspondientes para el login.
Standart ACL for SSH.- El uso más común es Por ejemplo, podrías configurar un ACL estándar
para SSH en un router o firewall para permitir el tráfico SSH solo desde una dirección IP
específica o un rango de direcciones IP autorizadas, limitando así quién puede acceder a los
dispositivos de red a través de SSH. Esto ayuda a proteger los dispositivos de posibles intentos
de acceso no autorizados o ataques desde direcciones IP no permitidas.
NAT + ACL.- Se configurará el PAT con esa combinación. Esta combinación es útil para
administrar el flujo de datos, proteger la red contra posibles amenazas y definir políticas de
acceso específicas para diferentes tipos de tráfico, todo ello mientras se mantiene la conectividad
eficiente de los dispositivos en la red.
IPsec VPN + ACL.- Se configurará la VPN site-to-site IPsec entre el servidor de sede y el router
border. Esta combinación es útil para administrar el flujo de datos, proteger la red contra posibles
amenazas y definir políticas de acceso específicas para diferentes tipos de tráfico, todo ello
mientras se mantiene la conectividad eficiente de los dispositivos en la red.
Un ejemplo es; ACLs pueden trabajar en conjunto con NAT para permitir o denegar ciertos tipos
de conexiones antes o después del proceso de traducción de direcciones. Por ejemplo, puedes
configurar un ACL para permitir el tráfico SSH solo desde ciertas direcciones IP después de que
se haya realizado la traducción de direcciones utilizando NAT.
