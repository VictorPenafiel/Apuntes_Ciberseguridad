
### El Endurecimiento (Security hardening) de seguridad es el proceso de reforzar un sistema para reducir su vulnerabilidad y superficie de ataque.

### superficie de ataque de un sistema: Todas las vulnerabilidades potenciales que un Agente de amenaza podría explotar se denominan . 

### VPN, HTTPS y no ocupar redes wifi sin encriptacion para proteger sniffing de paquetes

---

Ataques de fuerza bruta
 es un proceso de ensayo y error para descubrir información privada. Existen diferentes tipos de ataques de fuerza bruta que los actores maliciosos utilizan para adivinar contraseñas, entre ellos:

    Ataques de fuerza bruta simples. Cuando los atacantes intentan adivinar las credenciales de inicio de sesión de un usuario, se considera un ataque de fuerza bruta simple. Pueden hacerlo introduciendo cualquier combinación de nombres de usuario y contraseñas que se les ocurra hasta encontrar la que funcione.

    Los ataques de diccionario utilizan una técnica similar. En los ataques de diccionario, los atacantes utilizan una lista de contraseñas de uso común y credenciales robadas en violaciones anteriores para acceder a un sistema. Se denominan ataques de diccionario porque los atacantes utilizaban originalmente una lista de palabras del diccionario para adivinar las contraseñas, antes de que las reglas de contraseñas complejas se convirtieran en una práctica habitual de Seguridad.

Antes de que se produzca un ataque de fuerza bruta u otro incidente de ciberseguridad, las empresas pueden realizar una serie de pruebas en su red o en sus aplicaciones web para evaluar las vulnerabilidades. Los analistas pueden utilizar máquinas virtuales y cajas de arena para probar archivos sospechosos, comprobar vulnerabilidades antes de que se produzca un evento o simular un incidente de ciberseguridad.
Máquinas virtuales (VM)

Las máquinas virtuales (VM) son versiones de software de las computadoras físicas. Las VM proporcionan una capa adicional de Seguridad para una organización porque pueden utilizarse para ejecutar código en un entorno aislado, evitando que el código malicioso afecte al resto de la computadora o del sistema. Las VM también pueden eliminarse y sustituirse por una imagen prístina después de probar software malicioso.

Las VM son útiles cuando se investigan máquinas potencialmente infectadas o se ejecuta software malicioso en un entorno restringido. El uso de una VM puede evitar daños en su sistema en el caso de que sus herramientas se utilicen de forma inadecuada. Las VM también le ofrecen la posibilidad de volver a un estado anterior. Sin embargo, las máquinas virtuales conllevan algunos Riesgos. Todavía existe un pequeño Riesgo de que un programa malicioso pueda escapar a la virtualización y acceder a la máquina anfitriona.

Puede probar y explorar aplicaciones fácilmente con las máquinas virtuales, y es fácil cambiar entre diferentes máquinas virtuales desde su computadora. Esto también puede ayudar a agilizar muchas tareas de Seguridad.
Espacios aislados

Un entorno aislado es un tipo de entorno de pruebas que le permite ejecutar software o programas separados de su red. Suelen utilizarse para probar parches, Identificar y solucionar errores o Detectar vulnerabilidades de ciberseguridad. Los espacios aislados también pueden utilizarse para evaluar software sospechoso, evaluar archivos que contienen código malicioso y simular escenarios de ataque.

Los cajones de arena pueden ser ordenadores físicos autónomos que no están conectados a una red; sin embargo, a menudo es más rentable y económico utilizar software o máquinas virtuales basadas en la nube como entornos de cajones de arena. Tenga en cuenta que algunos autores de software malicioso saben cómo escribir código para detectar si el software malicioso se ejecuta en una VM o en un entorno de caja de arena. Los atacantes pueden programar su software malicioso para que se comporte como software inofensivo cuando se ejecuta dentro de este tipo de entornos de pruebas. 
Medidas de prevención

