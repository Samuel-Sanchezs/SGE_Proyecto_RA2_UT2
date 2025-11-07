# 03 — Preparación del sistema

1. Actualiza índices y paquetes:
   ```bash
   sudo apt update
   ```

      En este orden realiza primer el update  
   ![Pagina web](/retos/Reto_03_Instalacion_Odoo_Linux_Samuel_Sanchez_Sandoval/assets/img/03-preparacion_sistema/update.png)
   ```bash
   sudo apt upgrade
   ```
      Y luego el upgrade  
   ![Pagina web](/retos/Reto_03_Instalacion_Odoo_Linux_Samuel_Sanchez_Sandoval/assets/img/03-preparacion_sistema/upgrade.png)

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
   
> Resultado esperado: sistema actualizado y listo para instalar dependencias.
