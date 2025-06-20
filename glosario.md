Vulnerabilidades con Kali Linux

Este documento recopila los conceptos y herramientas clave para la ciberseguridad ofensiva, centrada en el uso de Kali Linux para la evaluación de vulnerabilidades y pruebas de penetración.
1. Marco General y Ética en Ciberseguridad

Las fuentes enfatizan la importancia de la ciberseguridad en diversas industrias a nivel global. Un aspecto crucial es la ética en el uso de las herramientas y técnicas.

    Uso Ético: "La información contenida en este libro está destinada a ser utilizada únicamente de manera ética. No utilice ninguna información del libro si no tiene permiso por escrito del propietario del equipo." Se recalca que el uso ilegal de esta información puede llevar a arrestos y persecución judicial. Es imperativo contar con autorización por escrito de las personas responsables antes de realizar cualquier prueba.
    Amenazas y Ataques: Un "ataque es simplemente un método o técnica utilizada por un actor de amenaza para aprovechar (explotar) una vulnerabilidad de seguridad (debilidad) dentro de un sistema". Se mencionan varios tipos de ataques, como el ransomware LockBit 3.0, que explota vulnerabilidades en sistemas expuestos a internet.

2. Identificación de Actores de Amenaza y sus Motivaciones

Comprender a los actores de amenaza es fundamental para un aspirante a hacker ético y probador de penetración.

    Tipos de Actores de Amenaza:Black Hat Hackers: Utilizan sus habilidades de hacking con fines maliciosos, ya sea para destruir la reputación, robar datos o como un desafío personal.
    White Hat Hackers: Son los "buenos" de la industria, que usan sus habilidades para ayudar a organizaciones a proteger sus redes y activos de hackers maliciosos. Los hackers éticos y probadores de penetración son ejemplos de white hats.
    Gray Hat Hackers: Se sitúan entre los white y black hats. Pueden usar sus habilidades profesionalmente durante el día y para fines maliciosos por la noche. Aunque tienen habilidades de hacking, "los hackers de sombrero gris se salen de la buena zona moral y pueden usar sus habilidades con intenciones maliciosas".
    Grupos APT (Advanced Persistent Threat): Son grupos organizados con "esfuerzo y recursos" significativos, a menudo financiados, con la intención de robar datos y venderlos para obtener ganancias financieras.
    Implantes de Red: Pueden ser basados en software (código malicioso instalado en un sistema comprometido para acceso remoto) o hardware (dispositivos físicos conectados a la red interna del objetivo para monitoreo, control y exfiltración de datos).

3. Modelado de Amenazas

El modelado de amenazas es un proceso crucial para identificar, comprender y mitigar posibles amenazas a un sistema.

    Modelos Comunes: STRIDE (Spoofing identity, Tampering with data, Repudiation threats, Information disclosure, Denial of service, Elevation of privilege) y PASTA (Process for Attack Simulation and Threat Analysis).
    Ejemplo STRIDE (Sistema Bancario Online):Spoofing Identity: Actor malicioso intenta suplantar la identidad de un usuario legítimo. Mitigación: Implementar autenticación multifactor (MFA).
    Tampering with Data: Actor malicioso intenta interceptar y alterar datos financieros sensibles. Mitigación: Implementar tecnologías de cifrado de datos de extremo a extremo, como certificados digitales.
    Repudiation Threats: Actor de amenaza realiza un ataque DoS para denegar solicitudes legítimas. Mitigación: Implementar sistemas de registro transaccional para la no-repudiación.

4. Enfoques y Tipos de Pruebas de Penetración

Existen diferentes metodologías para las pruebas de penetración, cada una con sus particularidades.

    Enfoques de Pruebas de Seguridad:Black Box Testing: El probador tiene conocimiento nulo o muy limitado de la infraestructura interna del objetivo, simulando un ataque externo.
    Gray Box Testing: El probador tiene algún conocimiento limitado de la arquitectura interna o credenciales de bajo nivel.
    White Box Testing: El probador tiene conocimiento completo y acceso a la arquitectura interna, código fuente y configuraciones del sistema.
    Diferencia entre Evaluación de Vulnerabilidades y Pruebas de Penetración:Evaluación de Vulnerabilidades: Un profesional de cibersegseguridad utiliza un escáner de vulnerabilidades para identificar la postura de seguridad de los sistemas, utilizando "varias técnicas para automatizar el proceso de descubrimiento de una amplia gama de debilidades de seguridad en los sistemas".
    Pruebas de Penetración: Implican explotar activamente las vulnerabilidades para demostrar el impacto real de un ataque exitoso.