Algunas medidas comunes que las organizaciones utilizan para evitar que se produzcan ataques de fuerza bruta y ataques similares incluyen:

    Salting y hash: El hash convierte la información en un valor único que puede utilizarse para determinar su integridad. Es una función unidireccional, lo que significa que es imposible desencriptar y obtener el texto original. El salting añade caracteres aleatorios a las contraseñas hash. Esto aumenta la Longitud y la complejidad de los valores hash, haciéndolos más seguros.

    Autenticación de múltiples factores (MFA) y autenticación de dos factores (2FA): MFA es una medida de seguridad que requiere que un usuario verifique su identidad de dos o más formas para acceder a un sistema o red. Esta autenticación se realiza mediante una combinación de factores de autenticación: un nombre de usuario y una contraseña, huellas dactilares, reconocimiento facial o una contraseña de un solo uso (OTP) enviada a un número de teléfono o a un correo electrónico. la 2FA es similar a la MFA, salvo que sólo utiliza dos formas de verificación.

    CAPTCHA y reCAPTCHA: CAPTCHA son las siglas de Completely Automated Public Turing test to tell Computers and Humans Apart (Prueba de Turing pública completamente automatizada para distinguir entre ordenadores y humanos). Pide a los usuarios que completen una sencilla prueba que demuestra que son humanos. Esto ayuda a evitar que el software intente forzar una contraseña. reCAPTCHA es un servicio CAPTCHA gratuito de Google que ayuda a proteger los sitios web de bots y software malicioso.

    Políticas de contraseñas: Las organizaciones utilizan políticas de contraseñas para estandarizar las buenas prácticas de contraseñas en toda la empresa. Las políticas pueden incluir directrices sobre lo compleja que debe ser una contraseña, la frecuencia con la que los usuarios deben actualizar las contraseñas, si las contraseñas se pueden reutilizar o no, y si hay límites en el número de veces que un usuario puede intentar iniciar sesión antes de que se suspenda su cuenta.

Puntos clave

Los ataques de fuerza bruta son un proceso de ensayo y error para adivinar contraseñas. Los ataques pueden lanzarse manualmente o mediante herramientas de software. Los métodos incluyen ataques de fuerza bruta simples y ataques de diccionario. Para protegerse contra los ataques de fuerza bruta, los analistas de ciberseguridad pueden utilizar sandboxes para probar archivos sospechosos, comprobar vulnerabilidades o simular ataques reales y máquinas virtuales para realizar pruebas de vulnerabilidad. Algunas medidas comunes para prevenir los ataques de fuerza bruta incluyen: hash y salting, MFA y/o 2FA, CAPTCHA y reCAPTCHA, y políticas de contraseña.

---

Resumen de la actividad

En esta actividad, asumirás el papel de un analista de ciberseguridad que trabaja para una empresa que aloja el sitio web de cocina, yummyrecipesforme.com. Los visitantes del sitio web experimentan un problema de seguridad al cargar la página web principal. Tu trabajo consiste en investigar, identificar, documentar y recomendar una solución al problema de seguridad.

Cuando investigue el evento de seguridad, revisará un registro tcpdump. Tendrás que identificar los Protocolos de red utilizados para establecer la conexión entre el usuario y la página web. Los Protocolos de red son las reglas y estándares de comunicación que los dispositivos en red utilizan para transmitir datos. Desafortunadamente, los actores maliciosos también pueden utilizar protocolos de red para invadir y atacar redes privadas. Saber identificar los protocolos utilizados habitualmente en los ataques le ayudará a proteger la red de su organización contra este tipo de eventos de seguridad.

Para completar la tarea, también tendrá que documentar lo que ocurrió durante el incidente de seguridad. A continuación, recomendará una medida de seguridad para prevenir problemas de seguridad similares en el futuro.

Asegúrese de completar esta actividad antes de continuar. El siguiente punto del curso le proporcionará un ejemplo completado para que lo compare con su propio trabajo. 
Escenario

Revise el escenario que aparece a continuación. Luego complete las instrucciones paso a paso.

Usted es un analista de ciberseguridad para yummyrecipesforme.com, un sitio web que vende recetas y libros de cocina. Un antiguo empleado ha decidido atraer a los usuarios a un sitio web falso con malware. 

