
---

# Framework

## SGSI: Sistema de Gestión de Seguridad de la Información

**SGSI** (en inglés, Information Security Management System o ISMS) es un conjunto de políticas y procedimientos que ayudan a las organizaciones a gestionar la seguridad de la información de forma sistemática y a proteger los activos de información de amenazas. El propósito de un SGSI es tener los riesgos gestionados.

---

# Gestión

## Riesgos

Al hablar de **riesgos**, nos referimos de manera proactiva a los elementos que pueden afectar a la organización, buscando medidas de mitigación para ellos.

## Evento de Seguridad de la Información

Según la norma ISO 27035, un **Evento de Seguridad de la Información** es una "Ocurrencia que indica una posible violación de la seguridad de la información o falla de los controles".

## Incidente de Seguridad de la Información

De acuerdo con la norma ISO 27035, un **Incidente de Seguridad de la Información** es "Uno o varios eventos de seguridad de la información relacionados e identificados que pueden dañar los activos de la organización y/o comprometer sus operaciones."

## Gestión de Incidentes de Seguridad de la Información

La **Gestión de Incidentes de Seguridad de la Información** es el "Ejercicio de un enfoque consistente y efectivo para el manejo de incidentes de seguridad de la información".

### Hardware y Software

Para una correcta y eficiente gestión de incidentes, la entidad debería tener en cuenta los siguientes elementos:

* Portátiles Forenses
* Analizadores de protocolos
* Software de adquisición
* Software para recolección de evidencia
* Kit de respuesta a incidentes
* Software de análisis forense
* Medios de almacenamiento

### Recursos para el Análisis de Incidentes

Es fundamental disponer de los siguientes recursos para el análisis de incidentes:

* Tener un **listado de los puertos conocidos y de los puertos utilizados para realizar un ataque**.
* Tener un **diagrama de red** para la ubicación rápida de los recursos existentes.
* Una **Línea Base de Información** de Servidores (Nombre, IP, Aplicaciones, Parches, Usuarios Configurados, responsable de cambios). Esta información siempre debe estar actualizada para conocer el funcionamiento normal del mismo y realizar una identificación más acertada de un incidente.
* Se debe tener un **análisis del comportamiento de red estándar**, incluyendo: puertos utilizados por los protocolos de red, horarios de utilización, direcciones IP con mayor tráfico, y direcciones IP que reciben el mayor número de peticiones.

### Recursos para la Mitigación y Remediación

En este punto se consideran los elementos básicos para la contención de un posible incidente: **Backup de Información**, **imágenes de servidores**, y cualquier información base que pueda recuperar el funcionamiento normal del sistema.

### Detección, Evaluación y Análisis

#### Detección, Identificación y Gestión de Elementos Indicadores de un Incidente

Los **indicadores** son los eventos que nos señalan que posiblemente ha ocurrido un incidente. Generalmente, algunos de estos elementos son:

* Alertas en sistemas de seguridad
* Caídas de servidores
* Reportes de usuarios
* Software antivirus dando informes
* Otros funcionamientos fuera de lo normal del sistema

La identificación y gestión de elementos que alertan sobre un incidente nos proveen información que puede alertarnos sobre su futura ocurrencia y preparar procedimientos para minimizar su impacto. Algunos de estos elementos pueden ser:

* Logs de servidores
* Logs de aplicaciones
* Logs de herramientas de seguridad
* Cualquier otra herramienta que permita la identificación de un incidente de seguridad

En la entidad debe existir un **listado de fuentes generadoras de eventos** que permitan la identificación de un incidente de seguridad de la información.

#### Análisis

Las actividades de análisis del incidente involucran otra serie de componentes. Es recomendable tener en cuenta los siguientes:

* Tener conocimientos de las **características normales a nivel de red y de los sistemas**.
* Los administradores de TI deben tener **conocimiento total sobre los comportamientos de la Infraestructura** que están administrando.
* Toda información que permita realizar análisis al incidente debe estar **centralizada** (Logs de servidores, redes, aplicaciones).
* Es importante efectuar **correlación de eventos**, ya que por medio de este proceso se pueden descubrir patrones de comportamiento anormal y poder identificar de manera más fácil la causa del incidente.
* Para un correcto análisis de un incidente, debe existir una **única fuente de tiempo** (Sincronización de Relojes), ya que esto facilita la correlación de eventos y el análisis de información.
* Se debe mantener y usar una **base de conocimiento** con información relacionada sobre nuevas vulnerabilidades, información de los servicios habilitados, y experiencias con incidentes anteriores.
* Crear **matrices de diagnóstico e información** para los administradores menos experimentados.

#### Evaluación

Para realizar la **evaluación de un incidente de seguridad**, se deben tener en cuenta los **niveles de impacto** con base en los insumos entregados por el análisis de riesgos y la clasificación de activos de información de la entidad.

La severidad del incidente puede ser:

* **Alto Impacto**: El incidente de seguridad afecta a activos de información considerados de impacto catastrófico y mayor que influyen directamente en los objetivos misionales del Instituto. Se incluyen en esta categoría aquellos incidentes que afecten la reputación y el buen nombre o involucren aspectos legales. Estos incidentes deben tener respuesta inmediata.
* **Medio Impacto**: El incidente de seguridad afecta a activos de información considerados de impacto moderado que influyen directamente en los objetivos de un proceso determinado.
* **Bajo Impacto**: El incidente de seguridad afecta a activos de información considerados de impacto menor e insignificante, que no influyen en ningún objetivo. Estos incidentes deben ser monitoreados con el fin de evitar un cambio en el impacto.

#### Clasificación de Incidentes de Seguridad de la Información

Algunos ejemplos de clasificación de incidentes podrían ser (esta clasificación está sujeta a cada entidad dependiendo de su infraestructura, de sus riesgos y criticidad de los activos. La clasificación dada es solo un ejemplo):

* **Acceso no autorizado**: Es un incidente que involucra a una persona, sistema o código malicioso que obtiene acceso lógico o físico sin autorización adecuada del dueño a un sistema, aplicación, información o un activo de información.
* **Modificación de recursos no autorizado**: Un incidente que involucra a una persona, sistema o código malicioso que afecta la integridad de la información o de un sistema de procesamiento.
* **Uso inapropiado de recursos**: Un incidente que involucra a una persona que viola alguna política de uso de recursos.
* **No disponibilidad de los recursos**: Un incidente que involucra a una persona, sistema o código malicioso que impide el uso autorizado de un activo de información.
* **Multicomponente**: Un incidente que involucra más de una categoría anteriormente mencionada.
* **Otros**: Un incidente que no puede clasificarse en alguna de las categorías anteriores. Este tipo de incidentes debe monitorearse con el fin de identificar la necesidad de crear nuevas categorías.

#### Priorización de los Incidentes y Tiempos de Respuesta

Con el fin de permitir una atención adecuada a los incidentes (análisis, contención y erradicación), se debe determinar el **nivel de prioridad** del mismo, y de esta manera atenderlos adecuadamente según la necesidad.

A modo de ejemplo, se definen una serie de variables que podrán ser utilizadas para realzar la evaluación de los incidentes:

* Prioridad
* Criticidad de impacto
* Impacto Actual
* Impacto Futuro

**Nivel de Prioridad**: Depende del valor o importancia dentro de la entidad y del proceso que soporta el o los sistemas afectados.

**Tabla 1: Niveles de Criticidad de Impacto**

| Nivel      | Criticidad | Valor | Definición                                                                  |
| :--------- | :--------- | :---- | :-------------------------------------------------------------------------- |
| Inferior   | 0,10       | Sistemas no críticos, como estaciones de trabajo de usuarios con funciones no críticas. |
| Bajo       | 0,25       | Sistemas que apoyan a una sola dependencia o proceso de una entidad.      |
| Medio      | 0,50       | Sistemas que apoyan más de una dependencia o proceso de la entidad.       |
| Alto       | 0,75       | Sistemas pertenecientes al área de Tecnología y estaciones de trabajo de usuarios con funciones críticas. |
| Superior   | 1,00       | Sistemas Críticos.                                                          |

**Impacto Actual**: Depende de la cantidad de daño que ha provocado el incidente en el momento de ser detectado.

