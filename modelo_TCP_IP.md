### la dirección MAC y la dirección IP del dispositivo de destino están contenidas en el encabezado y el pie de página de un paquete de datos. Esta es una amenaza de Seguridad porque muestra la IP y la ubicación virtual de su red privada. 

Los servicios de VPN cifran sus paquetes de datos y
los encapsulan en otros paquetes de datos
que los enrutadores pueden leer.
Esto permite que tus solicitudes de red
lleguen a su destino ,
pero aun así encripta tus datos personales para que no se puedan leer mientras están en tránsito.
Una VPN también utiliza un túnel cifrado
entre el dispositivo y el servidor VPN.
La encriptación no se puede hackear sin una clave criptográfica
por lo que nadie puede acceder a sus datos.
Los servicios de VPN son sencillos y ofrecen
una protección significativa mientras estás en Internet . 


El Modelo TCP/IP

TCP es un protocolo de comunicación de Internet que permite que
dos dispositivos establezcan una conexión y transmitan datos.
El TCP también verifica ambos dispositivos antes de permitir que se lleve a cabo cualquier otra comunicación
Esto a menudo se denomina protocolo de enlace. 

Tenga en cuenta que el protocolo TCP no se limita a dos dispositivos. Establece una conexión directa entre dos puntos finales, pero la infraestructura de red subyacente puede encargarse del enrutamiento de paquetes de datos a través de múltiples dispositivos. 

El Modelo TCP/IP es un framework utilizado para visualizar cómo se organizan y transmiten los datos a través de una red. Este Modelo ayuda a los ingenieros de redes y a los analistas de seguridad de redes a conceptualizar los procesos en la red y a comunicar dónde se producen las interrupciones o las amenazas a la seguridad.

El Modelo TCP/IP tiene cuatro capas: 
la capa 1 de accesibilidad a la red, 
la capa 2 de Internet, 
la capa 3 de transporte 
la capa 4 de aplicación.

El Protocolo de Resolución de Direcciones (ARP) es un protocolo de red que traduce direcciones IP a direcciones MAC (direcciones físicas) en una red de área local (LAN). 

Capa de acceso a la red

La capa de acceso a la red, a veces denominada capa de vínculo de datos, se ocupa de la creación de paquetes de datos y su transmisión a través de una red. Esta capa corresponde al hardware físico implicado en la transmisión de la red. Concentradores, módems, cables y cableado se consideran parte de esta capa. El protocolo de resolución de direcciones (ARP) forma parte de la capa de accesibilidad a la red. Dado que las direcciones MAC se utilizan para identificar hosts en la misma red física, ARP es necesario para asignar direcciones IP a direcciones MAC para la comunicación de red local.
Capa de Internet

La capa de Internet, a veces denominada capa de red, es responsable de garantizar la entrega al host de destino, que potencialmente reside en una red diferente. Garantiza que las direcciones IP se adjunten a los paquetes de datos para indicar la ubicación del remitente y el destinatario. La capa de Internet también determina qué protocolo es responsable de entregar los paquetes de datos y garantiza la entrega al host de destino. Estos son algunos de los protocolos comunes que operan en la capa de Internet:

    Protocolo de Internet (IP). IP envía los paquetes de datos al destino correcto y se basa en el Protocolo de control de transmisión/Protocolo de Datagramas de Usuario (TCP/UDP) para entregarlos al servicio correspondiente. Los paquetes IP permiten la comunicación entre dos redes. Se encaminan desde la red emisora hasta la red receptora. El TCP, en particular, retransmite cualquier dato que se pierda o esté corrupto.

    Protocolo de mensajes de control de Internet (ICMP). El ICMP comparte información sobre errores y actualizaciones del estado de los paquetes de datos. Esto resulta útil para detectar y solucionar errores de red. El ICMP transmite información sobre paquetes que se han perdido o que han desaparecido en tránsito, problemas con la conectividad de la red y paquetes redirigidos a otros routers.

Capa de transporte

