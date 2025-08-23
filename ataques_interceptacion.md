
Visión general de las tácticas de interceptación
Estado: Traducido automáticamente del Inglés
Traducido automáticamente del Inglés

En los puntos anteriores del curso, aprendió cómo se utilizan el sniffing de paquetes y la Suplantación de IP en los ataques a las redes. Dado que estos ataques interceptan paquetes de datos mientras viajan por la red, se denominan 

## Ataques de interceptación.
### Sniffing de paquetes    
    es la práctica de capturar e inspeccionar paquetes de datos a través de una red
La tarjeta de interfaz de red (NIC) del dispositivo es una pieza de hardware que conecta el dispositivo a una red. La NIC lee la transmisión de datos y, si contiene la dirección MAC del dispositivo, acepta el paquete y lo envía al dispositivo para que procese la información basándose en el protocolo. Esto ocurre en todas las operaciones de red estándar. Sin embargo, una NIC puede configurarse en modo promiscuo, lo que significa que acepta todo el tráfico de la red, incluso los paquetes que no están dirigidos al dispositivo de la NIC. Más adelante en el Programa aprenderá más sobre las NIC. Los actores maliciosos podrían utilizar software como Wireshark para capturar los datos de una red privada y almacenarlos para su uso posterior. A continuación, pueden utilizar la información personal en su propio beneficio. Otra posibilidad es que utilicen las direcciones IP y MAC de los usuarios autorizados de la red privada para realizar la suplantación de IP.

### Suplantación de IP (IP spoofing)
es un ataque de red que se realiza cuando un atacante cambia la IP de origen de un paquete de datos para hacerse pasar por un sistema autorizado y obtener acceso a una red. 

#### ataques en ruta
es un ataque en el que el actor malintencionado se coloca en medio de una conexión autorizada
e intercepta o altera los datos en tránsito. Donde se rastrea la información del paquete para conocer las direcciones IP y MAC de los dispositivos que se comunican entre sí.
Una vez que tengan esta información , pueden fingir ser cualquiera de estos dispositivos. 

#### ataques de repetición
Un ataque de reproducción es un ataque de red que se realiza cuando un actor malintencionado intercepta un paquete de datos en tránsito y lo retrasa o lo repite en otro momento.

## ataques de pitufos(ataque smurf)
Es una combinación de un ataque
DDoS y un ataque de suplantación de IP.
El atacante olfatea la dirección IP de un usuario autorizado
y la inunda de paquetes. 

Después de que un actor malicioso haya olfateado paquetes en la red, puede suplantar las direcciones IP y MAC de dispositivos autorizados para realizar un ataque de suplantación de IP. Los cortafuegos pueden evitar los ataques de suplantación de IP configurándolos para que rechacen los paquetes IP no autorizados y el tráfico sospechoso. A continuación, examinará algunos ataques comunes de suplantación de IP con los que es importante familiarizarse como analista de Seguridad.
Ataque en ruta

Un ataque en ruta se produce cuando un hacker intercepta la comunicación entre dos dispositivos o servidores que tienen una relación de confianza. La transmisión entre estos dos dispositivos de red de confianza podría contener información valiosa como nombres de usuario y contraseñas que el actor malicioso puede recopilar. Un ataque en ruta se denomina a veces ataque de intermediario porque el hacker se esconde en medio de las comunicaciones entre dos partes de confianza.

También puede ocurrir que la transmisión interceptada contenga una búsqueda en el sistema DNS. Recordará de un vídeo anterior que un servidor DNS traduce los nombres de dominio de los sitios web en direcciones IP. Si un agente malicioso intercepta una transmisión que contiene una búsqueda DNS, podría falsificar la respuesta DNS del servidor y redirigir un nombre de dominio a una dirección IP diferente, quizás una que contenga código malicioso u otras amenazas. La forma más importante de protegerse contra un ataque en ruta es la encriptación de sus Datos en tránsito, por ejemplo utilizando TLS. 
Ataque Smurf

