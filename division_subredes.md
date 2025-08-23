### Un servidor proxy inverso regula y restringe la accesibilidad de Internet a un servidor interno.

Anteriormente en este curso, usted aprendió acerca de la segmentación de red, una técnica de seguridad que divide las redes en secciones. Una red privada puede segmentarse para proteger partes de la red de Internet, que es una red global no segura.

Por ejemplo, usted aprendió sobre la zona no controlada, la zona controlada, la zona desmilitarizada y la zona restringida. No dude en revisar el vídeo sobre las zonas de seguridad

 para refrescar sus conocimientos sobre cómo puede utilizarse la segmentación de red para añadir una capa de seguridad a las operaciones de red de su organización. La creación de zonas de seguridad es un ejemplo de una estrategia de redes denominada división en subredes.
Visión general de la división en subredes

Ladivisión en subredes es la subdivisión de una red en grupos lógicos denominados subredes. Funciona como una red dentro de otra red. La división en subredes divide un rango de direcciones de red en subredes más pequeñas dentro de la red. Estas subredes más pequeñas se forman en función de las direcciones IP y la máscara de red de los dispositivos de la red. La división en subredes crea una red de dispositivos para que funcionen como su propia red. Esto hace que la red sea más eficiente y también puede utilizarse para crear zonas de seguridad. Si los dispositivos de una misma subred se comunican entre sí, el Switch cambia las transmisiones para que permanezcan en la misma subred, lo que mejora la velocidad y la eficacia de las comunicaciones.
Dos subredes para dos redes conectadas a un router.
Notación de enrutamiento entre dominios sin clase para la división en subredes

El direccionamiento entre dominios sin clase (CIDR) es un método de asignación de máscaras de subred a direcciones IP para crear una subred. El direccionamiento sin clase sustituye al direccionamiento con clase. El direccionamiento classful se utilizó en la década de 1980 como sistema de agrupación de direcciones IP en clases (de la Clase A a la Clase E). Cada clase incluía un número limitado de direcciones IP, que se fueron agotando a medida que el número de dispositivos que se conectaban a Internet superaba el rango classful en la década de 1990. El direccionamiento CIDR sin clases amplió el número de direcciones IPv4 disponibles.

CIDR permite a los profesionales de la ciberseguridad segmentar las redes classful en trozos más pequeños. Las direcciones IP CIDR tienen el mismo formato que las direcciones IPv4, pero incluyen una barra oblicua ("/'") seguida de un número al final de la dirección. Este número adicional se denomina prefijo de red IP. Por ejemplo, una dirección IPv4 normal utiliza el formato 198.51.100.0, mientras que una dirección IP CIDR incluiría el prefijo de red IP al final de la dirección, 198.51.100.0/24. Esta dirección CIDR engloba todas las direcciones IP entre 198.51.100.0 y 198.51.100.255. El sistema de direccionamiento CIDR reduce el número de entradas en las tablas de enrutamiento y proporciona más direcciones IP disponibles dentro de las redes. Puede intentar convertir direcciones CIDR a IPv4 y viceversa mediante una herramienta de conversión en línea, como IPAddressGuide

, para practicar y comprender mejor este concepto.

Nota: Puede que aprenda más sobre CIDR durante su carrera, pero no se tratará con mayor profundidad en este programa de certificación. Por ahora, sólo necesita una comprensión básica de este concepto.
Beneficios de seguridad de la división en subredes

La división en subredes permite a los profesionales y analistas de redes crear una red dentro de su propia red sin solicitar otra dirección IP de red a su proveedor de servicios de Internet. Este proceso utiliza el ancho de banda de la red de forma más eficiente y mejora el rendimiento de la red. La división en subredes es uno de los componentes de la creación de subredes aisladas mediante el aislamiento físico, la configuración del enrutamiento y los firewalls.
Puntos clave

La división en subredes es una estrategia de Seguridad común utilizada por las organizaciones. La división en subredes permite a las organizaciones crear redes más pequeñas dentro de su red privada. Esto mejora la eficacia de la red y puede utilizarse para crear zonas de seguridad.


