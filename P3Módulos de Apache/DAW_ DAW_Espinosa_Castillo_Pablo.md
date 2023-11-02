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

Per crear les carpetas public i private hem de picar dos mkdir i a la carpeta publica fer un chmod 755 per fer-la pública. 
![appache](https://github.com/PabloEspinosaCastillo/despliegue-de-aplicaciones-web/assets/144775391/c6108216-9109-42bc-9d65-ec715970ee06)
Seguidament hem de crear un archiu .htaccess dintre de la carpeta principal del servidor amb el seguent codi:
![htaccess](https://github.com/PabloEspinosaCastillo/despliegue-de-aplicaciones-web/assets/144775391/65da7c77-1469-4ba0-ab28-5541d60debd0)
Finalment guerdem els canivs, reiniciem el servidor de apache i cerquem la carpeta public.
![restart](https://github.com/PabloEspinosaCastillo/despliegue-de-aplicaciones-web/assets/144775391/49547a39-45ad-45fe-b0d4-e59fe8da2bb8)
![public](https://github.com/PabloEspinosaCastillo/despliegue-de-aplicaciones-web/assets/144775391/36410418-62c3-4dc3-b5e0-2ced63e5089c)

4

He intentat investigar el motiu però no he trobat res que resolgui el perquè funciona sense tocar res del mòdul mod_rewrite, però m'agradaria saber-ho.
![wwwpublic](https://github.com/PabloEspinosaCastillo/despliegue-de-aplicaciones-web/assets/144775391/f44a7c87-cb49-438a-a5d4-d62ae419a108)

5

Para personalitzar el aspecte primer ens aseguram de que el autoindex està habilitat 
![mod](https://github.com/PabloEspinosaCastillo/despliegue-de-aplicaciones-web/assets/144775391/4c0b6c15-7aa2-412f-9c8d-c79864cd2f62)
Obrim el archiu de configuració apache2.conf
![apache1](https://github.com/PabloEspinosaCastillo/despliegue-de-aplicaciones-web/assets/144775391/38e43136-3616-483a-bc73-a98ae966a790)
Dintre d'aquest ens asegurem de que en <Directory /var/www/html> es trobi l'opció Options Indexes FollowSymLinks activada
![indexes](https://github.com/PabloEspinosaCastillo/despliegue-de-aplicaciones-web/assets/144775391/3bd6eacf-e666-4110-bfde-893a41d505d3)
Guardem i reiniciem.
Per utilitzar el archiu css hem d'editar la configuració novament. Aquesta vegada hemm de trobar <Directory /var/www/html> (en el meu cas l'he tingut que crear) i afegir el seguent:
![html](https://github.com/PabloEspinosaCastillo/despliegue-de-aplicaciones-web/assets/144775391/fb068052-0dfd-4fcd-83bd-0056fc974ba9)