**Impacto Futuro**: Depende de la cantidad de daño que pueda causar el incidente si no es contenido, ni erradicado.

**Tabla 2: Niveles de Impacto Actual y Futuro**

| Nivel      | Impacto | Valor | Definición                                                                                             |
| :--------- | :------ | :---- | :----------------------------------------------------------------------------------------------------- |
| Inferior   | 0,10    | Impacto leve en uno de los componentes de cualquier sistema de información o estación de trabajo.          |
| Bajo       | 0,25    | Impacto moderado en uno de los componentes de cualquier sistema de información o estación de trabajo.      |
| Medio      | 0,50    | Impacto alto en uno de los componentes de cualquier sistema de información o estación de trabajo.          |
| Alto       | 0,75    | Impacto moderado en uno o más componentes de más de un sistema de información.                             |
| Superior   | 1,00    | Impacto alto en uno o más componentes de más de un sistema de información.                                 |

Luego de tener definidas las variables, se obtiene la prioridad mediante la siguiente fórmula:

**Nivel Prioridad = (Impacto actual \* 2,5) + (Impacto futuro \* 2,5) + (Criticidad del Sistema \* 5)**

Y los resultados obtenidos se deben comparar con la siguiente tabla para determinar la prioridad de atención:

**Tabla 3: Niveles de Prioridad del Incidente**

| Nivel      | Prioridad | Valor           |
| :--------- | :-------- | :-------------- |
| Inferior   | 00,00     | 02,49           |
| Bajo       | 02,50     | 03,74           |
| Medio      | 03,75     | 04,99           |
| Alto       | 05,00     | 07,49           |
| Superior   | 07,50     | 10,00           |

## Evaluación y Decisión sobre los Eventos de Seguridad de Información

* Se debe establecer un **esquema de categorización y priorización de incidentes de seguridad de la información** para la identificación de las consecuencias y prioridad de un incidente.
* El esquema debe incluir los **criterios para clasificar los eventos como incidentes de seguridad de la información**.
* El punto de contacto debe **evaluar cada evento de seguridad de la información** utilizando el esquema acordado.
* El personal responsable de coordinar y responder a los incidentes de seguridad de la información debe **realizar la evaluación y tomar una decisión** sobre los eventos de seguridad de la información.
* Los resultados de la evaluación y la decisión deben **registrarse en detalle** para fines de referencia futura y verificación.

[ISO](https://www.iso.org/standard/27001) Norma Europea
[NICE](https://niccs.cisa.gov/tools/nice-framework) Norma Americana

[OWASP](https://owasp.org/projects/) 
Foco en riesgos de seguridad en software, ofrece un nivel técnico muy atractivo. Debe haber una gestion de riesgos previa.
[CIS Controls](https://www.cisecurity.org/controls)
Más basico y de facil implementacion ideales para concienciación y poder partir con medidas de control inmediatas.
[NIST](https://www.nist.gov/cyberframework)
Muy recomendable en contextos de implementación más maduros y de alto conocimiento en materias de ciberseguridad. Complejo en la evaluacion.

# Estructuras de equipos

## Red team
Seguridad Ofensiva
▪ Hacking Ético
▪ Explotar Vulnerabilidades
▪ Emulación Amenazas
▪ Ingeniería Social


## Blue team
Seguridad Defensivas
▪ Gestión de incidencias
▪ Infraestructura de protección
▪ Monitoreo proactivo
▪ Respuesta a incidentes
▪ Threat Hunter basado en TTP


# Estructuras Funcionales
## CERT: Recopila información de vulnerabilidades e IOC
[CISA](https://www.cisa.gov/)
[CSIRT](https://csirt.gob.cl/)

## SOC: Monitorear y defiende infraestructura
SIEM
SOAR
IDS/IPS- Snort / Suricata
End Point
EDr/XDR
Red(Firewall, Router)

SIEM: Plataformas de  monitoreo y análisis en tiempo real de eventos relacionados con la seguridad.
[SIEM](https://www.ibm.com/mx-es/topics/siem)

## CSIRT: Equipo que responde a los incidentes
