En esta actividad, crearás un reporte de incidente utilizando el conocimiento que has adquirido sobre redes a lo largo de este curso para analizar un incidente de red. Analizarás la situación utilizando el Marco de Ciberseguridad del Instituto Nacional de Estándares y Tecnología (NIST CSF). El CSF es un marco voluntario que consta de normas, directrices y mejores prácticas para gestionar los riesgos de ciberseguridad. Crear un informe de incidentes de ciberseguridad de calidad y aplicar el CSF puede demostrar un enfoque proactivo de la seguridad, mejorar la comunicación y la transparencia con las partes interesadas y mejorar las prácticas de seguridad dentro de su organización. También puede añadir el informe de incidentes que cree a su cartera de ciberseguridad cuando lo complete.

El CSF es escalable y puede aplicarse en una amplia variedad de contextos. A medida que continúe aprendiendo más y perfeccionando su comprensión de las habilidades clave de ciberseguridad, puede utilizar las plantillas proporcionadas en esta actividad en otras situaciones. Saber identificar qué medidas de seguridad aplicar en respuesta a las necesidades de la empresa le ayudará a determinar cuáles son las mejores opciones disponibles cuando se trata de la seguridad de la red.

Asegúrese de completar esta actividad antes de continuar. En el siguiente punto del curso, podrá autoevaluar su respuesta. Después de eso, habrá un ejemplar completado para comparar con su propio trabajo. También tendrá la oportunidad de responder a las preguntas de la rúbrica que le permitirán reflexionar sobre los elementos clave de su declaración profesional.
Escenario

Revise el siguiente escenario. A continuación, complete las instrucciones paso a paso.

Usted es un analista de ciberseguridad que trabaja para una empresa multimedia que ofrece servicios de diseño web, diseño gráfico y soluciones de Marketing en redes sociales a pequeñas empresas. Su organización ha sufrido recientemente un ataque DDoS, que ha puesto en peligro la red interna durante dos horas hasta que se ha resuelto.

Durante el ataque, los servicios de red de su organización dejaron de responder repentinamente debido a una avalancha de paquetes ICMP entrantes. El tráfico normal de la red interna no podía acceder a ningún recurso de la red. El equipo de gestión de incidentes respondió bloqueando los paquetes ICMP entrantes, deteniendo todos los servicios de red no críticos fuera de línea y restableciendo los servicios de red críticos.

A continuación, el equipo de ciberseguridad de la empresa investigó el incidente de seguridad. Descubrieron que un actor malicioso había enviado una avalancha de pings ICMP a la red de la empresa a través de un cortafuegos no configurado. Esta vulnerabilidad permitió al agresor abrumar la red de la empresa mediante un ataque de denegación de servicio distribuido (DDoS).

Para hacer frente a este problema de seguridad, el equipo de Seguridad de red implementó:

    Una nueva regla de cortafuegos para limitar la tasa de paquetes ICMP entrantes

    Verificación de la dirección IP de origen en el cortafuegos para comprobar si hay direcciones IP falsificadas en los paquetes ICMP entrantes

    Software de Monitoreo de red para detectar patrones de tráfico anormales

    Un sistema IDS/IPS para filtrar parte del tráfico ICMP basado en características sospechosas

Como analista de ciberseguridad, se le ha encomendado la tarea de utilizar este evento de seguridad para crear un plan que mejore la seguridad de la red de su empresa, siguiendo el Marco de Ciberseguridad (CSF) del Instituto Nacional de Estándares y Tecnología (NIST). Utilizarás el CSF para ayudarte a navegar a través de los diferentes pasos del análisis de este evento de ciberseguridad e integrar tu análisis en una estrategia de seguridad general. Hemos dividido el análisis en diferentes partes en la plantilla que figura a continuación. Puede explorarlas aquí:

    Identificar los riesgos de seguridad mediante auditorías periódicas de las redes internas, los sistemas, los dispositivos y los privilegios de acceso para identificar posibles brechas en la seguridad.

    Proteger los activos internos mediante la aplicación de políticas, procedimientos, formación y herramientas que ayuden a mitigar las amenazas a la ciberseguridad.

    Detectar posibles incidentes de seguridad y mejorar las capacidades de supervisión para aumentar la rapidez y eficacia de las detecciones.

    Responder para contener, neutralizar y analizar incidentes de seguridad; implantar mejoras en el proceso de seguridad.

Recuperar el funcionamiento normal de los sistemas afectados y restaurar los datos y/o activos de los sistemas que se hayan visto afectados por un incidente. 
Instrucciones paso a paso

Siga las instrucciones y rellene las secciones para completar la actividad. A continuación, vaya al siguiente elemento del curso para comparar su trabajo con un ejemplo completado.