---

Esta sección del curso abarca mucha información sobre el funcionamiento de las redes. Ha repasado los fundamentos de la arquitectura de red y la comunicación y ahora puede utilizar estos conocimientos mientras aprende a proteger las redes. La seguridad de una red privada requiere mantener la confidencialidad de sus datos y restringir el acceso a los usuarios autorizados. 

En esta lectura, repasará varios temas de seguridad de redes tratados anteriormente en el curso, como las redes privadas virtuales (VPN), los servidores proxy, los cortafuegos y las zonas de seguridad. Continuará aprendiendo más sobre estos conceptos y cómo se relacionan entre sí a medida que avance en el curso. 
Protocolos de red comunes

Los protocolos de red se utilizan para dirigir el tráfico al dispositivo y servicio correctos en función del tipo de comunicación que realicen los dispositivos de la red. Los protocolos son las reglas utilizadas por todos los dispositivos de red que proporcionan una base mutuamente acordada sobre cómo transferir datos a través de una red.

Existen tres categorías principales de protocolos de red: protocolos de comunicación, protocolos de gestión y protocolos de seguridad.

    Los protocolos de Comunicación se utilizan para establecer conexiones entre servidores. Algunos ejemplos son TCP, UDP y el Protocolo simple de transmisión de correo (SMTP), que proporciona un framework para la comunicación por correo electrónico.

    Los protocolos de gestión se utilizan para solucionar problemas de red. Un ejemplo es el Protocolo de mensajes de control de Internet (ICMP).

    Los protocolos de Seguridad proporcionan encriptación para los Datos en tránsito. Algunos ejemplos son IPSec y SSL/TLS.

Otros protocolos de uso común son:

    Protocolo de transferencia de hipertexto (HTTP). HTTP es un protocolo de comunicación de capa de aplicación. Permite que el navegador y el servidor web se comuniquen entre sí.

    Sistema de nombres de dominio (DNS). DNS es un protocolo de capa de aplicación que traduce, o mapea, nombres de host a direcciones IP.

    Protocolo de resolución de direcciones (ARP). ARP es un protocolo de comunicación de capa de red que mapea direcciones IP a máquinas físicas o a una dirección MAC reconocida en la red de área local.

Wi-Fi

En esta sección del curso también se han presentado varios protocolos de Seguridad inalámbrica, como WEP, WPA, WPA2 y WPA3. WPA3 cifra el Tráfico con el Estándar de encriptación avanzada (AES) cuando viaja desde su dispositivo hasta el punto de acceso inalámbrico. WPA2 y WPA3 ofrecen dos modos: personal y empresarial. El modo personal es el más adecuado para redes domésticas, mientras que el modo empresarial se utiliza generalmente para redes y aplicaciones empresariales.
Herramientas y prácticas de Seguridad de red
Firewalls

Anteriormente, aprendió que los cortafuegos son dispositivos virtuales de red (NVA) o dispositivos de hardware que inspeccionan y pueden filtrar el Tráfico de red antes de que se le permita entrar en la red privada. Los cortafuegos tradicionales se configuran con reglas que le indican qué tipos de paquetes de datos están permitidos en función del número de puerto y la dirección IP del paquete de datos.

Existen dos categorías principales de firewalls.

    Sin estado: Una clase de firewall que funciona basándose en reglas predefinidas y no realiza un seguimiento de la información de los paquetes de datos

    Con estado: Una clase de firewall que hace un seguimiento de la información que pasa a través de él y filtra proactivamente las amenazas. A diferencia de los cortafuegos sin estado, que requieren la configuración de reglas en dos direcciones, un cortafuegos con estado sólo requiere una regla en una dirección. Esto se debe a que utiliza una "tabla de estado" para rastrear las conexiones, de modo que puede hacer coincidir el tráfico de retorno con una sesión existente.