El antiguo empleado/hacker ejecutó un ataque de fuerza bruta para obtener acceso al host web. Introdujeron repetidamente varias contraseñas predeterminadas conocidas para la cuenta administrativa hasta que acertaron con la correcta. Una vez obtenidas las credenciales de inicio de sesión, pudieron acceder al panel de administración y cambiar el código fuente del sitio web. Incrustaron una función javascript en el código fuente que pedía a los visitantes que descargaran y ejecutaran un archivo al visitar el sitio web. Después de incrustar el programa malicioso, el hacker cambió la contraseña de la cuenta administrativa. Cuando los clientes descargaban el archivo, eran redirigidos a una versión falsa del sitio web que contenía el programa malicioso. 

Varias horas después del ataque, varios clientes enviaron correos electrónicos al servicio de asistencia de yummyrecipesforme. Se quejaban de que el sitio web de la empresa les había incitado a descargar un archivo para acceder a recetas gratuitas. Los clientes afirmaron que, tras ejecutar el archivo, la dirección del sitio web cambió y sus ordenadores personales empezaron a funcionar más lentamente.

En respuesta a este incidente, el propietario del sitio web intenta acceder al panel de administración, pero no lo consigue, por lo que se pone en contacto con el proveedor de alojamiento del sitio web. Usted y otros analistas de Ciberseguridad reciben el encargo de investigar este incidente de seguridad.

Para abordar el incidente, creas un entorno sandbox para observar el comportamiento sospechoso del sitio web. Ejecutas el analizador de protocolos de red tcpdump y escribes la URL del sitio web, yummyrecipesforme.com. En cuanto se carga el sitio web, se le pide que descargue un archivo ejecutable para actualizar su navegador. Aceptas la descarga y dejas que se ejecute el archivo. Entonces observa que su navegador le redirige a una URL diferente, greatrecipesforme.com, que contiene el malware.

Los registros muestran el siguiente proceso

    El navegador inicia una petición DNS: Solicita la dirección IP de la URL yummyrecipesforme.com al servidor DNS.

    El DNS responde con la dirección IP correcta.

    El navegador inicia una petición HTTP: Solicita la página web yummyrecipesforme.com utilizando la dirección IP enviada por el servidor DNS.

    El navegador inicia la descarga del malware.

    El navegador inicia una petición DNS para recetasriquitasforme.com.

    El servidor DNS responde con la dirección IP de greatrecipesforme.com.

    El navegador inicia una petición HTTP a la dirección IP de greatrecipesforme.com.

Un analista senior confirma que el sitio web ha sido comprometido. El analista comprueba el código fuente del sitio web. Observan que se ha añadido código javascript para pedir a los visitantes del sitio web que descarguen un archivo ejecutable. El análisis del archivo descargado encontró un script que redirige los navegadores de los visitantes de yummyrecipesforme.com a greatrecipesforme.com.

El equipo de ciberseguridad informa de que el servidor web fue afectado por un ataque de fuerza bruta. El hacker descontento pudo adivinar fácilmente la contraseña porque la contraseña de administrador seguía siendo la contraseña por defecto. Además, no había controles para prevenir un ataque de fuerza bruta.

Tu trabajo es documentar el incidente en detalle, incluyendo la identificación de los protocolos de red utilizados para establecer la conexión entre el usuario y el sitio web. También debes recomendar una acción de seguridad a tomar para prevenir ataques de fuerza bruta en el futuro.
Instrucciones paso a paso

Siga las instrucciones y responda a la siguiente pregunta para completar la actividad. A continuación, vaya al siguiente elemento del curso para comparar su trabajo con un ejemplo completado.

Paso 3: Identificar el protocolo de red implicado en el incidente

Como uno de los analistas de ciberseguridad en este escenario, se le ha encomendado la tarea de redactar un informe de incidente para este evento de seguridad. Utilizando el archivo de registro tcpdump, determine qué protocolo de red se identifica en las capturas de paquetes durante la investigación. Utilizará lo que aprendió sobre las cuatro capas del Modelo TCP/IP y qué protocolos ocurren en cada capa. Si es necesario, puede revisar el vídeo
 y la lectura sobre el Modelo TCP/IP

 para utilizarlos como guías para su respuesta. A continuación, revise el registro de tráfico tcpdump y anote qué protocolo ha identificado en la primera sección de la plantilla de informe de incidentes de seguridad.
