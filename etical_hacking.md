Fases: Se adecuan respectos al contexto
Caja gris
Caja negra

1. Footprinting[huella](https://www.google.com/search?q=que+esfootpring%2Bhacking&num=10&newwindow=1&client=firefox-b-d&sca_esv=c4feb57d21f36445&sxsrf=AE3TifPugdn0oqbZ3K8LNMwS720MnXqeiw%3A1749923460313&ei=hLZNaO_sEtff1sQPqvWLyA0&ved=0ahUKEwjvvvHxvPGNAxXXr5UCHar6AtkQ4dUDCBA&uact=5&oq=que+esfootpring%2Bhacking&gs_lp=Egxnd3Mtd2l6LXNlcnAiF3F1ZSBlc2Zvb3RwcmluZytoYWNraW5nMgcQIRigARgKSNAdUJIJWIQbcAF4AZABAJgBiwGgAc8HqgEDMC44uAEDyAEA-AEBmAIJoAKxCcICChAAGLADGNYEGEfCAgcQIxiwAhgnwgIHEAAYgAQYDcICBhAAGA0YHsICCBAAGAgYDRgewgIIEAAYgAQYogTCAgUQABjvBcICBRAhGKABmAMA4gMFEgExIECIBgGQBgiSBwMxLjigB-cfsgcDMC44uAfpCMIHBzMtNy4xLjHIB6UB&sclient=gws-wiz-serp)

Llamamos Footprinting (también conocido como reconocimiento), a una de las fases previas al ciberataque, es el proceso de recopilar la mayor cantidad de información sobre lo que queremos “hackear” para localizar vulnerabilidades y formas de acceder a él. Para obtener dicha información el “hacker” puede utilizar varias herramientas y procesos.

Si quieres aprender sobre las fases del hacking ético y convertirte en uno de los mejores, te recomendamos encarecidamente nuestro Máster en Dirección de Ciberseguridad, Hacking Ético y Seguridad Ofensiva, enfocado a la empleabilidad y desmárcate del resto en EIP.
Información que recopila el “hacker”

Footprinting es básicamente un paso previo al ciberataque donde el “hacker” recopila toda la información que pueda sobre su víctima para encontrar las formas de acceder al sistema o decidir que ciberataques serían los que tendrían más éxito contra su objetivo.

Normalmente la información que suelen recopilar es:

    Nombre del dominio
    Direcciones IP
    Sistema operativo utilizado
    Información de los empleados
    Números de teléfono
    Direcciones de correo
    Etc.

que es footprinting

Un hacker ético suele dedicar la mayoría de su tiempo en proteger una red u organización, recopilando información sobre el host, la red, los equipos y las personas relacionadas con el sistema, por la fase del Footprinting le ayudará a identificar vulnerabilidades que detectemos durante el reconocimiento y reforzar nuestro sistema ante posibles amenazas.
Tipos de Footprinting

Hay dos tipos de Footprinting que podemos utilizar: Footprinting activo y pasivo:

    Footprinting activo, es el proceso más tedioso para obtener información, donde usaremos herramientas y técnicas para ello. Por ejemplo podemos realizar un barrido de ping para recoger información sobre el objetivo o usar el comando traceroute.

    Footprinting pasivo, en este proceso más “light”, por ejemplo, se revisa el sitio web de una empresa, se visitan los perfiles de los empleados en redes sociales, buscamos en Google del objetivo a hackear o buscamos el sitio web en WHOIS.

Obtener la información de un sitio web es muy fácil, solo hay que acceder a la dirección: https://www.dondominio.com/whois/ y buscar la página que queramos.

Vamos a hacer un ejemplo de WHOIS a la web de Amazon.

## Herramienat a ocupar
[OSINT]()
inteligencia de código abierto (OSINT) es el proceso de recopilación y análisis de información disponible públicamente de fuentes como cuentas de redes sociales, registros gubernamentales y directorios en línea para evaluar amenazas, tomar decisiones o responder preguntas específicas.
[TheHarvester](https://www.osintux.org/documentacion/the-harvester)


2. SCAN/Enumeracion

Host activos
port/Servivios  Nmap


3. Identificar vulnerabilidades

Automatizacion de analisis   
Validacion Manual
Riesgos

Herramienetas
[openvas](https://openvas.org/)

4. - Explotacion

Dev/Exploit
Acceso

Herramientas
[Burp suite](https://portswigger.net/burp)

5. Post Explotacion

Persistencia
Escalacion Privilegios

6. Reporte

Hallazgo
Analisis de impacto


curl: Se utiliza para transmitir datos con sintaxis URL

curl --manual

curl poner_IP
    Entrega de informacion, a traves, de un Json

Instalar libreria para ver Json
    sudo apt-get install jq

curl http://3.86.214.94:30008/ | jq .

-X_Permite especificar el metodo HTTP
curl -X GET  http://3.86.214.94:30008/user/13
curl -X GET  http://3.86.214.94:30008/admin/settings
curl -X POST  http://3.86.214.94:30008/login -d "username=user1&password=password1"
curl -X GET  http://3.86.214.94:30008/admin/users | jq
curl -X GET "http://3.86.214.94:30008/system/info" | jq .   

-----------------------------------------------------------------------------------------------------
Ataque con diccionarios

Instalar
    sudo apt install hashcat
Obtener manual    
    hashcat --help 

    cat /etc/passwd
Manera de trabajar con diccionarios(informacion general)
    hashcat -m 0 -a 0 hash.txt diccionario.txt 
Tratar de romper por medio de fuerza bruta
    hashcat -m 0 hash.txt diccionario.txt --show

cat > hashcat.txt << EOF
a
b
c
EOF

echo -n "4618" | md5sum > ejemplo.txt
more ejemplo.txt
hashcat -m 0 -a 3 ejemplo.txt ?d?d?d?d
echo -n "4618" | sha1sum | cut -d '' -f1 >> ejemplo.txt
hashcat -m 100 -a 0 ejemplo.txt --show
-------------------------------------------------------------------------------