Los cortafuegos de nueva generación (NGFW) son los cortafuegos de protección tecnológicamente más avanzados. Superan la seguridad ofrecida por los cortafuegos con estado porque incluyen inspección profunda de paquetes (un tipo de sniffing de paquetes que examina los paquetes de datos y toma medidas si existen amenazas) y características de prevención de intrusiones que detectan las amenazas a la seguridad y notifican a los administradores del cortafuegos. Los NGFW pueden inspeccionar el Tráfico en la capa de aplicación del Modelo TCP/IP y suelen ser conscientes de las aplicaciones. A diferencia de los firewalls tradicionales que bloquean el tráfico en función de la dirección IP y los puertos, las reglas de los NGFW pueden configurarse para bloquear o permitir el tráfico en función de la aplicación. Algunos NGFW disponen de características adicionales como Sandboxing de software malicioso, antivirus de red y filtrado de URL y DNS.
Servidores proxy

Un servidor proxy es otra forma de añadir Seguridad a su red privada. Los servidores proxy utilizan la traducción de direcciones de red (NAT) para servir de barrera entre los clientes de la red y las amenazas externas. 

Los proxies directos gestionan las consultas de los clientes internos cuando acceden a Recursos externos a la red. 
Los proxies inversos funcionan de forma opuesta a los proxies directos; gestionan las peticiones de sistemas externos a servicios de la red interna. Algunos servidores proxy también pueden configurarse con reglas, como un firewall. Por ejemplo, puede crear filtros para bloquear los sitios web identificados por contener software malicioso.
Redes privadas virtuales (VPN)

Una VPN es un servicio que encripta Datos en tránsito y disfraza su dirección IP. Las VPN utilizan un proceso llamado Encapsulación. La encapsulación envuelve sus datos no cifrados en un paquete de datos cifrados, lo que permite que sus datos se envíen a través de la red pública permaneciendo en el anonimato. Las empresas y otras organizaciones utilizan las VPN para ayudar a proteger las comunicaciones desde los dispositivos de los usuarios a los recursos corporativos. Algunos de estos recursos incluyen servidores o máquinas virtuales que alojan aplicaciones empresariales. Los particulares también utilizan las VPN para aumentar su privacidad personal. Las VPN protegen la privacidad del usuario ocultando su información personal, incluidas las direcciones IP, a servidores externos. Una VPN de buena reputación también minimiza su propio acceso a la actividad del usuario en Internet utilizando una fuerte encriptación y otras medidas de Seguridad. Las organizaciones utilizan cada vez más una combinación de VPN y SD-WAN para proteger sus redes. Una red de área extensa definida por software (SD-WAN) es un servicio WAN virtual que permite a las organizaciones conectar de forma segura a los usuarios con aplicaciones en múltiples ubicaciones y a través de grandes distancias geográficas. 
Claves

Existen tres categorías principales de protocolos de red: protocolos de comunicación, de gestión y de Seguridad. En esta lectura, ha aprendido los fundamentos de los firewalls, los servidores proxy y las VPN. Cada vez más organizaciones están implementando un enfoque basado en la nube para la seguridad de la red mediante la incorporación de una combinación de VPN y capacidades SD-WAN como servicio. 


---

Protocolos VPN: Wireguard e IPSec
Estado: Traducido automáticamente del Inglés
Traducido automáticamente del Inglés

Una VPN, o red privada virtual, es un servicio de seguridad de red que cambia su dirección IP pública y oculta su ubicación virtual para que pueda mantener la privacidad de sus datos cuando utilice una red pública como Internet. Las VPN proporcionan un servidor que actúa como puerta de enlace entre una computadora e Internet. Este servidor crea una ruta similar a un túnel virtual que oculta la dirección IP de la computadora y encripta los Datos en tránsito hacia Internet. El objetivo principal de una VPN es crear una conexión segura entre una computadora y una red. Además, una VPN permite establecer conexiones de confianza en redes que no lo son. Los protocolos VPN determinan cómo se forma el túnel de red seguro. Los distintos proveedores de VPN ofrecen protocolos VPN diferentes.