Paso 4: Documente el incidente

Resuma el incidente en la segunda sección del informe. Proporcione tantos detalles y hechos como sea posible en su documentación. Al redactar la documentación, asegúrese de:

    Evite utilizar un lenguaje emocional fuerte (bueno, terrible, pésimo, etc.).

    Incluya tantos hechos sobre el asunto como pueda, incluyendo dónde ocurrió el incidente, cómo sucedió, si alguien lo presenció, cómo se descubrió, etc.

    Indique sus fuentes de información y pruebas.

Redactar una documentación precisa y detallada de los incidentes de ciberseguridad puede servir como punto de referencia para otros analistas de ciberseguridad. Además, una documentación de calidad puede utilizarse para educar a otros empleados sobre las medidas de ciberseguridad adoptadas en la empresa cuando se producen incidentes y puede ayudar a las empresas a cumplir con las distintas auditorías de seguridad.
Paso 5: Recomiende una solución para los ataques de fuerza bruta

Tras documentar el incidente, escriba una recomendación para ayudar a su organización a prevenir los ataques de fuerza bruta en el futuro.

Algunos de los métodos de seguridad más utilizados para prevenir los ataques de fuerza bruta son:

    Exigir contraseñas seguras

    Imponer la Autenticación de dos factores (2FA)

    Supervisar los intentos de inicio de sesión

    Exigir cambios de contraseña más frecuentes

    Impedir el uso de contraseñas anteriores

    Limitar el número de intentos de inicio de sesión

Seleccione una medida de seguridad y explique por qué es eficaz en la sección tres de la plantilla de informe sobre incidentes de seguridad.

Cuantas más medidas de seguridad se apliquen, menos probabilidades habrá de que un actor malintencionado pueda acceder a información confidencial.

Evaluación del ejemplar

Compare el ejemplar con su actividad finalizada. Revise su trabajo utilizando cada uno de los criterios del ejemplar. ¿Qué hizo bien? ¿En qué puede mejorar? Utilice sus respuestas a estas preguntas como guía para seguir avanzando en el curso. 

Nota: El ejemplar representa una posible explicación de los problemas a los que se enfrentan los usuarios finales. Es probable que la suya difiera en ciertos aspectos. Lo importante es que usted identificó los protocolos de red implicados y creó un Informe. En su función de analista de seguridad, usted y su Equipo documentarían cualquier Problema que se produzca en la red y propondrían soluciones para ayudar a evitar que se produzcan los mismos problemas en el futuro. Una documentación de buena calidad puede ahorrarle tiempo a usted y a su organización y, potencialmente, gestionar el ataque desde el principio.
Línea decorativa multicolor

En primer lugar, analice el registro de tráfico DNS y HTTP para identificar un protocolo de red. A continuación, documente el incidente de ciberseguridad. Por último, recomiende una medida de Seguridad que su organización podría implementar para prevenir ataques de fuerza bruta en el futuro. La creación de este proceso ayudará, a su vez, a mejorar la postura de Seguridad de la organización.

Acompañe la actividad con un ejemplo de documentación profesional que incluya lo siguiente:

    Un protocolo de red identificado durante la investigación.

    Documentación del Incidente

    Una medida de Seguridad recomendada

Puntos clave

Como analista de seguridad, es posible que no siempre sepa exactamente cuál es la causa principal de un problema de red o de un posible ataque. Pero ser capaz de analizar los protocolos implicados le ayudará a hacer una suposición informada sobre lo ocurrido. Esto le permitirá a usted y a su Equipo comenzar a resolver el Problema. 

---

Aplicaciones de Seguridad de red
Estado: Traducido automáticamente del Inglés
Traducido automáticamente del Inglés

Esta sección del curso trata el tema del endurecimiento de la red y su supervisión. Cada dispositivo, herramienta o estrategia de seguridad puesta en marcha por los analistas de seguridad protege -o endurece- aún más la red hasta que el propietario de la red está satisfecho con el nivel de seguridad. Este enfoque de añadir capas de seguridad a una red se conoce como defensa en profundidad.

