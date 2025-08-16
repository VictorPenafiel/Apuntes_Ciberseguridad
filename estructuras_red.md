## Una red es un grupo de dispositivos conectados
¿Qué puerto se utiliza para la Comunicación segura en Internet?
443

hub = concentrador
switch = conmutador

Componentes, dispositivos y diagramas de red
Estado: Traducido automáticamente del Inglés
Traducido automáticamente del Inglés

En esta lectura, revisará los dispositivos y conexiones de red e investigará un diagrama de red sencillo similar a los que utilizan a diario los profesionales de la seguridad de redes.

Una comprensión básica de la arquitectura de red, a veces denominada diseño de red, le ayudará a conocer las vulnerabilidades de seguridad inherentes a todas las redes y cómo los actores maliciosos intentan explotarlas. Empecemos

Dispositivos de red

Los dispositivos de red mantienen información y servicios para los usuarios de una red. Estos dispositivos se conectan a través de conexiones cableadas e inalámbricas. Tras establecer una conexión con la red, los dispositivos envían paquetes de datos. Los paquetes de datos proporcionan información sobre el origen y el destino de los datos. Así es como se envía y recibe la información a través de los distintos dispositivos de una red.

La red es la infraestructura general que permite a los dispositivos comunicarse entre sí. Los dispositivos de red son vehículos especializados, como enrutadores y conmutadores, que gestionan lo que se envía y recibe a través de la red. Además, dispositivos como ordenadores y teléfonos se conectan a la red a través de dispositivos de red. 

Nota: en este diagrama, un router se conecta a Internet a través de un módem, que le proporciona su proveedor de servicios de Internet (ISP). El cortafuegos es un dispositivo de seguridad que supervisa el tráfico entrante y saliente de la red. A continuación, el router dirige el tráfico a los dispositivos de tu red doméstica, que pueden incluir ordenadores, portátiles, smartphones, tabletas, impresoras y otros aparatos. Aquí puedes imaginar que el servidor es un servidor de archivos. Todos los dispositivos de esta red pueden acceder a los archivos de este servidor. Este diagrama también incluye un switch, que es un dispositivo opcional que se puede utilizar para conectar más dispositivos a la red proporcionando puertos adicionales y conexiones Ethernet. Además, hay 2 routers conectados al switch para equilibrar la carga y mejorar el rendimiento de la red.

Dispositivos y ordenadores de sobremesa

La mayoría de los usuarios de Internet están familiarizados con los dispositivos cotidianos, como ordenadores personales, portátiles, teléfonos móviles y tabletas. Cada dispositivo y ordenador de sobremesa tiene una dirección MAC y una dirección IP únicas, que lo identifican en la red. También tienen una interfaz de red que envía y recibe paquetes de datos. Estos dispositivos pueden conectarse a la red mediante un cable fijo o una conexión inalámbrica.
Cortafuegos

Un cortafuegos es un dispositivo de seguridad de red que supervisa el tráfico hacia o desde su red. Es como la primera línea de defensa. Los cortafuegos también pueden restringir el tráfico de red específico entrante y saliente. La organización configura las reglas de seguridad del cortafuegos. Los cortafuegos suelen situarse entre la red interna segura y controlada y los recursos de red no fiables fuera de la organización, como Internet. Recuerda, sin embargo, que los cortafuegos son sólo una línea de defensa en el panorama de la ciberseguridad.
Servidores

Losservidores proporcionan información y servicios para dispositivos como ordenadores, dispositivos domésticos inteligentes y teléfonos inteligentes en la red. Los dispositivos que se conectan a un servidor se denominan clientes. El siguiente gráfico esboza este modelo, que se denomina modelo cliente-servidor. En este modelo, los clientes envían peticiones de información y servicios al servidor. El servidor realiza las peticiones para los clientes. Algunos ejemplos comunes son los servidores DNS, que realizan búsquedas de nombres de dominio para sitios de Internet, los servidores de archivos, que almacenan y recuperan archivos de una base de datos, y los servidores de correo corporativo, que organizan el correo de una empresa.
Concentradores y conmutadores