5. Reconocimiento y Recopilación de Información (OSINT)

El reconocimiento es la fase inicial donde se recopila información sobre el objetivo.

    Enumeración DNS: La técnica de "sondear registros DNS específicos para un dominio objetivo para recuperar información sobre los activos de una organización expuestos a Internet e identificar cualquier vulnerabilidad de seguridad que pueda ayudar a planificar un ciberataque". Herramientas como DNSRecon y host son útiles.
    Cosecha de Subdominios: Descubrir todos los subdominios posibles de una organización objetivo puede revelar "ubicaciones y recursos sensibles, como portales de inicio de sesión y directorios corporativos expuestos involuntariamente". Herramientas: DNSMap y Sublist3r, theHarvester.
    Identificación de Presencia en Redes Sociales: Herramienta Sherlock (python3 sherlock <username>) para buscar la presencia de una organización en redes sociales.
    Shodan: Se destaca como una herramienta para identificar puertos abiertos y servicios, incluso versiones vulnerables como "Server Message Block (SMB) versión 1, que se sabe que contiene fallas de seguridad que permiten a un atacante realizar ejecución remota de código (RCE) en el sistema objetivo".

6. Escaneo y Enumeración de Redes

El escaneo es una técnica activa para descubrir sistemas en una red, identificar puertos abiertos, servicios y sistemas operativos.

    Advertencia Legal: "No realice ningún tipo de escaneo en sistemas y redes que no posea o para los que no tenga permiso legal para hacerlo. El escaneo se considera ilegal en muchos países."
    Cambio de Dirección MAC: La dirección MAC es teóricamente inalterable, pero puede ser spoofeadas para evadir detección o simular un dispositivo diferente (ej., sudo nmap -sT -Pn --spoof-mac hp 172.30.1.49).
    Descubrimiento de Hosts Vivos: Herramientas como ifconfig o ip address para verificar la conectividad y sipcalc para calcular rangos de red. Netdiscover -p -i eth1 para escanear pasivamente sistemas en vivo.
    Identificación de Puertos Abiertos, Servicios y SO:Nmap: Herramienta fundamental para "fingerprinting". Permite identificar el sistema operativo, versiones de servicios y realizar un traceroute (nmap -A -T4 -p- <IP_Objetivo>).
    Sintaxis Importantes de Nmap:-Pn: Considera al objetivo en línea sin descubrimiento de hosts.
    -sU: Escaneo de puertos UDP.
    -p: Especifica puertos (rangos, grupos o todos con -p-).
    -sV: Identificación de la versión del servicio.
    -6: Escaneo de redes o hosts IPv6.
    Nmap Scripting Engine (NSE): Característica poderosa con "600+ scripts pre-construidos" para realizar escaneos personalizados y detectar vulnerabilidades. Categorías incluyen Auth, Broadcast, Brute, Discovery, DoS, Exploit, Vuln, etc.
    ping Utility: Analizar el valor TTL (Time-To-Live) en los mensajes de respuesta ICMP para perfilar el sistema operativo (Windows: TTL 128, Linux: TTL 64).
    Enumeración de Servicios de Red:SMB (Server Message Block): Servicio común para compartir recursos. Herramientas como Metasploit (search smb_version) y SMBMap (smbmap -H <IP> --download .\tmp) son usadas para enumerar archivos y unidades compartidas. enum4linux para enumerar usuarios, políticas de contraseñas y shares SMB.
    SMTP (Simple Mail Transfer Protocol): Usar netcat (nc -nv <IP> 25) para verificar puertos y el comando VRFY para determinar usuarios válidos. Scripts personalizados (smtp_user_enum.sh) para enumeración automática de usuarios.
    SNMP (Simple Network Management Protocol): Protocolo para monitorear y gestionar dispositivos de red. Se puede usar Nmap (sudo nmap -sU -p 161 <IP>) para verificar si SNMP está corriendo, y snmp-check (snmp-check -p 161 -c public -v 1 <IP>) para enumerar información sensible como tiempo de actividad del sistema, nombre de host, utilización de CPU/memoria, etc.

7. Post-Explotación y Movimiento Lateral

