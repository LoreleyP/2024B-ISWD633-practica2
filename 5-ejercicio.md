## Esquema para el ejercicio
![Imagen](img/esquema-ejercicio5.PNG)

### Crear la red
![Imagen](img/img29.png)


### Crear el contenedor mysql a partir de la imagen mysql:8, configurar las variables de entorno necesarias
![Imagen](img/c5.png)

### Crear el contenedor wordpress a partir de la imagen: wordpress, configurar las variables de entorno necesarias
![Imagen](img/c6.png)

De acuerdo con el trabajo realizado, en la el esquema de ejercicio el puerto a 8080 es el puerto que expones para acceder a WordPress desde el host.

Ingresar desde el navegador al wordpress y finalizar la configuración de instalación.
![Imagen](img/c7.png)


Desde el panel de admin: cambiar el tema y crear una nueva publicación.
Ingresar a: http://localhost:8080/ 
recordar que a es el puerto que usó para el mapeo con wordpress
# COLOCAR UNA CAPTURA DEL SITO EN DONDE SEA VISIBLE LA PUBLICACIÓN.
![Imagen](img/c8.png)


### Eliminar el contenedor wordpress
![Imagen](img/c9.png)

### Crear nuevamente el contenedor wordpress
Ingresar a: http://localhost:8080/ 
recordar que a es el puerto que usó para el mapeo con wordpress

### ¿Qué ha sucedido, qué puede observar?
![Imagen](img/c10.png)
Pierdes la instalación y configuraciones de WordPress al borrar el contenedor.