En esta lectura, va a conocer la Función de cuatro dispositivos utilizados para proteger una red: cortafuegos, sistemas de detección de intrusiones, sistemas de prevención de intrusiones y herramientas de gestión de incidentes y eventos de seguridad. Los profesionales de la Seguridad de red tienen la opción de utilizar cualquiera de estos dispositivos y herramientas, o todos ellos, en función del nivel de seguridad que esperen alcanzar. 

En esta lectura se analizarán los beneficios de la Seguridad por capas. Cada herramienta mencionada es una capa adicional de defensa que puede endurecer una red de forma incremental, empezando por el nivel mínimo de seguridad (proporcionado sólo por un cortafuegos), hasta el nivel más alto de seguridad (proporcionado por la combinación de un cortafuegos, un dispositivo de detección y prevención de intrusiones y el monitoreo de eventos de seguridad). 
Imagen que muestra las diferencias entre un cortafuegos, un IPS y un IDS.

Tome nota de dónde se encuentra cada herramienta en la red. Cada herramienta tiene su propio lugar en la arquitectura de la red. Los analistas de seguridad deben comprender las topologías de red que se muestran en los diagramas a lo largo de esta lectura.
Firewall

Hasta ahora en este curso, ha aprendido sobre los firewalls sin estado, los firewalls con estado y los firewalls de nueva generación (NGFW), así como las ventajas de seguridad de cada uno de ellos.

La mayoría de los firewalls son similares en sus funciones básicas. Los firewalls permiten o bloquean el tráfico basándose en un conjunto de reglas. Cuando los paquetes de datos entran en una red, se inspecciona el encabezado del paquete y se permite o deniega en función de su número de puerto. Los NGFW también pueden inspeccionar la carga útil de los paquetes. Cada sistema debe tener su propio firewall, independientemente del cortafuegos de la red.
Un cortafuegos rodeado de guiones que protege la red interna del tráfico de Internet que entra por el modo.
Sistema de detección de intrusiones 

Un Sistema de detección de intrusiones (IDS) es una aplicación que monitoriza la actividad del sistema y alerta sobre posibles intrusiones. Un IDS alerta a los administradores basándose en la firma del tráfico malicioso.

El IDS está configurado para detectar ataques conocidos. Los sistemas IDS suelen olfatear los paquetes de datos mientras se desplazan por la red y los analizan en busca de las características de ataques conocidos. Algunos sistemas IDS revisan no sólo en busca de firmas de ataques conocidos, sino también de anomalías que podrían ser el signo de una actividad maliciosa. Cuando el IDS descubre una anomalía, envía una alerta al administrador de la red, que puede investigar más a fondo.

Las limitaciones de los sistemas IDS son que sólo pueden buscar ataques conocidos o anomalías evidentes. Los ataques nuevos y sofisticados podrían no ser detectados. La otra limitación es que el IDS no detiene realmente el tráfico entrante si detecta algo raro. Depende del administrador de la red detectar la actividad maliciosa antes de que cause algún daño a la red.
Un IDS rodea con un círculo la imagen de un conmutador, que se sitúa entre un cortafuegos y la red.

Cuando se combina con un firewall, un IDS añade otra capa de defensa. El IDS se coloca detrás del firewall y antes de entrar en la LAN, lo que permite al IDS analizar los flujos de Datos después de que el Tráfico de red no permitido por el firewall haya sido filtrado. Esto se hace para reducir el ruido en las alertas del IDS, también denominadas falsos positivos.
Sistema de prevención de intrusiones 

Un Sistema de prevención de intrusiones (IPS ) es una aplicación que monitoriza la actividad del sistema en busca de actividades intrusivas y toma medidas para detenerlas. Ofrece incluso más protección que un IDS porque detiene activamente las anomalías cuando las detecta, a diferencia del IDS que simplemente informa de la anomalía a un administrador de red.

Un IPS busca firmas de ataques conocidos y anomalías en los Datos. Un IPS informa de la anomalía a los analistas de seguridad y bloquea un remitente específico o elimina los paquetes de red que parecen sospechosos.
Un IPS se sitúa entre un cortafuegos y la red interna.

