# 11 — Problemas comunes (FAQ)

- **PostgreSQL no accesible** → Revisa servicio.
    Puedes revisar su servicio con el siguiente comando
    ```bash
    sudo systemctl status postgresql
    ```
    Con ello puedes ver si tiene algún error al iniciar o funciona correctamente
    También puedes intentar acceder a la base de datos con este comando
    ```bash
    psql -U nombre_usuario -h 127.0.0.1 -W
    ```
    Y poder comprobar los permisos que tiene el usuario  
- **Servicio falla al arrancar** → Revisa `journalctl -u odoo` y `odoo.log`.  
    Puedes comprobar los distintos archivos los cuales tienes acceso y comprobar que todos estén correctos, si crees que no son el caso, puedes intentar ejecutar el servicio de Odoo y revisar sus fallos con el siguiente comando  
    ```bash
    sudo systemctl status odoo.service
    ```
    Y si sigue sin funcionar puedes revisar el log de Odoo que es donde lo creaste anteriormente.