# 07 — Configuración de Odoo (`/etc/odoo/odoo.conf`)

1. Crea/edita el archivo de configuración con:  
   Debes acceder al fichero odoo.conf con el siguiente codigo  
   ```bash
   nano /etc/odoo/odoo.conf
   ```
   Y ya dentro del fichero deberias modificar o añadir (en caso de no estar) los siguientes datos.
   ```ini
   [options]
   db_host = 172.0.0.1
   db_port = 5432
   db_user = odoo
   db_password = False
   addons_path = **Dejar el predeterminado de Python3**
   logfile = /var/log/odoo/odoo.log
   xmlrpc_port = 8069
   ```
2. Crea carpetas y permisos si procede:
   Si es necesario o por si acaso crear la carpeta para los logs
   ```bash
   sudo mkdir -p /var/log/odoo && sudo chown odoo:odoo /var/log/odoo
   ```

> Resultado esperado: configuración mínima funcional creada.
