# 06 — Instalación de Odoo


1. Añade repositorio/clave y luego instala `odoo`:  
   Ponemos este codigo para bajar el paquete de ODoo 19.
   ```bash
   wget -q -O - https://nightly.odoo.com/odoo.key | sudo gpg --dearmor -o /usr/share/keyrings/odoo-archive-keyring.gpg
   ```
   Introducimos este codigo para continuar la instalación
   ```bash
   echo 'deb [signed-by=/usr/share/keyrings/odoo-archive-keyring.gpg] https://nightly.odoo.com/19.0/nightly/deb/ ./' | sudo tee /etc/apt/sources.list.d/odoo.list
   ```
   Y terminamos de instalarlo.
   ```bash
   sudo apt-get update && sudo apt-get install odoo
   ```
   Si todo esto no funciona ejecuta estos distintos comandos para solucionar los problemas de clave a la hora de la instalación
   Borramos los directorios originales
   ```bash
   sudo rm -f /usr/share/keyrings/odoo-archive-keyring.gpg
   sudo rm -f /etc/apt/sources.list.d/odoo.list
   ```
   Volvemos a bajar la clave desde otro enlace
   ```bash
   sudo mkdir -p /usr/share/keyrings/
   curl -fsSL https://nightly.odoo.com/odoo.key | sudo gpg --dearmor -o /usr/share/keyrings/odoo-archive-keyring.gpg
   ```
   Agregamos el repositorio
   ```bash
   echo "deb [signed-by=/usr/share/keyrings/odoo-archive-keyring.gpg] https://nightly.odoo.com/19.0/nightly/deb/ ./" | sudo tee /etc/apt/sources.list.d/odoo.list
   ```
   Y volvemos a intentar instalarlo
   ```bash
   sudo apt-get update && sudo apt-get install odoo
   ```




> Resultado esperado: binarios/código de Odoo instalados.
