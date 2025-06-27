Aquí tienes el código utilizable del texto proporcionado, centrado principalmente en los comandos `nmap`:

---

## Comandos Nmap para Escaneo de Red

### 1. Identifica tu Propia Dirección IP

Para encontrar tu propia dirección IP (en Kali Linux), usa el siguiente comando:

```bash
ifconfig
```

### 2. Escanea Todos los Dispositivos en tu Red Local

Para escanear toda tu red local e intentar detectar el sistema operativo de los dispositivos conectados, usa este comando. Reemplaza `[PREFIJO_IP_DE_TU_RED]` con los primeros tres octetos de tu dirección IP (por ejemplo, si tu IP es 192.168.1.5, usa 192.168.1).

```bash
sudo nmap -O [PREFIJO_IP_DE_TU_RED].0/24
```

### 3. Escaneo Detallado de un Objetivo Específico

Una vez que hayas identificado una dirección IP objetivo (por ejemplo, del escaneo anterior), puedes realizar un escaneo más exhaustivo para encontrar puertos abiertos, versiones de servicios y otra información valiosa. Reemplaza `[DIRECCION_IP_OBJETIVO]` con la IP de tu objetivo.

```bash
sudo nmap -p- -sV -sC --open -vvv -n -Pn [DIRECCION_IP_OBJETIVO]
```

**Explicación de los parámetros del comando de escaneo detallado:**

* `-p-`: Escanea los 65535 puertos.
* `-sV`: Detecta las versiones de los servicios que se ejecutan en los puertos abiertos.
* `-sC`: Ejecuta scripts predeterminados de Nmap para una enumeración adicional.
* `--open`: Muestra solo los puertos abiertos en la salida.
* `-vvv`: Aumenta la verbosidad para mostrar más detalles durante el escaneo.
* `-n`: Desactiva la resolución de DNS (acelera el escaneo).
* `-Pn`: Trata a todos los hosts como en línea, omitiendo el descubrimiento de hosts (útil si un firewall bloquea los pings).

### 4. Guarda los Resultados del Escaneo en un Archivo

Para guardar los resultados de un escaneo detallado en un archivo para su posterior revisión, añade `-oN [NOMBRE_DE_ARCHIVO]` al comando. Por ejemplo:

```bash
sudo nmap -p- -sV -sC --open -vvv -n -Pn [DIRECCION_IP_OBJETIVO] -oN escaneo
```

Esto guardará la salida en un archivo llamado `escaneo` en el directorio actual.

### 5. Visualiza el Reporte de Escaneo Guardado

Para ver el contenido del archivo de reporte de escaneo guardado:

```bash
cat escaneo
```

---