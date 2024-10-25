# COMPLETAR  
Comparando sus conocimientos antes de hacer la práctica con sus conocimientos después de hacer la tarea, explicar los principales aprendizajes logrados para beneficio de su formación profesional.  

Al comparar los conocimientos adquiridos antes y después de realizar la práctica, los principales aprendizajes que he logrado para mi formación profesional son los siguientes:

   - Antes de la práctica, tenía conocimientos limitados sobre la creación y gestión de contenedores en Docker. A través de esta práctica, aprendí a crear contenedores utilizando diferentes imágenes (como `mysql:8` y `wordpress`), a conectarlos a redes específicas y a configurar variables de entorno necesarias para su funcionamiento.
   - Aprendí cómo utilizar redes de Docker para permitir la comunicación entre diferentes contenedores, como en el caso de MySQL y WordPress, garantizando que se puedan comunicar dentro de la misma red (`net-wp`).

   - También comprendí la importancia de los volúmenes persistentes en Docker. Antes, no era consciente de que los datos dentro de un contenedor podrían perderse si no se guardan en un volumen externo. Ahora sé cómo montar volúmenes para asegurar que los datos persistan, incluso si los contenedores se eliminan y se vuelven a crear.

   - Antes de la práctica, no tenía claro cómo conectar aplicaciones (como WordPress) a bases de datos en contenedores separados. Aprendí cómo configurar las variables de entorno correctas para conectar WordPress con un servidor MySQL ejecutándose en otro contenedor, usando `WORDPRESS_DB_HOST`, `WORDPRESS_DB_USER`, `WORDPRESS_DB_PASSWORD`, y `WORDPRESS_DB_NAME`.

   - Al realizar la práctica, enfrenté un problema de conectividad entre contenedores que no podía resolver inicialmente. Entendí como diagnosticar problemas de red en Docker utilizando comandos como `ping` entre contenedores para verificar la conectividad. También me familiaricé más con la estructura y los comandos de Docker para depurar estos problemas, como verificar los logs de contenedores y configurar adecuadamente las redes.

   ```
 Este conocimiento sin duda refuerza mi capacidad para trabajar en entornos más complejos, mejorando mi formación como ingeniera de software.

```
Si solucionó un problema presentado al realizar la práctica también se debe documentar.