Un Ataque Smurf es un ataque a la red que se realiza cuando un atacante olfatea la dirección IP de un usuario autorizado y lo inunda de paquetes. Una vez que el paquete falsificado alcanza la dirección de broadcast, se envía a todos los dispositivos y servidores de la red.

En un ataque Smurf, la suplantación de IP se combina con otra técnica de denegación de servicio (DoS) para inundar la red con tráfico no deseado. Por ejemplo, el Paquete falsificado podría incluir un ping del Protocolo de mensajes de control de Internet (ICMP). Como ya ha aprendido, el ICMP se utiliza para solucionar problemas en una red. Pero si se transmiten demasiados mensajes ICMP, las respuestas de eco ICMP abruman a los servidores de la red y éstos se apagan. Esto crea una denegación de servicio y puede paralizar las operaciones de una organización.

Una forma importante de protegerse contra un ataque smurf es utilizar un firewall avanzado que pueda supervisar cualquier tráfico inusual en la red. La mayoría de los firewalls de nueva generación (NGFW) incluyen características que detectan anomalías en la red para garantizar que se detectan las broadcast de tamaño excesivo antes de que tengan la oportunidad de hacer caer la red.
Ataque DoS

Como ya ha aprendido, una vez que el actor malicioso ha olfateado el tráfico de red, puede hacerse pasar por un usuario autorizado. Un ataque de denegación de servicio es una clase de ataques en los que el atacante impide que el sistema comprometido realice una actividad legítima o responda al tráfico legítimo. Sin embargo, a diferencia de la suplantación de IP, el atacante no recibirá respuesta del host atacado. Todo en el paquete de datos está autorizado, incluida la dirección IP en el Encabezado del paquete. En los ataques de suplantación de IP, el actor malicioso utiliza paquetes IP que contienen direcciones IP falsas. Los atacantes siguen enviando paquetes IP que contienen direcciones IP falsas hasta que el servidor de red se bloquea.




Consejo profesional: Recuerde el principio de defensa en profundidad. No existe una estrategia perfecta para detener cada tipo de ataque. Puede estratificar su defensa utilizando múltiples estrategias. En este caso, el uso de la encriptación estándar del sector reforzará su Seguridad y le ayudará a defenderse de los ataques DoS en más de un nivel.
Puntos clave

Esta lectura cubrió varios tipos de ataques comunes de Suplantación de IP. Ha aprendido cómo se realiza el sniffing de paquetes y cómo la recopilación de información a partir de la interceptación de transmisiones de datos puede dar a los actores maliciosos oportunidades para la suplantación de IP. Tanto si se trata de un ataque en ruta, un ataque de suplantación de IP o un ataque Smurf, los analistas deben asegurarse de que existen estrategias de mitigación para limitar la amenaza y prevenir las brechas de Seguridad.


---


Un analizador de protocolos de red, a veces denominado sniffer de paquetes o analizador de paquetes, es una herramienta diseñada para capturar y analizar el tráfico de datos dentro de una red. Suelen utilizarse como herramientas de investigación para monitorizar redes e identificar actividades sospechosas. Existe una gran variedad de analizadores de protocolos de red, pero algunos de los más comunes son:

    Analizador de Tráfico NetFlow de SolarWinds

    ManageEngine OpManager

    Observador de redes Azure

    Wireshark

    tcpdump

Esta lectura se centrará exclusivamente en tcpdump, aunque puede aplicar lo que aprenda aquí a muchos de los otros analizadores de protocolos de red que utilizará como analista de ciberseguridad para defenderse de cualquier intrusión en la red. En una próxima actividad, revisará un registro de Tráfico de Datos de tcpdump e identificará un ataque DoS para practicar estas habilidades. 
tcpdump

