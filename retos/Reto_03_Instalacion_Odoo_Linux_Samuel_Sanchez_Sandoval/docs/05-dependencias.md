# 05 — Dependencias (Python, wkhtmltopdf, librerías)

1. Instala Python y paquetes de compilación:  
   Si trabajas en un servidor Ubuntu Python viene ya preconfigurado y preinstalado, si no es el caso, los siguientes comandos deberian solventarlo
   ```bash
   sudo apt install python3
   ```
   ```bash
   sudo apt install python3-dev
   ```
   ```bash
   sudo apt install python3-pip
   ```

2. Instala **wkhtmltopdf** compatible (para reportes PDF).  
   Obtenemos el paquete de este enlace mediante este comando
   ```bash
   wget https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-2/wkhtmltox_0.12.6.1-2.jammy_amd64.deb
   ```
   ![Obtener paquete](/retos/Reto_03_Instalacion_Odoo_Linux_Samuel_Sanchez_Sandoval/assets/img/05-dependencias/install_whtmltopdf.png)   
   Tras obtener el paquete lo instalamos. **DARA ERROR, NO SE PREOCUPE**  
   ```bash
   sudo dpkg -i wkhtmltox_0.12.6.1-2.jammy_amd64.deb
   ```
   ![Instalar paquete](/retos/Reto_03_Instalacion_Odoo_Linux_Samuel_Sanchez_Sandoval/assets/img/05-dependencias/instalamos_paquete.png)  
   Entonces tras dar error deberas ejecutar este comando para completar la instalación correctamente sin errores
   ``bash
   sudo apt install -f
   ```


3. Verifica versiones:  
   Con estos comandos puedes comprobar el estado y version de las instalaciones
   ```bash
   python3 --version
   ```
   ```bash
   wkhtmltopdf --version
   ```
   ![Comprobar paquetes](/retos/Reto_03_Instalacion_Odoo_Linux_Samuel_Sanchez_Sandoval/assets/img/05-dependencias/verificar_instalaciones.png) 


> Resultado esperado: dependencias instaladas y comprobadas.
