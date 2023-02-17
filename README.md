# vulneravility_scan
Proyecto de escaneo de vulnerabilidades y generación de reportes automático
Este es un script de Bash que utiliza la herramienta de escaneo de puertos Nmap para realizar un escaneo en un segmento de red o un dominio web, y devuelve un informe en formato PDF de los hosts activos, los puertos abiertos y los servicios que corren en ellos, así como un escaneo de vulnerabilidades y evasión de firewalls y WAF.

Este script está diseñado para ser utilizado solo para multas éticas y con el permiso de los propietarios de los activos. El uso inapropiado de este script puede ser ilegal.

# Requisitos
Este script requiere que Nmap esté instalado en su sistema. Si no tiene Nmap instalado, puede hacerlo en Kali Linux con el siguiente comando:
'''
sudo apt install nmap
'''
Además, el script también utiliza las siguientes herramientas para el escaneo de vulnerabilidades y la evasión de firewalls y WAF:

'''
Nikto

wafw00f

Unicornscan

'''

Puede instalar estas herramientas en Kali Linux con los siguientes comandos:
'''
sudo apt install nikto

sudo apt install wafw00f

sudo apt install unicornscan
'''

Finalmente, el script utiliza la herramienta wkhtmltopdfpara generar el informe en formato PDF. Puede instalar esta herramienta en Kali Linux con el siguiente comando:
'''
sudo apt install wkhtmltopdf
'''
# Uso
Para utilizar el script, simplemente descárguelo y déjelos permisos de ejecución:

'''
chmod +x nmap_scan.sh
'''
Luego, puede ejecutar el script con el siguiente comando:

./nmap_scan.sh [opciones]
Las opciones disponibles son las siguientes:


-h: Muestra la ayuda y las opciones disponibles.

-s <dirección_IP/máscara>: Especifica el segmento de rojo a escanear. Por ejemplo: -s 192.168.1.0/24.

-d <dominio>: Especifica el dominio web a escanear. Por ejemplo: -d www.example.com.

-o <nombre_archivo>: Especifica el nombre del archivo de salida en formato PDF. Por ejemplo: -o informe.pdf.

-t <título>: Especifica el título del informe en el archivo PDF. Por ejemplo: -t "Informe de Seguridad".

-l <ruta_logo>: Especifica la ruta del archivo de imagen a incluir como logo en el informe PDF. Por ejemplo: -l /ruta/al/logo.png.

Para un escaneo completo de un segmento de red, puede utilizar el siguiente comando:

./nmap_scan.sh -s 192.168.1.0/24 -o informe.pdf -t "Informe de Seguridad" -l /ruta/al/logo.png

Para un escaneo completo de un dominio web, puede utilizar el siguiente comando:

./nmap_scan.sh -d www.example.com -o informe.pdf -t "Informe de Seguridad" -l /ruta/al/logo.png

# Resultado 
Una vez que se complete el escaneo y se genere el archivo de informe en formato PDF, podrá encontrar el archivo en la ruta especificada en la variable OUTPUT_FILE. El informe contendrá información detallada sobre todos los hosts activos, puertos abiertos, servicios que se ejecutan en ellos y cualquier posible vulnerabilidad detectada.

Es importante tener en cuenta que este script está destinado a ser utilizado solo con fines éticos y con el permiso de los propietarios de los activos. Además, no garantizo que el script pueda evadir todos los firewalls y WAF, por lo que es responsabilidad del usuario asegurarse de que esté utilizando el script de manera responsable y de acuerdo con las leyes y regulaciones locales.

¡Espero que este script sea útil para tus proyectos de seguridad y te ayude a simplificar el proceso de escaneo y generación de informes! Si tienes alguna pregunta o sugerencia, no dudes en hacerlo saber.





