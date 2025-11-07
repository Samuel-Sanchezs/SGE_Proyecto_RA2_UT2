# 03 — Preparación del sistema

1. Actualiza índices y paquetes:
   ```bash
   sudo apt update
   ```

      En este orden realiza primer el update  
   ![Update](/retos/Reto_03_Instalacion_Odoo_Linux_Samuel_Sanchez_Sandoval/assets/img/03-preparacion_sistema/update.png)
   ```bash
   sudo apt upgrade
   ```
      Y luego el upgrade  
   ![Upgrade](/retos/Reto_03_Instalacion_Odoo_Linux_Samuel_Sanchez_Sandoval/assets/img/03-preparacion_sistema/upgrade.png)

2. Configura zona horaria e idioma si procede.
   En el caso de que sea necesario cambiar la zona horaria, en el caso de España deberias introducir el siguiente comando
   ```bash
   sudo timedatectl set-timezone Europe/Madrid
   ```
   Y para cambiar el idioma deberias introducir primero el siguiente comando
   ```bash
   sudo apt-get install language-pack-es
   ```
   Instalamos los diccionarios en español
   ```bash
   sudo apt install aspell-es
   ```
   ```bash
   sudo apt install myspell-es
   ```
   Luego vamos a ya seleccionar el idioma que nos hemos bajado, en este caso Español  
   ```bash
   sudo dpkg-reconfigure locales
   ```
   Una vez en el menu que se despliega deberas elegir el idioma que corresponda con el que necesites
   ![Idiomas](/retos/Reto_03_Instalacion_Odoo_Linux_Samuel_Sanchez_Sandoval/assets/img/03-preparacion_sistema/idiomas.png)  
   Le das al Enter una vez lo tengas seleccionado para acceder al proximo menu  
   ![Confirmar Idioma](/retos/Reto_03_Instalacion_Odoo_Linux_Samuel_Sanchez_Sandoval/assets/img/03-preparacion_sistema/configurar_idioma.png)  
   Luego vuelves a confirmar con el Enter y terminarias la instalacion reiniciando el dispositivo
   ```bash
   reboot
   ```
> Resultado esperado: sistema actualizado y listo para instalar dependencias.