Paso 2: Resumir el incidente de seguridad

Utilizando la plantilla proporcionada, proporcione un resumen del suceso de seguridad ocurrido. Incluye información sobre el suceso de seguridad, su causa, el impacto y la respuesta. También puedes incluir información sobre los sistemas atacados, el origen del ataque y el impacto estimado. 

Paso 3: Identificar el tipo de ataque y los sistemas afectados

Piensa en todos los conceptos tratados en el curso hasta ahora y reflexiona sobre el escenario y define qué tipo de ataque se produjo y qué sistemas se vieron afectados. Enumera esta información en la hoja de trabajo de análisis de informes de incidentes en la sección titulada "Identificar"."

Paso 4: Proteja los activos de su organización para que no corran peligro

A continuación, evaluará dónde puede mejorar la organización para proteger aún más sus activos. En este paso, se centrará en crear un plan de acción inmediato para responder al incidente de ciberseguridad. Al crear este plan, reflexione sobre la siguiente pregunta:

    ¿Qué sistemas o procedimientos deben actualizarse o modificarse para proteger mejor los activos de la organización?

Escriba su respuesta en la plantilla de análisis de informes de incidentes en la sección "Proteger".

Paso 5: Detectar incidentes similares en el futuro

Es importante supervisar continuamente el tráfico de red en los dispositivos de red para comprobar si hay actividad sospechosa, como paquetes ICMP externos entrantes procedentes de direcciones IP no fiables que intentan atravesar el cortafuegos de red de la organización.

Para este paso, considere las formas en que usted y su equipo pueden supervisar y analizar el tráfico de red, las aplicaciones de software, realizar un seguimiento de los usuarios autorizados frente a los no autorizados y detectar cualquier actividad inusual en las cuentas de usuario. Escriba su respuesta en la hoja de trabajo de análisis de respuesta ante incidentes, en la sección "Detectar".

Paso 6: Responder a futuros incidentes de ciberseguridad

Después de identificar las herramientas y métodos que usted y su organización tienen en marcha para detectar posibles vulnerabilidades y amenazas, cree un plan de respuesta en caso de que se produzca un incidente en el futuro. Esto suele ocurrir después de que se haya producido el incidente y haya sido resuelto por usted y su equipo. En este caso, creará un plan de respuesta para futuros incidentes de ciberseguridad. Algunos puntos a tener en cuenta a la hora de crear un plan de respuesta ante cualquier incidente de ciberseguridad:

    ¿Cómo pueden usted y su equipo contener los incidentes de ciberseguridad y los dispositivos afectados?

    ¿Qué procedimientos existen para ayudarle a usted y a su equipo a neutralizar los incidentes de ciberseguridad?

    ¿Qué datos o información pueden utilizarse para analizar este incidente?

    ¿Cómo puede mejorarse el proceso de recuperación de su organización para gestionar mejor futuros incidentes de ciberseguridad?

Escriba su respuesta en la plantilla de análisis de informes de incidentes, en la sección "responder". 

Paso 7: Recuperarse del incidente

Considere qué medidas deben tomarse para ayudar a la organización a recuperarse del incidente de ciberseguridad. Reflexione sobre toda la información que ha recopilado sobre el incidente en los pasos anteriores para considerar qué dispositivos, sistemas y procesos deben restaurarse y recuperarse.

Considere las siguientes preguntas:

    ¿Qué información necesita poder recuperar inmediatamente?

    ¿Qué procesos existen para ayudar a la organización a recuperarse del incidente?

Escribe tu respuesta en la parte de "recuperación" de la hoja de trabajo.

Consejo profesional: Guarde la plantilla de análisis de informes de incidentes

Por último, asegúrese de guardar una copia de su plantilla de análisis de informes de incidentes en algún lugar accesible para que pueda acceder a ella a medida que avance en el curso y en el campo de la seguridad.
Qué incluir en su respuesta

Más adelante, tendrá la oportunidad de evaluar su actuación utilizando los criterios enumerados. Asegúrese de incluir lo siguiente en su actividad completa.

Curso 3 análisis de informes de incidentes

    Resume el evento de seguridad

    Identifica el tipo de ataque y los sistemas afectados por el incidente

    Ofrece un plan de protección contra futuros incidentes de ciberseguridad

    Describe los métodos de detección que pueden utilizarse para identificar posibles incidentes de ciberseguridad

    Incluye un plan de respuesta para el incidente de ciberseguridad y un esquema para futuros incidentes de ciberseguridad

    Esboza planes de recuperación que usted y la organización pueden aplicar en futuros incidentes de ciberseguridad.