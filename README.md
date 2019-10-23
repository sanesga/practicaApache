<h1 style="text-align:center"> Práctica Apache</h1>

![logo](img/logo.png)

**Apache** es un servidor web de código abierto desarrollado por Apache Software Foundation. Se trata de un servidor de grado comercial robusto y seguro que se adhiere a todos los estándares HTTP. Ha sido el líder del mercado desde que apareció en 1995 y sigue siéndolo actualmente. Una de sus características principales es que tiene la capacidad de funcionar en múltiples plataformas.

**Características:**

- Gratuito, no requiere licencia.
- Se puede modificar para ajustar el código y/o corregir errores.
- Ofrece la posibilidad de agregar más funciones y módulos.
- Altamente fiable.
- Instalación fácil.
- Los cambios realizado se registran de forma inmediata, incluso sin reiniciar el servidor.
- Puede ejecutarse en casi cualquier sistema operativo.
- Regularmente mantenido y actualizado.
- Integración con otras aplicaciones creando los paquetes XAMPP, LAMPP y MAMP.
- Posibilidad de modificar su configuración.
- Bajo rendimiento si recibe miles de requests simultáneos.

## **1. SITIO 1**

Este primer sitio permitirá visualizar una página php.

- Creación del host virtual:

  ```
  sudo mkdir -p /var/www/sitioPhp
  ```

  ![logo](img/captura1.png)

- Otorgamos permisos al directorio creado para usuarios distintos a root:

   ```
  sudo chown -R $USER:$USER /var/www/sitioPhp/
   ```

- Damos permisos en el directorio web general _(/var/www)_ para que todos sus archivos y directorios puedan ser servidos correctamente.

   ```
  sudo chown -R 755 /var/www/
   ```

- Creamos una carpeta html dentro de nuestro host virtual e introducimos nuestra página php en el interior.

  ![logo](img/captura2.png)

  ![logo](img/captura3.png)







Características:

- Estar publicada en el puerto 82.


- El directorio donde se encuentra el contenido será /var/wwww/sitioPhp.
- Los logs se sitúan en el directorio /etc/logs/sitioPhp.
- Debe disponer de un fichero de log (log_personalizado.log) que mostrará la traza generada por un CustomLog cuyo formato será _"%t%h%m%>s"_, al cual se le asociará el nombre PhpLogFormat.
- Dispone de una página que se mostrará al acceder a una ruta que no exista, mostrando el mensaje _"Página no encontrada"_.






