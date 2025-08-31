`tcpdump`, una herramienta fundamental para el análisis de tráfico.

`tcpdump` es un analizador de paquetes de red de línea de comandos. Permite capturar y analizar el tráfico que pasa a través de una interfaz de red, mostrando los encabezados de los paquetes. Es invaluable para la depuración de redes, seguridad y diagnóstico.

### Sintaxis Básica

La sintaxis general es `tcpdump [opciones] [expresiones]`. Las **opciones** modifican el comportamiento de la herramienta (cómo se muestra la salida), mientras que las **expresiones** se usan para filtrar el tráfico capturado.

### Opciones y Banderas Clave

  * `-i <interfaz>`: **Obligatorio en muchos casos.** Especifica la interfaz de red a monitorear (ej. `eth0`, `wlan0`).
  * `-n`: No resuelve nombres de host a partir de direcciones IP. Esto acelera la captura.
  * `-nn`: No resuelve nombres de host ni puertos. Aún más rápido.
  * `-v`, `-vv`, `-vvv`: Aumenta el nivel de verbosidad para ver más detalles del paquete.
  * `-A`: Muestra la carga útil (payload) de los paquetes en formato ASCII, útil para ver datos de texto.
  * `-w <archivo.pcap>`: Escribe el tráfico capturado a un archivo en formato `.pcap`. Es el formato estándar para herramientas como Wireshark.
  * `-r <archivo.pcap>`: Lee y muestra el contenido de un archivo `.pcap` en lugar de capturar en tiempo real.

### Expresiones de Filtro

Las expresiones son la parte más potente de `tcpdump`. Se pueden combinar usando `and`, `or` y `not`.

  * **Tipos de filtro:** `host`, `net`, `port`.
  * **Direcciones:** `src` (origen), `dst` (destino).
  * **Protocolos:** `tcp`, `udp`, `icmp`.

### Ejemplos Prácticos

1.  **Capturar todo el tráfico en una interfaz específica:**
    ```bash
    sudo tcpdump -i eth0
    ```
2.  **Ver el tráfico de un host específico (sin resolución de nombres):**
    ```bash
    sudo tcpdump -i eth0 -n host 192.168.1.100
    ```
3.  **Capturar todo el tráfico TCP del puerto 80 (HTTP):**
    ```bash
    sudo tcpdump -i eth0 -nn tcp port 80
    ```
4.  **Capturar el tráfico UDP hacia un puerto específico en una máquina remota:**
    ```bash
    sudo tcpdump -i eth0 -nn udp and dst host 10.0.0.5 and dst port 53
    ```
5.  **Guardar el tráfico filtrado a un archivo para su posterior análisis:**
    ```bash
    sudo tcpdump -i eth0 -nn tcp port 22 -w ssh_capture.pcap
    ```

**Nota:** Es casi siempre necesario ejecutar `tcpdump` con privilegios de superusuario (`sudo`) para poder acceder a las interfaces de red.