La capa de transporte es responsable de la entrega de datos entre dos sistemas o redes e incluye protocolos para controlar el flujo de tráfico a través de una red. TCP y UDP son los dos protocolos de transporte que se dan en esta capa.
Protocolo de control de transmisión

El Protocolo de control de transmisión (TCP ) es un protocolo de comunicación de Internet que permite que dos dispositivos formen una conexión y transmitan datos. Garantiza que los Datos se transmitan de forma fiable al servicio de destino. TCP contiene el número de puerto del servicio de destino previsto, que reside en el encabezado TCP de un paquete TCP/IP.
Protocolo de Datagramas de Usuario 

El Protocolo de Datagramas de Usuario (UDP) es un protocolo no orientado a la conexión que no establece una conexión entre dispositivos antes de las transmisiones. Lo utilizan aplicaciones a las que no les preocupa la fiabilidad de la transmisión. Los Datos enviados a través de UDP no son objeto de un seguimiento tan exhaustivo como los enviados mediante TCP. Dado que UDP no establece conexiones de red, se utiliza sobre todo para aplicaciones sensibles al rendimiento que funcionan en tiempo real, como la transmisión de vídeo.
Capa de aplicación

La capa de aplicación en el Modelo TCP/IP es similar a las capas de aplicación, presentación y sesión del Modelo OSI. La capa de aplicación es la responsable de realizar las solicitudes de red o de responder a las peticiones. Esta capa define a qué servicios y aplicaciones de Internet puede acceder cualquier usuario. Los protocolos de la capa de aplicación determinan cómo interactuarán los paquetes de datos con los dispositivos receptores. Algunos protocolos comunes utilizados en esta capa son:

    Protocolo de transferencia de hipertexto (HTTP)

    Protocolo simple de transmisión de correo (SMTP)

    Secure Shell (SSH)

    Protocolo de transferencia de archivos (FTP)

    Sistema de nombres de dominio (DNS)

Los protocolos de la capa de aplicación se basan en capas subyacentes para transferir los datos a través de la red.
Modelo TCP/IP frente al modelo OSI
Modelo TCP/IP junto al modelo OSI

El OSI organiza visualmente los protocolos de redes en diferentes capas. Los profesionales de las redes suelen utilizar este modelo para comunicarse entre sí sobre posibles fuentes de problemas o amenazas a la seguridad cuando se producen. 

El Modelo TCP/IP combina varias capas del modelo OSI. Existen muchas similitudes entre ambos Modelos. Ambos Modelos definen Estándares para las redes y dividen el proceso de comunicación de la red en diferentes capas. El Modelo TCP/IP es una versión simplificada del modelo OSI.
Puntos clave

Tanto el modelo TCP/IP como el OSI son modelos conceptuales que ayudan a los profesionales de las redes a visualizar los procesos y protocolos de red en lo que respecta a la transmisión de datos entre dos o más sistemas. El Modelo TCP/IP contiene cuatro capas y el modelo OSI, siete.



---

Componentes de la capa de red de comunicación
Estado: Traducido automáticamente del Inglés
Traducido automáticamente del Inglés

En la lectura sobre el modelo OSI

, aprendió sobre las siete capas del Modelo OSI que se utilizan para conceptualizar la forma en que se transmiten los datos a través de Internet. En esta lectura, aprenderá más sobre las operaciones que tienen lugar en la capa 3 del modelo OSI: la capa de red.
Operaciones en la capa de red

Las funciones en la capa de red organizan el direccionamiento y la entrega de paquetes de datos a través de la red desde el dispositivo anfitrión hasta el dispositivo de destino. Esto incluye dirigir los paquetes de un router a otro a través de Internet, hasta que llega a la dirección IP (protocolo de Internet) de la red de destino. La dirección IP de destino está contenida en el encabezamiento de cada paquete de datos. Esta dirección se almacenará con fines de enrutamiento futuro en las tablas de enrutamiento a lo largo de la ruta de acceso del paquete hasta su destino.