tcpdump es un analizador de protocolos de red de línea de comandos. Es popular, ligero -lo que significa que utiliza poca memoria y tiene un bajo uso de CPU- y utiliza la biblioteca de código abierto libpcap. tcpdump está basado en texto, lo que significa que todos los comandos de tcpdump se ejecutan en el terminal. También puede instalarse en otros sistemas operativos basados en Unix, como macOS®. Está preinstalado en muchas distribuciones de Linux.

tcpdump proporciona un breve análisis de paquetes y convierte la información clave sobre el tráfico de red en formatos fácilmente legibles por humanos. Imprime información sobre cada paquete directamente en su terminal. tcpdump también muestra la dirección IP de origen, las direcciones IP de destino y los números de puerto que se están utilizando en las comunicaciones. 
Interpretar la salida

tcpdump imprime la salida del comando como los paquetes olfateados en la línea de comandos, y opcionalmente en un archivo de registro, después de ejecutar un comando. La salida de una captura de paquetes contiene muchas piezas de información importante sobre el tráfico de la red.
tipos de información presentados en una captura de paquetes tcpdump.

Alguna de la información que recibe de una captura de paquetes incluye:

    Marca de tiempo: La salida comienza con la marca de tiempo, formateada como horas, minutos, segundos y fracciones de segundo.

    IP de origen: El origen del paquete lo proporciona su dirección IP de origen.

    Puerto de origen: Este número de puerto es donde se originó el paquete.

    IP de destino: La dirección IP de destino es hacia dónde se está transmitiendo el paquete.

    Puerto de destino: Este número de puerto es hacia donde se está transmitiendo el paquete.

Nota: Por defecto, tcpdump intentará resolver las direcciones de host a nombres de host. También sustituirá los números de puerto por servicios comúnmente asociados que utilicen estos puertos.
Usos comunes

tcpdump y otros analizadores de protocolos de red se utilizan habitualmente para capturar y visualizar las comunicaciones de red y para recopilar estadísticas sobre la red, como la solución de problemas de rendimiento de la red. También pueden utilizarse para:

    Establecer una línea de base para los patrones de tráfico de red y las métricas de utilización de la red.

    Detectar e identificar el tráfico malicioso

    Crear alertas personalizadas para enviar las notificaciones adecuadas cuando surjan problemas en la red o amenazas a la seguridad.

    Localizar la mensajería instantánea (MI), el tráfico o los puntos de acceso inalámbricos no autorizados.

Sin embargo, los atacantes también pueden utilizar los analizadores de protocolos de red de forma maliciosa para obtener información sobre una red específica. Por ejemplo, los atacantes pueden capturar paquetes de datos que contengan información confidencial, como nombres de usuario de cuentas y contraseñas. Como analista de ciberseguridad, es importante comprender la finalidad y los usos de los analizadores de protocolos de red.
Puntos clave

Los analizadores de protocolos de red, como tcpdump, son herramientas comunes que pueden utilizarse para supervisar los patrones de tráfico de red e investigar actividades sospechosas. tcpdump es un analizador de protocolos de red de línea de comandos compatible con Linux/Unix y macOS®. Cuando ejecute un comando tcpdump, la herramienta mostrará información sobre el enrutamiento de paquetes, como la marca de tiempo, la dirección IP de origen y el número de puerto, y la dirección IP de destino y el número de puerto. Por desgracia, los atacantes también pueden utilizar analizadores de protocolos de red para capturar paquetes de datos que contengan información confidencial, como nombres de usuario y contraseñas de cuentas

---
# Ejemplo
Resumen de la actividad

En esta actividad, analizará el tráfico DNS e ICMP en tránsito utilizando los datos de una herramienta de análisis de protocolos de red. Identificará qué protocolo de red se utilizó en la evaluación del incidente de ciberseguridad.

En la capa de Internet del Modelo TCP/IP, la IP formatea los paquetes de datos en datagramas IP. La información proporcionada en el datagrama de un paquete IP puede ofrecer a los analistas de seguridad una visión de los paquetes de datos sospechosos en tránsito.