El IPS (como un IDS) se sitúa detrás del firewall en la arquitectura de red. Esto ofrece un alto nivel de seguridad porque los flujos de datos arriesgados se interrumpen incluso antes de que lleguen a las partes sensibles de la red. Sin embargo, una limitación potencial es que está en línea: Si se rompe, se interrumpe la conexión entre la red privada e Internet. Otra limitación de los IPS es la posibilidad de que se produzcan falsos positivos, lo que puede hacer que se interrumpa el tráfico legítimo.
Dispositivos de captura de paquetes completos

Los dispositivos de captura de paquetes completos pueden ser increíblemente útiles para los administradores de redes y los profesionales de la Seguridad. Estos dispositivos le permiten registrar y analizar todos los Datos que se transmiten a través de su red. También ayudan a investigar las alertas creadas por un IDS. 
Administración de información y eventos de seguridad 

Un sistema de administración de información y eventos de seguridad (SIEM ) es una aplicación que recopila y analiza los datos de registro para supervisar las actividades críticas de una organización. Las herramientas SIEM trabajan en tiempo real para informar de las actividades sospechosas en un panel centralizado. Las herramientas SIEM analizan además los datos de registro de red procedentes de IDS, IPS, cortafuegos, VPN, proxies y registros DNS. Las herramientas SIEM son una forma de agregar los datos de los eventos de seguridad para que aparezcan todos en un mismo lugar y puedan ser analizados por los analistas de seguridad. Esto se conoce como un panel único de cristal. 

A continuación, puede revisar un ejemplo de un panel de control de la herramienta SIEM de Google Nube, Chronicle. Chronicle es una herramienta nativa de la nube diseñada para retener, analizar y buscar datos.
Imagen del cuadro de mandos de la Crónica

Splunk es otra herramienta SIEM común. Splunk ofrece diferentes opciones de herramientas SIEM: Splunk Enterprise y Splunk Cloud. Ambas opciones incluyen cuadros de mando detallados que ayudan a los profesionales de la Seguridad a revisar y analizar los datos de una organización. También hay otras herramientas SIEM similares disponibles, y es importante que los profesionales de la Seguridad investiguen las diferentes herramientas para determinar cuál es la más beneficiosa para la organización.

Una herramienta SIEM no sustituye a los conocimientos de los analistas de seguridad ni a las actividades de refuerzo de redes y sistemas que se tratan en este curso, pero se utilizan en combinación con otros métodos de seguridad. Los analistas de seguridad suelen trabajar en un Centro de Operaciones de Seguridad (SOC) donde pueden supervisar la actividad en toda la red. A continuación, pueden utilizar sus conocimientos y experiencia para determinar cómo responder a la información del cuadro de mandos y decidir cuándo los eventos cumplen los criterios para ser escalados a supervisión.
Puntos clave

Dispositivos / Herramientas
	

Ventajas
	

Desventajas

Firewall
	

Un firewall permite o bloquea el tráfico basándose en un conjunto de reglas.
	

Un firewall sólo es capaz de filtrar paquetes basándose en la Información proporcionada en la cabecera de los paquetes.

Sistema de detección de intrusiones (IDS)
	

Un IDS detecta y alerta a los administradores sobre posibles intrusiones, ataques y otro tipo de tráfico malicioso.
	

Un IDS sólo puede escanear en busca de ataques conocidos o anomalías obvias; los ataques nuevos y sofisticados podrían no ser detectados. En realidad, no detiene el Tráfico entrante.

Sistema de prevención de intrusiones (IPS)
	

Un IPS monitorea la actividad del sistema en busca de intrusiones y anomalías y toma medidas para detenerlas.
	

Un IPS es un dispositivo en línea. Si falla, se interrumpe la conexión entre la red privada e Internet. Puede detectar falsos positivos y bloquear el tráfico legítimo.

Administración de información y eventos de seguridad (SIEM)
	

Una herramienta SIEM recopila y analiza los datos de registro de varios equipos de red. Agrega los eventos de Seguridad para su Monitoreo en un tablero central.
	