Todos los paquetes de datos incluyen una dirección IP. Un paquete de datos también se denomina paquete IP para las conexiones TCP o datagrama para las conexiones UDP. Un router utiliza la dirección IP para encaminar los paquetes de una red a otra basándose en la información contenida en el encabezado IP de un paquete de datos. La Información del Encabezado comunica algo más que la dirección del destino. También incluye información como la dirección IP de origen, el tamaño del paquete y qué protocolo se utilizará para la parte de datos del paquete.
Formato de un paquete IPv4
Un paquete IP dividido en dos partes: una sección a la izquierda marcada como "cabecera" y una sección a la derecha marcada como "datos"

A continuación, puede repasar el formato de un paquete IP versión 4 (IPv4) y revisar un gráfico detallado del encabezado del paquete. Un paquete IPv4 se compone de dos secciones, la cabecera y los datos:

    El formato del Encabezado IPv4 viene determinado por el protocolo IPv4 e incluye la información de enrutamiento IP que los dispositivos utilizan para dirigir el Paquete. El tamaño del encabezado IPv4 oscila entre 20 y 60 bytes. Los primeros 20 bytes son un conjunto fijo de información que contiene datos como la dirección IP de origen y destino, la longitud de la cabecera y la longitud total del paquete. El último conjunto de bytes puede oscilar entre 0 y 40 y está formado por el campo de opciones.

    La longitud de la sección de Datos de un paquete IPv4 puede variar mucho en tamaño. Sin embargo, el tamaño máximo posible de un paquete IPv4 es de 65.535 bytes. Contiene el mensaje que se transfiere por Internet, como la información de un sitio web o el texto de un correo electrónico. 

Diagrama de una cabecera de paquete IPv4, 13 campos y tamaño de bit

Hay 13 campos dentro del Encabezado de un paquete IPv4:

    Versión (VER): Este componente de 4 bits indica a los dispositivos receptores qué protocolo está utilizando el paquete. El paquete utilizado en la ilustración anterior es un paquete IPv4.

    Longitud del Encabezado IP (HLEN o IHL): HLEN es la longitud del encabezado del paquete. Este valor indica dónde termina el encabezado del paquete y dónde comienza el segmento de datos.

    Tipo de servicio (ToS): Los routers priorizan la entrega de paquetes para mantener la calidad del servicio en la red. El Campo ToS proporciona al router esta Información.

    Longitud total: Este campo comunica la longitud total de todo el paquete IP, incluyendo la cabecera y los datos. El tamaño máximo de un paquete IPv4 es de 65.535 bytes.

    Identificación: Los paquetes IPv4 pueden tener hasta 65, 535 bytes, pero la mayoría de las redes tienen un límite menor. En estos casos, los paquetes se dividen, o fragmentan, en paquetes IP más pequeños. El campo de identificación proporciona un identificador Único para todos los fragmentos del paquete IP original, de forma que puedan ser reensamblados una vez que lleguen a su destino.

    Banderas: Este Campo proporciona al dispositivo de enrutamiento más información sobre si el paquete original ha sido fragmentado y si hay más fragmentos en tránsito.

    Desplazamiento de fragmentación: El campo de offset de fragmentación indica a los dispositivos de encaminamiento a qué parte del paquete original pertenece el fragmento.

    Tiempo de vida (TTL ): El TTL impide que los paquetes de datos sean reenviados por los routers indefinidamente. Contiene un contador que establece la fuente. El contador se decrementa en uno a medida que pasa por cada router a lo largo de su ruta de acceso. Cuando el contador TTL llega a cero, el router que tiene el paquete en ese momento lo descarta y devuelve al remitente un mensaje de error ICMP Time Exceeded.

    Protocolo: El campo de protocolo indica al dispositivo receptor qué protocolo se utilizará para la parte de datos del paquete.

    Suma de comprobación del encabezado: El campo de suma de comprobación de encabezado contiene una suma de comprobación que puede utilizarse para detectar la corrupción del encabezado IP en tránsito. Los paquetes corruptos se descartan.

    Dirección IP de origen: La dirección IP de origen es la dirección IPv4 del dispositivo emisor.

    Dirección IP de destino: La dirección IP de destino es la dirección IPv4 del dispositivo de destino.

    Opciones: El campo de opciones permite aplicar opciones de Seguridad al Paquete si el valor HLEN es superior a cinco. El Campo comunica estas opciones a los dispositivos de enrutamiento.