Esta lectura cubrirá las diferencias entre las VPN de acceso remoto y de sitio a sitio, y dos protocolos VPN: VPN WireGuard y VPN IPSec. Un protocolo VPN es similar a un protocolo de red: Es un conjunto de reglas o instrucciones que determinarán cómo se mueven los datos entre los puntos finales. Un punto final es cualquier dispositivo conectado a una red. Algunos ejemplos de puntos de conexión son las computadoras, los dispositivos móviles y los servidores.
Acceso remoto y VPN de sitio a sitio

Los usuarios individuales utilizan las VPN de acceso remoto para establecer una conexión entre un dispositivo personal y un servidor VPN. Las VPN de acceso remoto encriptan los datos enviados o recibidos a través de un dispositivo personal. La conexión entre el usuario y la VPN de acceso remoto se establece a través de Internet.

Las empresas utilizan las VPN de sitio a sitio en gran medida para extender su red a otras redes y ubicaciones. Esto es especialmente útil para las organizaciones que tienen muchas oficinas en todo el mundo. IPSec se utiliza habitualmente en las VPN de sitio a sitio para crear un túnel cifrado entre la red principal y la red remota. Una desventaja de las VPN de sitio a sitio es lo complejas que pueden ser de configurar y gestionar en comparación con las VPN remotas.
VPN WireGuard frente a VPN IPSec

WireGuard e IPSec son dos protocolos VPN diferentes que se utilizan para encriptar el tráfico a través de un túnel de red seguro. La mayoría de los proveedores de VPN ofrecen una gran variedad de opciones de protocolos VPN, como WireGuard o IPSec. En última instancia, elegir entre IPSec y WireGuard depende de muchos factores, como la velocidad de conexión, la compatibilidad con la infraestructura de red existente y las necesidades empresariales o individuales.
VPN WireGuard

WireGuard es un protocolo VPN de alta velocidad, con una encriptación avanzada, para proteger a los usuarios cuando acceden a Internet. Está diseñado para ser sencillo de configurar y mantener. WireGuard puede utilizarse tanto para conexiones de sitio a sitio como para conexiones cliente-servidor. WireGuard es relativamente más reciente que IPSec, y es utilizado por muchas personas debido a que su velocidad de descarga aumenta al utilizar menos líneas de programación. WireGuard también es de código abierto, lo que facilita a los usuarios su implementación y depuración. Este protocolo es útil para procesos que requieren velocidades de descarga más rápidas, como la transmisión de contenidos de vídeo o la descarga de archivos de gran tamaño.
VPN IPSec

IPSec es otro protocolo VPN que puede utilizarse para configurar VPN. La mayoría de los proveedores de VPN utilizan IPSec para encriptar y autenticar los paquetes de datos con el fin de establecer conexiones seguras y encriptadas. Dado que IPSec es uno de los primeros protocolos VPN, muchos sistemas operativos son compatibles con IPSec de los proveedores de VPN.

Aunque IPSec y WireGuard son ambos protocolos VPN, IPSec es más antiguo y más complejo que WireGuard. Algunos clientes pueden preferir IPSec debido a su larga historia de uso, sus exhaustivas pruebas de seguridad y su amplia Adopción. Sin embargo, otros pueden preferir WireGuard por su potencial de mejor rendimiento y configuración más sencilla.
Claves

Un protocolo VPN es similar a un protocolo de redes: Es un conjunto de reglas o instrucciones que determinarán cómo se mueven los datos entre los puntos finales. Existen dos tipos de VPN: de acceso remoto y de sitio a sitio. Las VPN de acceso remoto establecen una conexión entre un dispositivo personal y un servidor VPN y encriptan o desencriptan los datos intercambiados con un dispositivo personal. Las empresas utilizan las VPN de sitio a sitio en gran medida para extender su red a diferentes ubicaciones y redes. IPSec puede utilizarse para crear conexiones de sitio a sitio y WireGuard puede utilizarse tanto para conexiones de sitio a sitio como para conexiones de acceso remoto