## Hub 
(concentradores) como los conmutadores dirigen el tráfico de una red local. Un concentrador es un dispositivo que proporciona un punto común de conexión para todos los dispositivos conectados directamente a él. Además, los concentradores repiten toda la información a todos los puertos. Desde el punto de vista de la seguridad, esto hace que los concentradores sean vulnerables a las escuchas. Por este motivo, los concentradores no se utilizan con tanta frecuencia en las redes modernas; la mayoría de las organizaciones utilizan conmutadores en su lugar. Los concentradores suelen utilizarse en redes limitadas, como las oficinas domésticas.

## Switch 
(conmutadores) son la opción preferida en la mayoría de las redes. Un conmutador reenvía paquetes entre dispositivos conectados directamente a él. Analizan la dirección de destino de cada paquete de datos y lo envían al dispositivo previsto. Los conmutadores mantienen una tabla de direcciones MAC que coteja las direcciones MAC de los dispositivos de la red con los números de puerto del conmutador y reenvía los paquetes de datos entrantes según la dirección MAC de destino. Los conmutadores forman parte de la capa de vínculo de datos en el Modelo TCP/IP. En general, los conmutadores mejoran el rendimiento y la seguridad.


Routers
Losrouters conectan redes y dirigen el tráfico, basándose en la dirección IP de la red de destino. Los routers permiten que los dispositivos de diferentes redes se comuniquen entre sí. En el Modelo TCP/IP, los routers forman parte de la capa de red. La dirección IP de la red de destino está contenida en la cabecera IP. El router lee la información de la cabecera IP y reenvía el paquete al siguiente router en la ruta hacia el destino. Esto continúa hasta que el paquete llega a la red de destino. Los routers también pueden incluir una función de cortafuegos que permite o bloquea el tráfico entrante basándose en la información de la transmisión. Esto impide que el tráfico malicioso entre en la red privada y dañe la red de área local.
Módems y puntos de acceso inalámbricos

Los módems suelen conectar su casa u oficina con un proveedor de servicios de Internet (ISP). Los ISP proporcionan conexión a Internet a través de líneas telefónicas, cables coaxiales o cables de fibra óptica. Los módems reciben transmisiones o señales digitales de Internet y las convierten en un formato digital compatible con la conexión física que le proporciona su ISP. Normalmente, los módems se conectan a un router que toma las transmisiones descodificadas y las envía a la red local.

Nota: las redes empresariales que utilizan las grandes organizaciones para conectar a sus usuarios y dispositivos suelen emplear otras tecnologías de banda ancha para gestionar el tráfico de gran volumen, en lugar de utilizar un módem.

Punto de acceso inalámbrico

Un punto de acceso inalámbrico envía y recibe señales digitales a través de ondas de radio creando una red inalámbrica. Los dispositivos con adaptadores inalámbricos se conectan al punto de acceso mediante Wi-Fi. Wi-Fi hace referencia a un conjunto de estándares que utilizan los dispositivos de red para comunicarse de forma inalámbrica. Los puntos de acceso inalámbricos y los dispositivos conectados a ellos utilizan protocolos Wi-Fi para enviar datos a través de ondas de radio, donde se envían a enrutadores y conmutadores y se dirigen a lo largo de la ruta hasta su destino final.
Uso de diagramas de red como analista de seguridad

Los diagramas de red permiten a los administradores de red y al personal de seguridad imaginar la arquitectura y el diseño de la red privada de su organización.

Los diagramas de red son mapas que muestran los dispositivos de la red y cómo se conectan. Los diagramas de red utilizan pequeños gráficos representativos para representar cada dispositivo de la red y líneas de puntos para mostrar cómo se conecta cada dispositivo entre sí. Mediante el estudio de los diagramas de red, los analistas de seguridad desarrollan y perfeccionan sus estrategias para proteger las arquitecturas de red.
Puntos clave

