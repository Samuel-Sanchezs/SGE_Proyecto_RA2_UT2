# 08 — Servicio systemd (`odoo.service`)

1. Crea el servicio en `/etc/systemd/system/odoo.service`:  
Accedemos al archivo mediante nano
   ```bash
   sudo nano /etc/systemd/system/odoo.service
   ```
   Y dentro escribimos todo esto:  
   ```ini
   [Unit]
   Description=Odoo Service
   After=network.target postgresql.service

   [Service]
   Type=simple
   User=odoo
   Group=odoo
   ExecStart=/opt/odoo/venv/bin/python /opt/odoo/odoo-src/odoo-bin -c /etc/odoo/odoo.conf
   Restart=on-failure

   [Install]
   WantedBy=multi-user.target
   ```
2. Recarga y arranca:  
   Una vez hecho, ejecutamos esto para iniciar el servicio
   ```bash
   sudo systemctl daemon-reload
   sudo systemctl enable --now odoo
   sudo systemctl status odoo
   ```

![Obtener paquete](/retos/Reto_03_Instalacion_Odoo_Linux_Samuel_Sanchez_Sandoval/assets/img/08-servicio_systemd/service_status.png) 