Diferencia entre IPv4 e IPv6

En una parte anterior de este curso, conoció la historia de las direcciones IP. A medida que Internet crecía, se hizo evidente que todas las direcciones IPv4 acabarían agotándose; es lo que se denomina agotamiento de las direcciones IPv4. En aquel momento, nadie había previsto cuántos dispositivos informáticos necesitarían una dirección IP. IPv6 se desarrolló para mitigar el agotamiento de las direcciones IPv4 y otras preocupaciones relacionadas.

Algunas de las principales diferencias entre IPv4 e IPv6 son la longitud y el formato de las direcciones. Las direcciones IPv4 se componen de cuatro números decimales separados por puntos, cada número va de 0 a 255. Juntos, los números abarcan 4 bytes y permiten hasta 4.300 millones de direcciones posibles. Un ejemplo de dirección IPv4 sería: 198.51.100.0. Las direcciones IPv6 están formadas por ocho números hexadecimales separados por dos puntos, cada número consta de hasta cuatro dígitos hexadecimales. Juntos, todos los números abarcan 16 bytes y permiten hasta 340 undecilillones de direcciones (340 seguidos de 36 ceros). Un ejemplo de dirección IPv6 sería: 2002:0db8:0000:0000:0000:ff21:0023:1234.

Nota: para representar uno o más conjuntos consecutivos de todos ceros, puede sustituir los ceros por dos puntos dobles "::", por lo que la dirección IPv6 anterior sería "2002:0db8::ff21:0023:1234"

También existen algunas diferencias en el diseño del Encabezado de un Paquete IPv6. El formato del Encabezado IPv6 es mucho más sencillo que el de IPv4. Por ejemplo, el Encabezado IPv4 incluye los campos IHL, Identificación y Banderas, mientras que el IPv6 no. El encabezado IPv6 sólo introduce el campo de etiqueta de flujo, donde la etiqueta de flujo identifica un paquete como que requiere un manejo especial por parte de otros routers IPv6.
Diagramas paralelos de una cabecera de paquete IPv4 y un paquete IPv6 simplificado

Existen algunas diferencias de Seguridad importantes entre IPv4 e IPv6. IPv6 ofrece un enrutamiento más eficaz y elimina las colisiones de direcciones privadas que pueden producirse en IPv4 cuando dos dispositivos de la misma red intentan utilizar la misma dirección.
Puntos clave

El análisis de los distintos campos de un paquete de datos IP puede servir para averiguar información importante sobre la seguridad del paquete. Algunos ejemplos de información relacionada con la seguridad que se encuentra en los paquetes de direcciones IP son: de dónde viene el paquete, a dónde va y qué protocolo está utilizando. Comprender los datos de un paquete de datos IP le permitirá tomar decisiones críticas sobre las implicaciones para la seguridad de los paquetes que inspeccione.

---


Protocolos de red comunes
Estado: Traducido automáticamente del Inglés
Traducido automáticamente del Inglés

En esta sección del curso, ha aprendido acerca de los protocolos de red y cómo organizan la comunicación a través de una red. Esta lectura tratará los protocolos de red en mayor profundidad y repasará algunos protocolos básicos que ha aprendido anteriormente. También aprenderá nuevos protocolos y analizará algunas de las formas en que los protocolos intervienen en la Seguridad de las redes.
Visión general de los protocolos de red

Un protocolo de red es un conjunto de reglas utilizadas por dos o más dispositivos de una red para describir el orden de entrega y la estructura de los datos. Los protocolos de red sirven como instrucciones que acompañan a la información del paquete de datos. Estas instrucciones indican al dispositivo receptor qué debe hacer con los Datos. Los protocolos son como un lenguaje común que permite a los dispositivos de todo el mundo comunicarse y entenderse entre sí.