Una herramienta SIEM sólo informa sobre posibles Problemas de Seguridad. No lleva a cabo ninguna acción para detener o prevenir eventos sospechosos.

La compra, instalación y mantenimiento de cada uno de estos dispositivos o herramientas cuesta dinero. Es posible que una organización necesite contratar personal adicional para monitorizar las herramientas de Seguridad, como en el caso de un SIEM. Los responsables de la toma de decisiones tienen la tarea de seleccionar el nivel apropiado de Seguridad basándose en el coste y el Riesgo para la organización. Más adelante aprenderá más sobre la elección de los niveles de Seguridad. 


---

Resumen de la actividad

En esta actividad, se le presentará un escenario sobre una organización de medios sociales que recientemente experimentó una importante violación de datos causada por vulnerabilidades no detectadas. Para hacer frente a la violación, identificará algunas herramientas comunes de refuerzo de la red que se pueden implementar para proteger la seguridad general de la organización. A continuación, seleccionará una vulnerabilidad específica que tenga la empresa y propondrá diferentes métodos de endurecimiento de la red. Por último, explicará cómo los métodos y herramientas que haya elegido serán eficaces para gestionar la vulnerabilidad y cómo evitarán posibles brechas en el futuro.

En el curso, ha aprendido prácticas de endurecimiento de la red y prácticas de endurecimiento relacionadas con la seguridad de la red, como el filtrado de puertos, los privilegios de acceso a la red y el cifrado en las redes. Las prácticas de endurecimiento de la red ayudan a las organizaciones a controlar las posibles amenazas y ataques a su red y a evitar que se produzcan algunos ataques. Algunas prácticas de endurecimiento se aplican todos los días, mientras que otras se ejecutan de vez en cuando, como cada dos semanas o una vez al mes. Comprender cómo utilizar las herramientas y los métodos de endurecimiento de la red le ayudará a supervisar mejor la actividad de la red y a proteger la red de su organización contra diversos ataques.

Asegúrese de completar esta actividad antes de continuar. El siguiente punto del curso le proporcionará un ejemplo completado para que lo compare con su propio trabajo. 
Escenario

Revise el siguiente escenario. A continuación, complete las instrucciones paso a paso.

Usted es un analista de seguridad que trabaja para una organización de medios sociales. La organización ha sufrido recientemente una importante violación de datos, que ha puesto en peligro la seguridad de la información personal de sus clientes, como nombres y direcciones. Su organización quiere implantar prácticas sólidas de endurecimiento de la red que puedan llevarse a cabo de forma coherente para evitar ataques y violaciones en el futuro.

Tras inspeccionar la red de la organización, usted descubre cuatro vulnerabilidades importantes. Las cuatro vulnerabilidades son las siguientes

    Los empleados de la organización comparten contraseñas.

    La contraseña de administrador de la base de datos está configurada por defecto.

    Los cortafuegos no tienen reglas establecidas para filtrar el tráfico que entra y sale de la red.

    No se utiliza la autenticación multifactor (MFA).

Si no se toman medidas para solucionar estas vulnerabilidades, la organización corre el riesgo de sufrir otra violación de datos u otros ataques en el futuro.

En esta actividad, redactará una evaluación de riesgos de seguridad para analizar el incidente y explicar qué métodos se pueden utilizar para proteger aún más la red.
Instrucciones paso a paso

Siga las instrucciones y responda a la siguiente pregunta para completar la actividad. A continuación, vaya al siguiente punto del curso para comparar su trabajo con un ejemplar completado.

Paso 1: Acceder a la plantilla

Para utilizar la plantilla para este elemento del curso, haga clic en el siguiente enlace y seleccione Utilizar plantilla.

Enlace a la plantilla: Informe de evaluación de riesgos de seguridad

O

Si no dispone de una cuenta de Google, puede descargar la plantilla directamente desde el archivo adjunto a continuación.  

Paso 2: Acceso a los materiales de apoyo

Los siguientes materiales de apoyo le ayudarán a completar esta actividad. Manténgalos abiertos mientras avanza a los siguientes pasos.

