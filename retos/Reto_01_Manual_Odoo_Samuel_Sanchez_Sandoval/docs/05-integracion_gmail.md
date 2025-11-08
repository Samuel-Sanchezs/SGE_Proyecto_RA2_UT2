# 05 — Integración con Gmail (OAuth GCP + Add-on)

> Estructura orientativa

## Requisitos
- Cuenta Google Cloud (GCP).

## Pasos resumidos
Debemos acceder al apartado de opciones generales en ajustes y activar el plugin de correo  
![Integraciones Pluggin](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/05-integracion_gmail/plugin_correo.png)  
Vamos al gmail, le damos al + que aparece a la derecha y se nos desplegara el Google Workspace donde buscaremos Odoo e instalaremos Oodo Inbox Addin  
![Addon Odoo](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/05-integracion_gmail/addon_odoo.png)  
Gestionamos todos los permisos que nos pida iniciando sesión en nuestra cuenta, ya hecho aparecerá a la derecha  
![Google Oauth](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/05-integracion_gmail/addon_instalado.png)  
Al abrir el addon te pedirá que para empezar abras un correo de ejemplo  
![Correo Ejemplo](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/05-integracion_gmail/falta_login.png)  
Como se puede ver, nos falta hacer login en nuestra cuenta, le daremos al boton de Login e introduciremos el enlace a nuestra pagina de Odoo  
![Login](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/05-integracion_gmail/login.png)  
Una vez inicies sesión te aparecerá una pestaña para permitir a Gmail acceder a tu base de datos  
![Gmail Permiso](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/05-integracion_gmail/permitir_acceso.png)  
Debería salir Succes si todo se ha hecho de manera correcta.  
Una vez activado tomamos de nuevo el ejemplo del correo de Odoo, donde podemos ver la información de toda la empresa.  
![Odoo Addon Funcional](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/05-integracion_gmail/informacion_completa.png)  
Puedes añadir a la empresa del correo dandole al + junto a su nombre en el addon para poder crear oportunidades y/o tareas en el.  
![Oportunidades](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/05-integracion_gmail/oportunidades_comerciales.png)  
Volviendo a los ajustes volvemos a integraciones y le damos a autenticación Oauth.  
![Oauth](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/05-integracion_gmail/plugin_correo.png)  
Una vez activada accedemos a los Proveedores Oauth.  
![Proveedores Oauth](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/05-integracion_gmail/oauth.png)  
Seleccionamos el de Google  
![Google Oauth](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/05-integracion_gmail/google_oauth.png)  
Vamos a introducir el ID de cliente, para ello vamos a Google y buscamos Google Cloud Console.   
![Google console](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/05-integracion_gmail/google_console.png)  
Le damos a crear un nuevo proyecto  
![Nuevo proyecto](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/05-integracion_gmail/crear_proyecto.png)  
Le ponemos cualquier nombre, por ejemplo Odoo-test  
![Odoo test](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/05-integracion_gmail/odoo_test.png)  
Una vez dentro del proyecto vamos a darle a la barra de búsqueda superior y vamos a buscar gmail y hacer click en Gmail API  
![Google Oauth](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/05-integracion_gmail/gmail_api.png)  
Y le damos a habilitar, una vez habilitada le damos a crear credenciales  
![Crear credenciales](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/05-integracion_gmail/crear_credenciales.png)  
Seleccionamos la api de gmail y activamos los datos de los usuarios  
![Tipo de credencial](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/05-integracion_gmail/api_gmail.png)  
Le damos a siguiente, ahora le ponemos nombre a la aplicación, puede ser cualquiera, ponemos nuestro correo electrónico y volvemos a poner nuestro correo en información de contacto del desarrollador  
![Consentimiento Oauth](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/05-integracion_gmail/consentimiento_oauth.png)  
Le das a guardar y continuar, y en la siguiente pantalla seleccionamos agregar permisos y seleccionamos los siguientes  
![Google permisos](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/05-integracion_gmail/actualizar_permisos.png)  
![Google permisos 2](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/05-integracion_gmail/actualizar_permisos_2.png)  
Una vez seleccionados, le damos a actualizar, le damos a guardar y continuar.  
En la siguiente pantalla le damos a aplicacion web y volvemos a poner el nombre de la app  
![Google aplicacion web](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/05-integracion_gmail/aplicacion_web.png)  
Mas abajo vamos a poner la URL de redireccionamiento autorizado. **IMPORTANTE** el enlace a poner es el siguiente:  
https://nombre.odoo.com/google_gmail/confirm  
Donde pone nombre tendrás que sustituirlo por tu nombre de pagina Odoo  
![Google url rediccionamiento](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/05-integracion_gmail/enlace_nombre.png)  
Accedemos a nuestras credenciales ya terminado todo lo anterior  
![Google credenciales](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/05-integracion_gmail/credenciales.png)  
Una vez dentro de nuestra credencial debemos copiar nuestra ID de cliente y copiarla de vuelta en Oauth de Google  
![Google id cliente](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/05-integracion_gmail/id_cliente.png)  
![Google Oauth Id](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/05-integracion_gmail/odoo_id_cliente.png)  
Una vez hecho esto y guardado si volvemos a ajustes al apartado de correos electrónicos, le damos a utilizar servidores de correo electrónico personalizado y en la función de usar correo de Gmail le introducimos el ID y el secreto de la aplicación de Google cloud  
![Google Correos](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/05-integracion_gmail/servidores_correo_electronico.png)  
![Gmail ID](/retos/Reto_01_Manual_Odoo_Samuel_Sanchez_Sandoval/assets/img/05-integracion_gmail/claves_gmail.png)  
Una vez hecho esto ya podríamos controlar nuestro correo electrónico desde Odoo  