Saber cómo identificar el tráfico potencialmente malicioso en una red puede ayudar a los analistas de ciberseguridad a evaluar los riesgos de seguridad en una red y a reforzar la seguridad de la misma.

Asegúrese de completar esta actividad antes de continuar. El siguiente punto del curso le proporcionará un ejemplo completado para que lo compare con su propio trabajo. 
Escenario

Revise el escenario que aparece a continuación. A continuación, complete las instrucciones paso a paso.

Usted es un analista de ciberseguridad que trabaja en una empresa especializada en la prestación de servicios informáticos para clientes. Varios clientes de clientes informaron de que no podían acceder al sitio web de la empresa cliente www.yummyrecipesforme.com, y vieron el error "puerto de destino inalcanzable" después de esperar a que se cargara la página.

Usted tiene la tarea de analizar la situación y determinar qué protocolo de red se vio afectado durante este incidente. Para empezar, intenta visitar la página web y también recibe el error "puerto de destino inalcanzable" Para solucionar el problema, carga su herramienta de análisis de red, tcpdump, e intenta cargar de nuevo la página web. Para cargar la página web, su navegador envía una consulta a un servidor DNS a través del protocolo UDP para recuperar la dirección IP del nombre de dominio del sitio web; esto forma parte del protocolo DNS. A continuación, su navegador utiliza esta dirección IP como IP de destino para enviar una solicitud HTTPS al servidor web para mostrar la página web El analizador muestra que cuando envía paquetes UDP al servidor DNS, recibe paquetes ICMP que contienen el mensaje de error: "Puerto udp 53 inalcanzable".
log from tcpdump paquete de datos

En el registro tcpdump, se encuentra la siguiente información:

    Las dos primeras líneas del archivo de registro muestran la petición saliente inicial de su ordenador al servidor DNS solicitando la dirección IP de yummyrecipesforme.com. Esta solicitud se envía en un Paquete UDP.

    La tercera y cuarta líneas del registro muestran la respuesta a su paquete UDP. En este caso, la línea ICMP 203.0.113.2 es el inicio del mensaje de error que indica que el paquete UDP no se pudo entregar en el puerto 53 del servidor DNS.

    Delante de cada solicitud y respuesta, encontrará marcas de tiempo que indican cuándo se produjo el incidente. En el registro, ésta es la primera secuencia de números que aparece: 13:24:32.192571. Esto significa que la hora es 13:24, 32,192571 segundos.

    Después de las marcas de tiempo, encontrará las direcciones IP de origen y destino. En la primera línea, donde el paquete UDP viaja desde su navegador hasta el servidor DNS, esta información se muestra como: 192.51.100.15 > 203.0.113.2.dominio. La dirección IP a la izquierda del símbolo mayor que (>) es la dirección de origen, que en este ejemplo es la dirección IP de su ordenador. La dirección IP a la derecha del símbolo mayor que (>) es la dirección IP de destino. En este caso, es la dirección IP del servidor DNS: 203.0.113.2.dominio. Para la respuesta de error ICMP, la dirección de origen es 203.0.113.2 y el destino es la dirección IP de su ordenador 192.51.100.15.

    Después de las direcciones IP de origen y destino, puede haber una serie de detalles adicionales como el protocolo, el número de puerto de origen y las banderas. En la primera línea del registro de errores, el número de identificación de la consulta aparece como: 35084. El signo más después del número de identificación de la consulta indica que hay banderas asociadas al mensaje UDP. La "A?" indica una bandera asociada con la solicitud DNS de un registro A, donde un registro A mapea un nombre de dominio a una dirección IP. La tercera línea muestra el protocolo del mensaje de respuesta al navegador: "ICMP", al que sigue un mensaje de error ICMP.

    El mensaje de error, "puerto udp 53 inalcanzable" se menciona en la última línea. Puerto 53 es un puerto para el servicio DNS. La palabra "inalcanzable" en el mensaje indica que el mensaje UDP que solicitaba una dirección IP para el dominio "www.yummyrecipesforme.com" no llegó al servidor DNS porque no había ningún servicio escuchando en el puerto DNS receptor.

    Las líneas restantes del registro indican que se enviaron paquetes ICMP dos veces más, pero en ambas ocasiones se recibió el mismo error de entrega.

