# 07 — Calendario y Citas

## Sincronización con Google Calendar
Vamos a sincronizar el calendario de Odoo con el de Google Calendar en este apartado.  
Empezaremos creando un proyecto en Google Cloud  

![Crear proyecto](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/07-calendario_y_citas/crear_proyecto.png)  
Una vez creado el proyecto seguimos el mismo proceso que en la integración de Gmail pero cambiando el nombre a Google Calendar o cualquiera al gusto  
![Odoo calendar](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/07-calendario_y_citas/odoo_calendar.png)  
Elegimos la Api de Google Calendar  
![Calendario Api](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/07-calendario_y_citas/calendar_api.png)  
Habilitamos la api  
![Habilitar Api](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/07-calendario_y_citas/habilitar_api.png)  
![Crear credenciales](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/07-calendario_y_citas/crear_credenciales.png)  
![Tipo credencial](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/07-calendario_y_citas/tipo_credencial.png)  
Introducimos nuestro nombre y correo  
![Oauth](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/07-calendario_y_citas/consentimiento_oauth.png)  
Le ponemos los permisos a continuación  
![Permisos](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/07-calendario_y_citas/permisos.png)  
![Primer permiso](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/07-calendario_y_citas/primer_permiso.png)  
![Permisos1](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/07-calendario_y_citas/permisos1.png)  
![Permisos2](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/07-calendario_y_citas/permisos2.png)  
Una vez hecho todo esto elegiremos que nuestra app sea web y le pondremos nombre  
![App web](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/07-calendario_y_citas/id_cliente_oauth.png)  
Y añadiremos la url de redireccionamiento que es:  
https://nombre.odoo.com/google_account/authentication  
Donde *nombre* deberá ser sustituido por el nombre de tu pagina de Odoo  

Ye hecho cogeremos nuestras credenciales  
![Credenciales](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/07-calendario_y_citas/credenciales.png)  
Pinchamos en Odoo Calendar  
![Copiar credenciales](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/07-calendario_y_citas/copiar_credenciales.png)  
Una vez copiada la credencial y el numero secreto, nos vamos a ajustes en nuestro servidor Odoo y accedemos a ajustes de calendario reconocible por su icono y en el apartado de Google calendar lo activamos y pegamos la credencial y el numero secreto  
![Calendario google](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/07-calendario_y_citas/configuracion_gmail.png)  