Aunque los protocolos de red desempeñan una función esencial en la comunicación de la red, los analistas de seguridad deben comprender sus implicaciones de seguridad asociadas. Algunos protocolos tienen vulnerabilidades que los actores maliciosos explotan. Por ejemplo, un actor nefasto podría utilizar el protocolo del sistema de nombres de dominio (DNS), que resuelve las direcciones web en direcciones IP, para desviar el tráfico de un sitio web legítimo a un sitio web malicioso que contenga software malicioso. Aprenderá más sobre este tema en los próximos materiales del curso.
Tres categorías de protocolos de red

Los protocolos de red pueden dividirse en tres categorías principales: protocolos de comunicación, protocolos de gestión y protocolos de seguridad. Existen docenas de protocolos de red diferentes, pero no necesita memorizarlos todos para desempeñar un papel de analista de seguridad de nivel básico. Sin embargo, es importante que conozca los que se enumeran en esta lectura.
Protocolos de comunicación

Los protocolos de comunicación rigen el intercambio de información en la transmisión por red. Dictan cómo se transmiten los Datos entre dispositivos y el momento de la comunicación. También incluyen métodos para recuperar Datos perdidos en tránsito. He aquí algunos de ellos.

    ElProtocolo de control de transmisión (TCP ) es un protocolo de comunicación de Internet que permite que dos dispositivos formen una conexión y transmitan datos. TCP utiliza un proceso de protocolo de enlace de tres vías. En primer lugar, el dispositivo envía una solicitud de sincronización (SYN) a un servidor. A continuación, el servidor responde con un paquete SYN/ACK para acusar recibo de la solicitud del dispositivo. Una vez que el servidor recibe el último paquete ACK del dispositivo, se establece una conexión TCP. En el Modelo TCP/IP, TCP se produce en la capa de transporte.

    ElProtocolo de Datagramas de Usuario (UDP) es un protocolo no orientado a la conexión que no establece una conexión entre dispositivos antes de una transmisión. Esto hace que sea menos fiable que TCP. Pero también significa que funciona bien para transmisiones que necesitan llegar a su destino rápidamente. Por ejemplo, un uso de UDP es para enviar solicitudes DNS a servidores DNS locales. En el Modelo TCP/IP, UDP se produce en la capa de transporte.

    ElProtocolo de transferencia de hipertexto (HTTP) es un protocolo de capa de aplicación que proporciona un método de comunicación entre clientes y servidores de sitios web. HTTP utiliza el puerto 80. HTTP se considera inseguro, por lo que está siendo sustituido en la mayoría de los sitios web por una versión segura, denominada HTTPS que utiliza la encriptación de SSL/TLS para la comunicación. Sin embargo, todavía hay muchos sitios web que utilizan el protocolo inseguro HTTP. En el Modelo TCP/IP, HTTP se produce en la capa de aplicación.

    Elsistema de nombres de dominio (DNS) es un protocolo que traduce los nombres de dominio de Internet en direcciones IP. Cuando una computadora de cliente desea acceder al dominio de un sitio web utilizando su navegador de Internet, se envía una consulta a un servidor DNS dedicado. El servidor DNS busca entonces la dirección IP que corresponde al dominio del sitio web. DNS utiliza normalmente UDP en el puerto 53. Sin embargo, si la respuesta del DNS a una solicitud es grande, pasará a utilizar el protocolo TCP. En el Modelo TCP/IP, el DNS se produce en la capa de aplicación.

Protocolos de Gestion

