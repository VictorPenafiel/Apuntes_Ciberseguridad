DAST, API security
La prueba dinámica de seguridad de aplicaciones (DAST) es un método de prueba de ciberseguridad que se utiliza para identificar vulnerabilidades y configuraciones incorrectas en aplicaciones web, API y, más recientemente, aplicaciones móviles.

Importante: Todo debe ser de manera automatizada implementada en el proceso de desarrollo, muy mala practica validaciones de codigo de manera no automatizada

Seguridad integrada desde el inicio, no al final
Priorizar la seguridad en la etapa de diseño y planificacion del software
Incorporar la seguridad en el pipeline de desarrollo
Implementar pruebas a lo largo del proceso de desarrollo
automatizar los procesos de seguridad tanto como sea posible

planificacion
    Requisitos de seguridad

desarrollo de software o codificacion
    SAST ( Pruebas de Seguridad de Aplicaciones Estáticas ) : Las herramientas SAST analizan el código fuente de la aplicación y determinan vulnerabilidades o secretos (basándose en un conjunto de reglas que definen los errores en el código fuente que deben abordarse y evaluarse). Se suelen utilizar para analizar software personalizado escrito en lenguajes como Java, Python, Node.js, C/C++, etc.

construccion de nuestro software
    AutoFix AI

etapa de prueba
    SCA analiza el código fuente de la aplicación y/o los paquetes de distribución, identificando las dependencias de código abierto y comparando sus versiones con bases de datos de vulnerabilidades conocidas (CVEs

despliegue
    Pentesting, OPA

Operacion
    Patch, RASP

Mantenimiento y monitoreo
    Monitoreo de vulnerabilidades

---

Shift Left
Seguridad desde el incio
Pruebas de seguridad automatizadas
Se previenen errores antes de llegar a produccion
Reduce costos al encontrar problemas antes de que sucedan

Shift Right
Seguridad continua despues de despliegue
Se detectan y responden incidentes en produccion
Monitoreo de vulnerabilidades
Deteccion de anomalias