En el modelo cliente-servidor, el cliente solicita información y servicios al servidor, y el servidor realiza las solicitudes para los clientes. Los dispositivos de red incluyen enrutadores, estaciones de trabajo, servidores, concentradores, conmutadores y módems. Los analistas de seguridad utilizan diagramas de red para visualizar la arquitectura de red.

 Computación en la nube y redes definidas por software
Estado: Traducido automáticamente del Inglés
Traducido automáticamente del Inglés
Información:
Este elemento incluye contenido que aún no se tradujo a tu idioma preferido.

En esta sección del curso, ha estado aprendiendo la arquitectura básica de las redes. Ha aprendido cómo los dispositivos físicos de red como estaciones de trabajo, servidores, routers y switches se conectan entre sí para crear una red. Las redes pueden abarcar áreas geográficas pequeñas, como es el caso de una red de área local (LAN). O pueden abarcar un área geográfica extensa, como una ciudad, un estado o un país, como es el caso de una red de área extensa (WAN). También ha aprendido sobre las redes en la nube y cómo ha crecido la computación en la nube en los últimos años.

En esta lectura, examinará más a fondo los conceptos de computación en la nube y redes informáticas en la nube. También conocerá las redes híbridas y las redes definidas por software, así como las ventajas que ofrecen. Esta lectura también cubrirá los beneficios de alojar redes en la nube y por qué el alojamiento en la nube es beneficioso para las grandes organizaciones.
Procesos de computación en la nube

Las redes tradicionales se denominan redes on-premise, lo que significa que todos los dispositivos utilizados para las operaciones de red se mantienen en una ubicación física propiedad de la empresa, como en un edificio de oficinas, por ejemplo. La computación en la nube, sin embargo, se refiere a la práctica de utilizar servidores, aplicaciones y servicios de red remotos que se alojan en Internet en lugar de en un lugar físico propiedad de la empresa.

Un proveedor de servicios en la nube (PSN) es una empresa que ofrece servicios de computación en la nube. Estas empresas poseen grandes centros de datos en ubicaciones de todo el mundo que albergan millones de servidores. Los centros de datos proporcionan servicios tecnológicos, como almacenamiento y computación, a una escala tan grande que pueden vender sus servicios a otras empresas por una tarifa. Las empresas pueden pagar por el almacenamiento y los servicios que necesitan y consumirlos a través de la interfaz de programación de aplicaciones (API) o la consola web del CSP.

Los CSP ofrecen tres categorías principales de servicios:

    Software como servicio (SaaS ) se refiere a conjuntos de software operados por el CSP que una empresa puede utilizar de forma remota sin alojar el software.

    Lainfraestructura como servicio (IaaS) se refiere al uso de componentes informáticos virtuales ofrecidos por el CSP. Estos incluyen contenedores virtuales y almacenamiento que se configuran de forma remota a través de la API o la consola web del CSP. Los servicios de computación en la nube y almacenamiento pueden utilizarse para operar aplicaciones existentes y otras cargas de trabajo tecnológicas sin modificaciones significativas. Las aplicaciones existentes pueden modificarse para aprovechar las características de disponibilidad, rendimiento y seguridad que son exclusivas de los servicios del proveedor de la nube.

    Laplataforma como servicio (PaaS ) hace referencia a las herramientas que los desarrolladores de aplicaciones pueden utilizar para diseñar aplicaciones personalizadas para su empresa. Las aplicaciones personalizadas se diseñan y se accede a ellas en la nube y se utilizan para las necesidades empresariales específicas de una empresa.

Diferencias entre IaaS, PaaS y SaaS y cómo cada uno se conecta a un centro de datos físico.
Entornos de nube híbrida

Cuando las organizaciones utilizan los servicios de un CSP además de sus ordenadores, redes y almacenamiento locales, se habla de un entorno de nube híbrida. Cuando las organizaciones utilizan más de un CSP, se denomina entorno de nubes múltiples. La gran mayoría de las organizaciones utilizan entornos de nube híbrida para reducir costes y mantener el control sobre los recursos de red.
Redes definidas por software

