Ejercicio 1

![DebianPablo](https://github.com/PabloEspinosaCastillo/despliegue-de-aplicaciones-web/assets/144775391/96bd04c4-0d90-4917-87d0-f0313abf6843)

![Apache](https://github.com/PabloEspinosaCastillo/despliegue-de-aplicaciones-web/assets/144775391/0b2444e0-3531-4132-8822-1b9cd90264b8)

Ejercicio 2

Una petición GET es un método utilizado en el protocolo HTTP para solicitar datos de un recurso específico en un servidor. Esta petición no tiene efectos secundarios en el servidor.

Una petición POST es un método utilizado en el protocolo HTTP para enviar datos al servidor para su procesamiento. Los parámetros y datos se envían en el cuerpo de la petición en lugar de la URL no como con GET. Esta petición crea un nuevo recurso o se actualiza uno existente en el servidor.

Una petición PUT es un método utilizado en el protocolo HTTP para actualizar un recurso específico en el servidor. Similar a una petición POST, pero en este caso, se espera que el servidor reemplace completamente el recurso existente con los datos proporcionados.

Una petición DELETE es un método utilizado en el protocolo HTTP para eliminar un recurso específico en el servidor. Al enviar una petición DELETE, se indica al servidor que elimine el recurso solicitadoy elimina el recurso del servidor.

Ejercicio 3

![4444](https://github.com/PabloEspinosaCastillo/despliegue-de-aplicaciones-web/assets/144775391/ee9edeea-678d-4614-8b66-bf9136347637)

![web](https://github.com/PabloEspinosaCastillo/despliegue-de-aplicaciones-web/assets/144775391/5b1b07cc-67e2-43af-8c11-8c24c7299838)

Antes de buscar la web he intentado cambiar un par de cosas que no funcinaban, otras sitios que tenia que cambiar no se enontraban donde deberian estar y no he podido cambiar. Supongo que el error reside ahí y por eso no funciona.

Ejercicio 4


Ejercicio 5

Los archivos de configuración de Apache2 están en /etc/apache2/.

- apache2.conf: Es el archivo principal de configuración de Apache2. Contiene la configuración global, los módulos habilitados y otros ajustes generales.

La diferencia entre sites-available y sites-enabled es que sites-available contiene los archivos de configuración de los sitios web disponibles, pero no están activos hasta que se creen enlaces simbólicos en sites-enabled. Esto permite habilitar y deshabilitar fácilmente los sitios web sin modificar los archivos de configuración.

La diferencia entre mods-available contiene los archivos de configuración de los módulos disponibles, pero no están activos hasta que se creen enlaces simbólicos en mods-enabled. Esto permite habilitar o deshabilitar

Ejercicio 6

Los ficheros de ejecucion de Apache2 se encuentran en diferentes ubicaciones dependiendo del sistema operativo:

En sistemas basados en Debian la ubicacipn principal es /etc/apache2/.
En sistemas basados en Red Hat la ubicacion principal es /etc/httpd/.
El control del servicio se realiza utilizando el binario de ejecucion de Apache2 se encuentra en /usr/sbin/.

Iniciar: El comando utilizado para iniciar el servidor Apache2 es "sudo service apache2 start" en Debian. Este comando inicia el servidor y comienza a escuchar las solicitudes entrantes.
Detener: El comando utilizado para detener el servidor Apache2 es "sudo service apache2 stop" en Debian. Este comando detiene el servidor y deja de escuchar las solicitudes entrantes.
Recargar: El comando utilizado para recargar la configuración del servidor Apache2 es "sudo service apache2 reload" en Debian. Este comando recarga la configuración del servidor sin detenerlo, lo que permite aplicar cambios en la configuración.
Reiniciar: El comando utilizado para reiniciar el servidor Apache2 es "sudo service apache2 restart" en Debian. Este comando detiene y luego inicia nuevamente el servidor, lo que permite aplicar cambios en la configuración y reiniciar el servicio.
La comprobación de sintaxis se realiza utilizando el binario de Apache, que generalmente se encuentra en /usr/sbin/. El comando utilizado es "sudo apache2ctl configtest" en sistemas basados en Debian. Este comando verifica la sintaxis de la configuración del servidor Apache2 y muestra cualquier error que pueda existir.

Ejercicio 7 

Los ficheros de monitorización de Apache2 se encuentran en la ubicación principal del servidor Apache2 generalmente es /var/log/apache2/.

- error.log: Este archivo registra todos los errores ocurridos en el servidor Apache2. Es útil para identificar y solucionar problemas en el servidor.

- access.log: Este archivo registra todas las solicitudes de acceso al servidor Apache2. Proporciona información sobre las visitas al servidor puede ser utilizado para analizar el tráfico y realizar estadísticas.

La rotación de logs en Apache2 es importante para evitar que los archivos de log crezcan en tamaño indefinidamente y ocupen demasiado espacio en disco. La rotación de logs se configura a través del archivo de configuración de Apache2, generalmente ubicado en /etc/apache2/apache2.conf. En este archivo, se pueden especificar los parámetros de rotación de logs, como el tamaño máximo de cada archivo de log y la cantidad de archivos de log a mantener.

Para realizar la monitorización en tiempo real de los accesos en el servidor Apache2, se puede utilizar la herramienta "tail -f" en la línea de comandos. Para monitorear el archivo access.log en tiempo real se puede ejecutar el siguiente comando: "tail -f /var/log/apache2/access.log". Esto mostrará las últimas entradas en el archivo y se actualizará automáticamente a medida que se agreguen nuevas entradas.

Para analizar y obtener estadísticas visuales a partir de los logs de Apache2, se puede utilizar la herramienta GoAccess es una herramienta de línea de comandos que analiza los archivos de log de Apache2 y genera informes y estadísticas interactivas. Para instalar GoAccess, se puede utilizar el gestor de paquetes del sistema operativo. En sistemas basados en Debian se puede ejecutar el siguiente comando: "sudo apt-get install goaccess". Se puede ejecutar GoAccess especificando el archivo de log a analizar, por ejemplo: "goaccess /var/log/apache2/access.log". Esto mostrará un informe con estadísticas visuales sobre el tráfico del servidor.

Ejercicio 8

Un Firewall es una medida de seguridad utilizada para controlar el trafico de red y protegerla. 
Su funcion principal es filtrar y bloquear el trafico no autorizado permitiendo paso solo a las conexines con las condiciones de seguridad establecidas
Un Firewall es necesario para prevenir ataques como malware, acceso a datos no autorizados de una red o el sistema...

Instalacion firewall:

Ejercicio 9

En una URL encontramos:
-Protocolo: El protocolo es el HTTP, HTTPS u otros. Se utilizan para la transferencia de datos.
-Puerto: El puerto es el puerto de red que se utliza en HTTP que seria 80 y en HTTPS 443. 
-Parametros: Son valores o datos adicionales que se envian al servidor a través de la URL.
-Dominio: El dominio es el nombre del sitio web https://www.ejemplo.com, un ejemplo de subdominio seria www.
-Ruta: La ruta es la ubicacion de la web por ejemplo: https://www.ejemplo.com/Documentos/archivo.html
-Fragmento: Hace referenecia a una seccion especifica del recurso, ejemplo: https://www.ejemplo.com/pagina.html#prueba1


Ejercicio 10

El http es un protocolo de transferencia de datos que se utiliza en todo el mundo.

Ejercicio 11

Un archivo .htaccess es un archivo de configuración utilizado en servidores web Apache para controlar la configuració y el comportamiento de un directorio especifico o de todo el sitio web. 
Como ejemplo de uso se podria utilizar para la reescritura del URL de Apache, cuando el usuario acceda a una URl el servidor la reescribira internamente y mostrara el contenido de la URL deseada.







