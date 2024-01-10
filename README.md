# Cisco-Packet-Tracer
compilation of my projects on cisco packet tracer

PROYECTO DE RED FUNCIONAL CON SERVICIO DE REDUNDANCIA.
1. Diseño de la red
2. Configuraciones básicas para todos los dispositivos aplicando ssh en los routers y los switches.
3. VLANs configurando a todos los equipos y agregando modo trunk en los puertos 12 y 13.
4. Switchport-security.
5. Subnnetting e Ip addressing.
6. OSPF en los routers y switches.
7. IP Statica para el cuarto de servidores.
Manual de Proyecto
48. DHCP Sserver configuraciones.
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
Manual de Proyecto

5Core Switches.- Los switches de capa 3 se espera que hagan tanto las funcionalidades de
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