Los CSP ofrecen herramientas de redes similares a los dispositivos físicos que ha conocido en esta sección del curso. A continuación, repasará las redes definidas por software en la nube. Las redes definidas por software (SDN) están formadas por dispositivos y servicios de red virtuales. Al igual que las CSP proporcionan computadoras virtuales, muchas SDN también proporcionan conmutadores virtuales, routers, firewalls y mucho más. La mayoría de los dispositivos de hardware de red modernos también son compatibles con la virtualización de redes y las redes definidas por software. Esto significa que los Switch y routers físicos utilizan software para realizar el enrutamiento de paquetes. En el caso de las redes en la nube, las herramientas SDN se alojan en servidores situados en el centro de datos del CSP.
Beneficios de la computación en la nube y las redes definidas por software 

Tres de las principales razones por las que la computación en la nube resulta tan atractiva para las empresas son la Confiabilidad, la disminución de los costes y el aumento de la escalabilidad. 
Confiabilidad

La fiabilidad en la computación en la nube se basa en el grado de disponibilidad de los servicios y Recursos de la nube, la seguridad de las conexiones y la frecuencia con la que los servicios funcionan eficazmente. La computación en la nube permite a empleados y Clientes acceder a los Recursos que necesitan de forma constante y con una interrupción mínima. 
Costes

Tradicionalmente, las empresas han tenido que proporcionar su propia infraestructura de red, al menos para las conexiones a Internet. Esto suponía unos costes iniciales potencialmente significativos para las empresas. Sin embargo, como los CSP disponen de centros de datos tan grandes, pueden ofrecer dispositivos y servicios virtuales a una fracción del coste que supone para las empresas instalar, parchear, actualizar y gestionar ellas mismas los componentes y el software.
Escalabilidad

Otro reto al que se enfrentan las empresas con la informática tradicional es la escalabilidad. Cuando las organizaciones experimentan un aumento de sus necesidades empresariales, pueden verse obligadas a comprar más equipos y software para mantener el ritmo. Pero, ¿qué ocurre si el negocio disminuye poco después? Es posible que ya no tengan negocio para justificar el coste en el que han incurrido por los componentes actualizados. Los CSP reducen este Riesgo facilitando el consumo de servicios en un Modelo de utilidad elástico según las necesidades. Esto significa que las empresas sólo pagan por lo que necesitan cuando lo necesitan.

Los cambios pueden realizarse rápidamente a través de los CSP, las API o la consola web, mucho más rápido que si los técnicos de red tuvieran que comprar su propio hardware y configurarlo. Por ejemplo, si una empresa necesita protegerse contra una amenaza a su red, los cortafuegos de aplicaciones web (WAF), los sistemas de detección/protección de intrusiones (IDS/IPS) o los cortafuegos L3/L4 pueden configurarse rápidamente siempre que sea necesario, lo que mejora el rendimiento y la seguridad de la red.
Puntos clave

En esta lectura, ha aprendido más sobre la computación en la nube y las redes informáticas en la nube. Ha aprendido que los CSP son empresas propietarias de grandes centros de datos que albergan millones de servidores en ubicaciones de todo el mundo y que luego proporcionan servicios de tecnología moderna, como computación, almacenamiento y redes, a través de Internet. Las SDN son un enfoque de la gestión de redes. Las SDN permiten configuraciones de red dinámicas y eficientes desde el punto de vista de la programación para mejorar el rendimiento y la supervisión de la red. Esto las asemeja más a la computación en la nube que a la gestión tradicional de redes. Las organizaciones pueden mejorar la Confiabilidad, ahorrar Costos y escalar rápidamente utilizando CSPs para proveer servicios de redes en lugar de construir y mantener su propia infraestructura de redes. 
Recursos para más Información

Si desea más información sobre la computación en la nube y los servicios que ofrece, puede consultar 