La siguiente categoría de protocolos de red son los protocolos de gestión. Los protocolos de gestión se utilizan para supervisar y gestionar la actividad en una red. Incluyen protocolos para la notificación de errores y la optimización del rendimiento en la red.

    ElProtocolo simple de administración de red (SNMP) es un protocolo de red utilizado para supervisar y gestionar los dispositivos de una red. SNMP puede restablecer una contraseña en un dispositivo de red o cambiar su configuración base. También puede enviar solicitudes a los dispositivos de red para obtener un informe sobre la cantidad de ancho de banda de la red que se está utilizando. En el Modelo TCP/IP, SNMP se produce en la capa de aplicación.

    ElProtocolo de mensajes de control de Internet (ICMP) es un protocolo de Internet utilizado por los dispositivos para informarse mutuamente de los errores de transmisión de datos a través de la red. El ICMP es utilizado por un dispositivo receptor para enviar un informe al dispositivo emisor sobre la transmisión de datos. El ICMP se utiliza habitualmente como una forma rápida de solucionar problemas de conectividad y latencia de la red mediante la emisión del comando "ping" en un sistema operativo Linux. En el Modelo TCP/IP, el ICMP se produce en la capa de Internet.

Protocolos de Seguridad

Los protocolos de Seguridad son protocolos de red que garantizan que los datos se envían y reciben de forma segura a través de una red. Los protocolos de Seguridad utilizan algoritmos de encriptación para proteger los datos en tránsito. A continuación se indican algunos protocolos de Seguridad comunes.

    Protocolo seguro de transferencia de hipertexto (HTTPS ) es un protocolo de red que proporciona un método seguro de comunicación entre clientes y servidores de sitios web. HTTPS es una versión segura de HTTP que utiliza la encriptación secure sockets layer/transport layer security (SSL/TLS) en todas las transmisiones para que los actores maliciosos no puedan leer la información contenida. HTTPS utiliza el puerto 443. En el Modelo TCP/IP, HTTPS se produce en la capa de aplicación.

    ElProtocolo seguro de transferencia de archivos (SFTP ) es un protocolo seguro utilizado para transferir archivos de un dispositivo a otro a través de una red. SFTP utiliza Secure Shell (SSH), normalmente a través del puerto TCP 22. SSH utiliza el Estándar de encriptación avanzada (AES) y otros tipos de encriptación para garantizar que los destinatarios no deseados no puedan interceptar las transmisiones. En el Modelo TCP/IP, SFTP se produce en la capa de aplicación. SFTP se utiliza a menudo con el almacenamiento en la nube. Cada vez que un usuario sube o baja un archivo del almacenamiento en la nube, el archivo se transfiere utilizando el protocolo SFTP.

Nota: Los protocolos de encriptación mencionados no ocultan la dirección IP de origen o destino del tráfico de red. Esto significa que un actor malicioso aún puede conocer cierta información básica sobre el tráfico de red si lo intercepta.
Puntos clave

Los protocolos sobre los que ha aprendido en esta lectura son protocolos de redes básicos que los analistas de ciberseguridad de nivel básico deberían conocer. Comprender cómo funcionan los protocolos en una red es esencial. Los analistas de ciberseguridad pueden aprovechar su conocimiento de los protocolos para mitigar con éxito las vulnerabilidades de una red y prevenir potencialmente futuros ataques.



---


Protocolos de red adicionales
Estado: Traducido automáticamente del Inglés
Traducido automáticamente del Inglés

En lecturas y vídeos anteriores, aprendió cómo los protocolos de red organizan el envío y la recepción de datos a través de una red. También aprendió que los protocolos pueden dividirse en tres categorías: protocolos de Comunicación, protocolos de Gestión y protocolos de Seguridad.

Esta lectura le presentará algunos conceptos y protocolos adicionales que surgirán con regularidad en su trabajo como analista de Seguridad. La Autoridad de Números Asignados en Internet (IANA) asigna números de puerto a algunos protocolos. Estos números de puerto se incluyen en la descripción de cada protocolo, si se han asignado.
Traducción de direcciones de red

Los dispositivos de su red local doméstica o de oficina tienen cada uno una dirección IP privada que utilizan para comunicarse directamente entre sí. Sin embargo, para que los dispositivos con direcciones IP privadas puedan comunicarse con la Internet pública, necesitan tener una única dirección IP pública que represente a todos los dispositivos de la LAN ante el público. Para los mensajes salientes, el router puede sustituir una dirección IP de origen privada por su dirección IP pública y realizar la operación inversa para las respuestas. Este proceso se conoce como traducción de direcciones de red (NAT) y generalmente requiere que un router o firewall esté configurado específicamente para realizar NAT. NAT forma parte de la capa 2 (capa de Internet) y de la capa 3 (capa de transporte) del Modelo TCP/IP.

 Direcciones IP privadas
	