Para utilizar los materiales de apoyo para este tema del curso, haga clic en el siguiente enlace y seleccione Utilizar plantilla.

Enlace a los materiales de apoyo: Herramientas de endurecimiento de la red

O

Si no dispone de una cuenta de Google, puede descargar los materiales de apoyo directamente desde el siguiente archivo adjunto.

Paso 3: Seleccionar hasta tres herramientas y métodos de endurecimiento para implementar

Piense en todas las herramientas y métodos de endurecimiento de la red que ha conocido en este curso y que pueden proteger la red de la organización de futuros ataques. ¿Qué tareas de endurecimiento serían la forma más eficaz de responder a esta situación? 
Escriba su respuesta en la primera parte de la hoja de trabajo.

Paso 4: Proporcionar y explicar 1-2 recomendaciones

Ha recomendado una o dos prácticas de Endurecimiento de seguridad para ayudar a evitar que esto vuelva a ocurrir en el futuro. Explique por qué la herramienta o método de endurecimiento de seguridad seleccionado es eficaz para abordar la vulnerabilidad. Aquí tiene un par de preguntas para empezar:

    ¿Por qué es eficaz la técnica de Endurecimiento de seguridad recomendada?

    ¿Con qué frecuencia debe implementarse la técnica de endurecimiento?

Escriba su respuesta en la segunda parte de la hoja de trabajo.
Consejo profesional: Guarde la plantilla

Por último, asegúrese de guardar una copia en blanco de la plantilla que ha utilizado para completar esta actividad. Puede utilizarla para seguir practicando o en sus proyectos profesionales. Estas plantillas le ayudarán a elaborar sus procesos de reflexión y a demostrar su experiencia a posibles empleadores.
Qué incluir en su respuesta

Asegúrese de abordar los siguientes criterios en su actividad completada:

    De una a tres herramientas y métodos de endurecimiento de la red.

    Las razones por las que las herramientas y métodos seleccionados son eficaces.

Evaluación del ejemplar

Compare el ejemplar con su actividad finalizada. Revise su trabajo utilizando cada uno de los criterios del ejemplar. ¿Qué ha hecho bien? ¿En qué puede mejorar? Utilice sus respuestas a estas preguntas como guía para seguir avanzando en el curso.

Nota: El ejemplar representa una posible explicación de los problemas a los que se enfrenta la organización de redes sociales. Existen múltiples herramientas y métodos correctos de Endurecimiento de seguridad que puede utilizar. Lo importante es que haya identificado las medidas de endurecimiento de la red más eficaces para gestionar las vulnerabilidades seleccionadas. En su Función de analista de seguridad, usted y su Equipo explicarían a continuación sus decisiones y argumentarían por qué esas medidas serán eficaces para proteger la red.

El ejemplo se centra en la vulnerabilidad de un software obsoleto para una base de datos local. Se identifica una posible solución a la vulnerabilidad y se incluye en el Informe para los supervisores directos. En el Informe se explica cómo la empresa podría verse comprometida en el futuro si la base de datos no se parchea y si los empleados siguen compartiendo contraseñas. 


En la sección sobre la política de seguridad de la información de la organización, el Informe incluye información sobre la adición de prácticas generales de refuerzo de la seguridad, una recomendación sobre la frecuencia con la que deben realizarse las prácticas de refuerzo y una explicación de cuáles son las posibles consecuencias si no se sigue la política. Este es un ejemplo de cómo puede analizarse un informe de evaluación de riesgos para la seguridad y cómo podría redactarse una política de seguridad de la información. 
Puntos clave


Como analista de seguridad, puede ser responsable de iniciar las prácticas de Seguridad de red. Tomar decisiones ejecutivas sobre qué herramientas utilizar basándose en lo que sabe sobre ciertas vulnerabilidades será un punto de partida para ayudar a la organización a mejorar la seguridad de su red. Explicar y documentar sus decisiones como analista de ciberseguridad le ayudará en el futuro si alguna vez hay que solucionar problemas en la red. También contribuirá a que los empleados sin conocimientos técnicos se impliquen y les ayudará a seguir las prácticas de Seguridad, como la autenticación multifactor. 