Una vez que se obtiene acceso a un sistema, el siguiente paso es mantener la persistencia y expandir el control dentro de la red.

    Shells Remotas (Bind y Reverse Shells):Bind Shells: El sistema objetivo escucha en un puerto específico (nc -nlvp 1234 -e /bin/bash), y el atacante se conecta a él. Útiles cuando se conoce la IP del objetivo y se puede configurar un listener.
    Reverse Shells: El sistema objetivo inicia una conexión hacia el atacante (que está escuchando), útil cuando el objetivo está detrás de un firewall o NAT.
    Netcat: Herramienta fundamental para configurar listeners y shells remotas.
    Técnicas de Evasión de Antimalware: Implican desarrollar payloads personalizados para sistemas Windows, Linux, Android, iOS, que evadan la detección. Shellter es una herramienta para generar payloads.
    Persistencia en Windows: Módulos de Metasploit como exploit/windows/local/persistence y exploit/windows/local/registry_persistence pueden crear payloads que modifican el registro del sistema (HKLM\Software\Microsoft\Windows\CurrentVersion\Run\) y almacenan scripts VBS en C:\WINDOWS\TEMP\, ejecutándose en cada inicio de sistema o inicio de sesión de usuario. Es fundamental remover estos payloads al finalizar la prueba.
    Sugerencia de Explotación Local (Metasploit): El módulo post/multi/recon/local_exploit_suggester permite a Metasploit verificar si un sistema comprometido es vulnerable a otros módulos de explotación, identificando "vulnerabilidades adicionales en un sistema objetivo".
    CrackMapExec: Herramienta para realizar movimiento lateral y enumeración en dominios Windows.
    Enumeración SMB: Permite "determinar rápidamente si una cuenta de usuario de dominio puede acceder a otros sistemas en la red".
    Extracción de Bases de Datos SAM: Permite recuperar el contenido de la base de datos SAM (que contiene hashes NTLMv1) de dispositivos Windows en el dominio, si la cuenta de usuario tiene privilegios administrativos.
    Pass-The-Hash (PTH): Utilizar hashes NTLMv1 obtenidos para el movimiento lateral en el dominio (crackmapexec smb <rango_IP> -u bob -H <hash>).
    Mimikatz: Herramienta poderosa para la extracción de credenciales y la creación de "skeleton keys" en controladores de dominio, lo que permite acceso persistente y sin autenticación.
    Skeleton Key: Permite el acceso a cualquier cuenta en el dominio sin autenticación, una técnica extremadamente peligrosa.

8. Hacking de Redes Inalámbricas

Se cubren los fundamentos del hacking de redes inalámbricas, incluyendo adaptadores y modos de operación.

    Adaptadores Inalámbricos: No todos los adaptadores soportan "Monitor mode" y "packet injection". Se recomiendan adaptadores específicos como Alfa AWUS036NHA y Alfa AWUS036ACH.
    Modos de Operación Inalámbrica:Managed (Administrado): Modo predeterminado, permite conectar a un punto de acceso. No apto para pruebas de penetración inalámbricas.
    Monitor (Monitorización): Permite escanear redes 802.11, capturar tramas inalámbricas (beacons, probes) e inyectar paquetes sin establecer una conexión.
    Master (Maestro): Convierte el sistema Linux en un punto de acceso o router inalámbrico.
    Ad hoc: Conexión directa entre hosts sin un dispositivo intermediario.
    Repeater (Repetidor): Captura y reproduce una señal inalámbrica para extender el rango.
    Airodump-ng: Herramienta para monitorear redes inalámbricas cercanas, capturar "handshakes" WPA/WPA2.
    Campos Relevantes: BSSID (MAC del AP), PWR (señal), Beacons (tramas de AP), #Data (paquetes de datos), #/s (paquetes por segundo), CH (canal), MB (velocidad), ENC (cifrado), CIPHER (cifrado), AUTH (autenticación), ESSID (nombre de red), STATION (MAC de clientes), Probes (PNL de clientes).
    Aircrack-ng: Utilizado para descifrar contraseñas offline de handshakes WPA/WPA2 capturados, utilizando listas de palabras.
    Airmon-ng: Herramienta para cambiar el modo de operación de un adaptador inalámbrico a "Monitor mode".

9. Herramientas y Utilidades de Kali Linux

