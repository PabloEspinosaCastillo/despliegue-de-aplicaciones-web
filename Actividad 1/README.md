3. Analiza los headers de las peticiones cuando inicias sesión en el Moodle y comprende
cómo se obtiene el token. Para ello, necesitamos saber de dónde salen TODOS los
datos sensibles que se envían.

![token](https://github.com/PabloEspinosaCastillo/despliegue-de-aplicaciones-web/assets/144775391/a64f6f04-433e-4df4-b6e6-d0393cdecc3d)


4. ¿A qué puerto se reciben normalmente las peticiones del protocolo HTTP? ¿A qué
capa del modelo TCP/IP se encuentra el protocolo HTTP? ¿Y los protocolos TCP,
UDP, e IP?
-Normalmente se reciben en el puerto 80
-Capa 4 o de aplicación
-En la capa de transporte del modelo TCP/IP 


5. ¿Cuál es el significado de la siguiente respuesta de un servidor?
HTTP/1.1 302 Found
Location: http://www.example.com/test/index2.php

Es un código de estado HTTP que indica una redirección temporal.
Indica que el recurso solicitado se a movido temporalmente a la URL dada por las cabeceras Location

6. Utilizando el filtro de captura para la interfaz de red de Wireshark, analiza la petición
al host: www.google.com. Mostrando la cabecera IP, la dirección IP de tu ordenador y
la del servidor. Comprueba que, poniendo esa IP en el navegador, accedas a Google.