Direcciones IP públicas

    Asignadas por el router

    Únicas sólo dentro de la red privada

    Sin coste de uso

    Rangos de direcciones:

        10.0.0.0-10.255.255.255

        172.16.0.0-172.31.255.255

        192.168.0.0-192.168.255.255

	

    Asignada por ISP e IANA

    Dirección Única en Internet global

    Costos de arrendamiento de una dirección IP pública

    Rangos de direcciones asignables:

        1.0.0.0-9.255.255.255

        11.0.0.0-126.255.255.255

        128.0.0.0-172.15.255.255

        172.32.0.0-192.167.255.255

        192.169.0.0-233.255.255.255

Protocolo de configuración dinámica de host

El Protocolo de configuración dinámica de host (DHCP) pertenece a la familia de protocolos de red de gestión. DHCP es un protocolo de capa de aplicación que se utiliza en una red para configurar dispositivos. Funciona con el router para asignar una dirección IP Única a cada dispositivo y proporcionar las direcciones del servidor DNS y de la puerta de enlace predeterminada adecuados para cada dispositivo. Los servidores DHCP operan en el puerto UDP 67 mientras que los clientes DHCP lo hacen en el puerto UDP 68.
Protocolo de resolución de direcciones

A estas alturas, ya está familiarizado con las direcciones IP y MAC. Ha aprendido que cada dispositivo de una red tiene una dirección IP pública, una dirección IP privada y una dirección MAC que lo identifican en la red. La dirección IP de un dispositivo puede cambiar con el tiempo, pero su dirección MAC es permanente porque es Única para la tarjeta de interfaz de red de un dispositivo. La dirección MAC se utiliza para comunicarse con dispositivos dentro de la misma red, pero a veces, la dirección MAC es desconocida. Por eso es necesario el protocolo de resolución de direcciones (ARP). ARP es principalmente un protocolo de la capa de acceso a la red en el Modelo TCP/IP que se utiliza para traducir las direcciones IP que se encuentran en los paquetes de datos a la dirección MAC del dispositivo de hardware.

Cada dispositivo de la red ejecuta ARP y mantiene un registro de las direcciones IP y MAC coincidentes en un caché ARP. ARP no tiene un número de puerto específico ya que es un protocolo de capa 2 y los números de puerto están asociados a la capa de aplicación 7.
Telnet

Telnet es un protocolo de capa de aplicación que se utiliza para conectar con un sistema remoto. Telnet envía toda la Información en texto claro. Utiliza la línea de comandos para controlar otro dispositivo de forma similar a secure shell (SSH), pero Telnet no es tan seguro como SSH. Telnet puede utilizarse para conectarse a dispositivos locales o remotos y utiliza el puerto TCP 23.
Secure Shell

El protocolo Secure Shell (SSH) se utiliza para crear una conexión segura con un sistema remoto. Este protocolo de capa de aplicación proporciona una alternativa para la autenticación segura y la encriptación de la comunicación. SSH funciona a través del puerto TCP 22 y es un sustituto de protocolos menos seguros, como Telnet.
Protocolo de oficina de correos