Kali Linux es un sistema operativo diseñado para pruebas de penetración y auditoría de seguridad.

    PimpMyKali: Script de Dewalt para "arreglar e instalar utilidades y herramientas muy útiles que son comúnmente usadas por los probadores de penetración y actualizar los paquetes de software existentes en nuestra máquina virtual Kali Linux". Se advierte que se usa bajo propio riesgo.
    Metasploitable 3: Máquina virtual vulnerable (Linux y Windows) para practicar pruebas de penetración.
    FreeRadius: Servidor RADIUS para autenticación de red.
    DNSRecon: Herramienta para enumeración DNS.
    DNSMap y Sublist3r: Herramientas para la cosecha de subdominios.
    theHarvester: Recopilación de información de subdominios a través de motores de búsqueda y otras fuentes.
    Sherlock: Búsqueda de presencia en redes sociales.
    Nmap: Escáner de puertos y herramienta de fingerprinting robusta, con el Nmap Scripting Engine (NSE) para detección de vulnerabilidades.
    Netdiscover: Herramienta para el descubrimiento pasivo de hosts en una red.
    SMBMap y enum4linux: Herramientas para enumeración de servicios SMB.
    Netcat: Utilidad multipropósito para crear conexiones de red y shells remotas.
    SNMP-Check: Herramienta para enumeración SNMP.
    Nessus y Greenbone Vulnerability Manager (GVM): Herramientas para realizar evaluaciones de vulnerabilidades.
    WhatWeb, Nikto, Metasploit, WPScan: Escáneres de aplicaciones web.
    Shellter: Generación de payloads personalizados para evasión de antimalware.
    SecLists: Colección de listas de palabras (contraseñas, nombres de usuario, URLs, patrones de datos sensibles) para ataques de diccionario y fuzzing.
    Crunch: Generador de listas de palabras personalizadas.
    Hydra y Ncrack: Herramientas multi-hilo de fuerza bruta para cracking de contraseñas online.
    nbtscan: Herramienta para escanear nombres NetBIOS en una red.
    Mimikatz: Herramienta para extraer credenciales en sistemas Windows, incluyendo hashes NTLM y creación de "skeleton keys".
    Responder: Herramienta para ataques MiTM, a menudo utilizada para capturar hashes NTLM.
    Impacket (ntlmrelayx.py, GetUserSPNs.py): Colección de scripts Python para interactuar con protocolos de red, incluyendo ataques de retransmisión NTLM y enumeración de SPN.
    CrackMapExec: Herramienta de post-explotación para movimiento lateral y enumeración en entornos de dominio.
    Metasploit Framework: Plataforma modular para desarrollo y ejecución de exploits, con amplias capacidades de post-explotación.
    Python: Mencionado para shells pseudo-Terminal en Linux y para servidores web simples.

10. Conceptos Clave Adicionales

    OSINT (Open Source Intelligence): Recopilación de información de fuentes públicamente disponibles.
    Vulnerabilidad: Una "debilidad" en un sistema que puede ser explotada.
    Exploit: Código o técnica que aprovecha una vulnerabilidad. Los exploits deben ser probados rigurosamente ya que "a veces, un exploit puede funcionar en un sistema y no en otro".
    Payload: El componente de un exploit que realiza la acción deseada en el sistema comprometido.
    RCE (Remote Code Execution): Capacidad de ejecutar código arbitrario en un sistema remoto.
    DoS (Denial of Service): Ataque que busca hacer un servicio inaccesible para sus usuarios legítimos.
    SQL Injection: Vulnerabilidad de aplicación web que permite la ejecución de comandos SQL maliciosos.
    NAT (Network Address Translation): Servicio que permite que múltiples dispositivos en una red privada compartan una única dirección IP pública.
    Autenticación y Autorización: Proceso de verificar la identidad del usuario y sus permisos.
    Cifrado (Encryption): Proceso de transformar información para proteger su confidencialidad.
    Hashing (Hashed): Proceso de convertir datos en una cadena de caracteres de longitud fija, a menudo para almacenar contraseñas de forma segura.
    NTLMv1/NTLMv2: Protocolos de autenticación de Windows. Se advierte que NTLMv1 es obsoleto e inseguro.
    SID (Security Identifier): Identificador único para usuarios, grupos y otros objetos de seguridad en Windows.
    Kerberos: Protocolo de autenticación de red para entornos de dominio.
    Silver Ticket: Tipo de ataque de Kerberos que permite a un atacante crear tickets de servicio falsos para acceder a servicios específicos sin pasar por el controlador de dominio.
    IEEE 802.11: Estándares para redes de área local inalámbricas (Wi-Fi).
    WPA-PSK/WPA2-PSK: Estándares de seguridad para redes inalámbricas.