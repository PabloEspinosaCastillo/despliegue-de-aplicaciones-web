1

![1](https://github.com/PabloEspinosaCastillo/despliegue-de-aplicaciones-web/assets/144775391/b597d6d7-a92a-4c8b-b535-668d730fc73f)
![2](https://github.com/PabloEspinosaCastillo/despliegue-de-aplicaciones-web/assets/144775391/10eb7466-fe05-46d3-bca2-b60db811585f)

El mod_info proporciona informació detallada sobre la configuració i l'estat del server d'Apache2. Es pot utilitzar per fer diagnóstics, verificar la configuració, identificar móduls etc. 

2

Para ocultar la versió del sistema i sistema de apache hem de editar el archiu sudo nano /etc/apache2/conf-enabled/security.conf buscar on posa ServerTokens i cambiar el seu valor a "Prod" i el ServerSignature a "Off".

![3](https://github.com/PabloEspinosaCastillo/despliegue-de-aplicaciones-web/assets/144775391/7abdb87b-57d1-4aef-96f0-7fd5fb6a82ea)