Ahora que ha capturado los paquetes de datos utilizando una herramienta de análisis de red, su trabajo consiste en identificar qué protocolo de red y qué servicio se vieron afectados por este incidente. A continuación, deberá redactar un informe de seguimiento.

Como analista, puede inspeccionar el tráfico de red y los datos de red para determinar qué está causando los problemas relacionados con la red durante los incidentes de ciberseguridad. Más adelante en este curso, demostrará cómo gestionar y resolver incidentes. Por ahora, sólo necesita analizar la situación.

Mientras tanto, este incidente está siendo gestionado por ingenieros de seguridad después de que usted y otros analistas hayan informado del problema a su supervisor directo.
Instrucciones paso a paso

Siga las instrucciones y responda a la pregunta siguiente para completar la actividad. A continuación, pase al siguiente punto del curso para comparar su trabajo con un ejemplar completado.

---

# Ejemplo 2

Resumen de la actividad

En esta actividad, estudiará un escenario en el que un cliente de la empresa para la que trabaja experimenta un problema de seguridad al acceder al sitio web de la empresa. Identificará la causa probable de la interrupción del servicio. A continuación, explicará cómo se produjo el ataque y el impacto negativo que tuvo en el sitio web. 

En este curso, ha aprendido sobre varios ataques de red comunes. Ha aprendido sus nombres, cómo se llevan a cabo y las características de cada ataque desde la perspectiva del objetivo. Comprender cómo afectan los ataques a una red le ayudará a solucionar los problemas de la red de su organización. También le ayudará a tomar medidas para mitigar los daños y proteger una red de futuros ataques. Para repasar los ataques, visite Identificar: Ataques a la red

Asegúrese de completar esta actividad antes de continuar. El siguiente punto del curso le proporcionará un ejemplo completado para que lo compare con su propio trabajo. 
Escenario

Revise el siguiente escenario. A continuación, complete las instrucciones paso a paso.

Usted trabaja como analista de seguridad para una agencia de viajes que anuncia ventas y promociones en el sitio web de la empresa. Los empleados de la empresa acceden regularmente a la página web de ventas de la empresa para buscar paquetes vacacionales que puedan gustar a sus clientes.

Una tarde, recibe una alerta automática de su sistema de supervisión que le indica un problema con el servidor web. Intenta visitar la página web de la empresa, pero recibe un mensaje de error de tiempo de espera de conexión en su navegador.

Utiliza un rastreador de paquetes para capturar los paquetes de datos en tránsito hacia y desde el servidor web. Observa un gran número de solicitudes TCP SYN procedentes de una dirección IP desconocida. El servidor web parece estar desbordado por el volumen de tráfico entrante y está perdiendo su capacidad para responder al número anormalmente elevado de peticiones SYN. Usted sospecha que el servidor está siendo atacado por un actor malicioso. 

Usted desconecta temporalmente el servidor para que la máquina pueda recuperarse y volver a un estado operativo normal. También configura el cortafuegos de la empresa para que bloquee la dirección IP que estaba enviando el número anormal de peticiones SYN. Sabe que su solución de bloqueo de IP no durará mucho, ya que un atacante puede suplantar otras direcciones IP para burlar este bloqueo. Tiene que alertar rápidamente a su jefe sobre este problema y discutir los pasos a seguir para detener a este atacante y evitar que este problema se repita. Tendrá que estar preparado para contarle a su jefe el tipo de ataque que ha descubierto y cómo estaba afectando al servidor web y a los empleados.
Instrucciones paso a paso

Siga las instrucciones y responda a la pregunta para completar la actividad. A continuación, vaya al siguiente punto del curso para comparar su trabajo con un ejemplo completado.

