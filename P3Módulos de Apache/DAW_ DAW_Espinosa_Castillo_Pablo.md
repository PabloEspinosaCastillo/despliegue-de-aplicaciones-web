1

![1](https://github.com/PabloEspinosaCastillo/despliegue-de-aplicaciones-web/assets/144775391/b597d6d7-a92a-4c8b-b535-668d730fc73f)
![2](https://github.com/PabloEspinosaCastillo/despliegue-de-aplicaciones-web/assets/144775391/10eb7466-fe05-46d3-bca2-b60db811585f)

El mod_info proporciona informació detallada sobre la configuració i l'estat del server d'Apache2. Es pot utilitzar per fer diagnóstics, verificar la configuració, identificar móduls etc. 

2

Per ocultar la versió del sistema i sistema de apache hem de editar el archiu sudo nano /etc/apache2/conf-enabled/security.conf buscar on posa ServerTokens i cambiar el seu valor a "Prod" i el ServerSignature a "Off".

![3](https://github.com/PabloEspinosaCastillo/despliegue-de-aplicaciones-web/assets/144775391/7abdb87b-57d1-4aef-96f0-7fd5fb6a82ea)

![4](https://github.com/PabloEspinosaCastillo/despliegue-de-aplicaciones-web/assets/144775391/b5a11325-474b-4e04-b5ef-4590d4e9e256)

Després guardem els cambis i reiniciem 

![5](https://github.com/PabloEspinosaCastillo/despliegue-de-aplicaciones-web/assets/144775391/bbb800ce-3c40-4d42-bac9-69c0a9461a4a)
![6](https://github.com/PabloEspinosaCastillo/despliegue-de-aplicaciones-web/assets/144775391/fcaa373d-70ca-4a15-9b9d-c3ca3a619e56)

3