El protocolo de oficina de correos (POP) es un protocolo de capa de aplicación (capa 4 del Modelo TCP/IP) utilizado para gestionar y recuperar correo electrónico de un servidor de correo. POP3 es la versión más utilizada de POP. Muchas organizaciones tienen un servidor de correo dedicado en la red que gestiona el correo entrante y saliente para los usuarios de la red. Los dispositivos de los usuarios enviarán solicitudes al servidor de correo remoto y descargarán los mensajes de correo electrónico localmente. Si alguna vez ha actualizado su aplicación de correo electrónico y ha visto aparecer nuevos mensajes en su bandeja de entrada, está experimentando el POP y el protocolo de acceso a mensajes de Internet (IMAP) en acción. La autenticación en texto plano sin cifrar utiliza el puerto TCP/UDP 110 y los correos electrónicos cifrados utilizan la Capa de sockets seguros/Seguridad de la capa de transporte (SSL/TLS) a través del puerto TCP/UDP 995. Cuando se utiliza POP, el correo tiene que terminar de descargarse en un dispositivo local antes de poder ser leído. Después de descargarse, el correo puede o no borrarse del servidor de correo, por lo que no garantiza que un usuario pueda sincronizar el mismo correo electrónico en varios dispositivos.
Protocolo de acceso a mensajes de Internet (IMAP)

IMAP se utiliza para el correo electrónico entrante. Descarga las cabeceras de los correos electrónicos y el contenido del mensaje. El contenido también permanece en el servidor de correo electrónico, lo que permite a los usuarios acceder a su correo electrónico desde múltiples dispositivos. IMAP utiliza el puerto TCP 143 para el correo electrónico no cifrado y el puerto TCP 993 a través del protocolo TLS. El uso de IMAP permite a los usuarios leer parcialmente el correo electrónico antes de que termine de descargarse. Dado que el correo se guarda en el servidor de correo, permite al usuario sincronizar los correos electrónicos de varios dispositivos. 
Protocolo simple de transmisión de correo

El Protocolo simple de transmisión de correo (SMTP) se utiliza para transmitir y encaminar el correo electrónico del remitente a la dirección del destinatario. SMTP funciona con el software del Agente de Transferencia de Mensajes (MTA), que busca en los servidores DNS para resolver las direcciones de correo electrónico en direcciones IP, con el fin de garantizar que los correos electrónicos lleguen a su destino previsto. SMTP utiliza el puerto TCP/UDP 25 para los correos electrónicos no cifrados y el puerto TCP/UDP 587 que utiliza TLS para los correos electrónicos cifrados. El puerto TCP 25 suele ser utilizado por el spam de gran volumen. SMTP ayuda a filtrar el spam regulando cuántos correos electrónicos puede enviar una fuente a la vez.
Protocolos y números de puerto

Recuerde que los números de puerto son utilizados por los dispositivos de red para determinar qué debe hacerse con la información contenida en cada paquete de datos una vez que llegan a su destino. Los firewalls pueden filtrar el Tráfico no deseado basándose en los números de puerto. Por ejemplo, una organización puede configurar un firewall para que sólo permita la accesibilidad al puerto TCP 995 (POP3) a las direcciones IP pertenecientes a la organización.

Como analista de Seguridad, necesitará conocer muchos de los protocolos y números de puerto mencionados en este curso. Pueden ser utilizados para determinar sus conocimientos técnicos en las entrevistas, por lo que es una buena idea memorizarlos. También aprenderá sobre nuevos protocolos en el trabajo en un puesto de Seguridad.
Puntos clave

ASÍ COMO analista de ciberseguridad, se encontrará con varios protocolos comunes en su trabajo diario. Los protocolos cubiertos en esta lectura incluyen NAT, DHCP, ARP, Telnet, SSH, POP3, IMAP y SMTP. Es igualmente importante comprender dónde se estructura cada protocolo en el Modelo TCP/IP y qué puertos ocupan.

 Protocolo
	

Puerto

DHCP
	

Puerto UDP 67 (servidores)

Puerto UDP 68 (clientes)

ARP
	

ninguno

Telnet
	

Puerto TCP 23

SSH
	

TCP puerto 22

POP3
	

TCP/UDP puerto 110 (sin cifrar)

TCP/UDP puerto 995 (encriptado, SSL/TLS)

IMAP
	

TCP puerto 143 (sin cifrar)

Puerto TCP 993 (encriptado, SSL/TLS)

SMTP
	

TCP/UDP puerto 25 (sin cifrar)

SMTPS
	

TCP/UDP puerto 587 (encriptado, TLS)