Paso 3: Identificar el tipo de ataque causante de esta interrupción de la Red

Reflexione sobre los tipos de ataques de intrusión en la red que ha conocido hasta ahora en este curso. Como analista de seguridad, identificar el tipo de ataque a la red en función del incidente es el primer paso para gestionar el ataque y prevenir ataques similares en el futuro.

He aquí algunas preguntas a tener en cuenta a la hora de determinar qué tipo de ataque se ha producido:

    ¿Qué entiende actualmente sobre los ataques a la red?

    ¿Qué tipo de ataque provocaría probablemente los síntomas descritos en el escenario?

    ¿Cuál es la diferencia entre una denegación de servicio (DoS) y una denegación de servicio distribuida (DDoS)?

    ¿Por qué el sitio web tarda mucho en cargarse e informa de un error de tiempo de espera de conexión?

Revise la lectura de Wireshark del paso 2 e intente identificar patrones en el tráfico de red registrado. Analice los patrones para determinar qué tipo de ataque de red se ha producido. Escriba su análisis en la sección uno de la plantilla de informe de incidentes de ciberseguridad proporcionada. 

Paso 4: Explicar cómo el ataque está provocando el mal funcionamiento del sitio web

Revise la lectura de Wireshark del paso 2 y, a continuación, escriba su análisis en la sección dos de la plantilla de Informe de Incidentes de Ciberseguridad que se proporciona.

Cuando redacte su informe, hable de los dispositivos y actividades de red implicados en la interrupción. Incluya la siguiente Información en su explicación:

    Describa el ataque. ¿Cuáles son los principales síntomas o características de este tipo específico de ataque? 

    Explique cómo afectó a la red de la organización. ¿Cómo afecta este ataque específico a la red a la página web y a su funcionamiento?

    Describa las posibles consecuencias de este ataque y cómo afecta negativamente a la organización. 

    Opcional: Sugiera posibles formas de asegurar la red para poder evitar este ataque en el futuro.

---

Evaluación del Ejemplar

Compare el ejemplar con su actividad finalizada. Revise su trabajo utilizando cada uno de los criterios del ejemplar. ¿Qué ha hecho bien? ¿En qué puede mejorar? Utilice sus respuestas a estas preguntas como guía para seguir avanzando en el curso.

Nota: El ejemplar representa una posible explicación de los problemas a los que se enfrenta el usuario. Es probable que la suya difiera en ciertos aspectos. Lo importante es que ha identificado los protocolos de red implicados y ha creado un Informe. En su función de analista de seguridad, usted y su Equipo harían la mejor conjetura sobre lo ocurrido y luego investigarían más a fondo para solucionar el Problema y reforzar la seguridad general de su red.

El ejemplo identifica que el mensaje de tiempo de espera de la conexión es el resultado de un ataque DoS. En esta Instancia, el ataque DoS específico es un Ataque de SYN flood.

Para determinarlo, analice los datos presentados en el extracto del archivo de registro adjunto a esta actividad. A continuación, reflexione sobre su conocimiento actual de los ataques de red para identificar qué tipo de ataque se está produciendo en función de los datos disponibles.

Tras identificar un posible tipo de ataque a la red, proceda a explicar cómo llegó a identificar el ataque. A continuación, documente cómo este tipo específico de ataque pudo afectar a la red e incluya una descripción general de cómo el atacante explotó la vulnerabilidad de la red.

Por último, describa cómo este ataque provocó que la página web mostrara el error de tiempo de espera de la conexión.

El ejemplo sólo ofrece un ejemplo de explicación del suceso. Describir un Evento normalmente requiere presentar sus pruebas y explicar cómo llegó a su decisión. Todos los patrones que observe en los registros y datos son fundamentales para determinar el origen y el tipo de ataque a la red. Cuanta más práctica tenga en la identificación de estos patrones, más fácil le resultará detectar los ataques a la red en el momento en que se producen. Esto le permitirá responder a los incidentes con mayor rapidez y eficacia.