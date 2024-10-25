# Variables de Entorno
### ¿Qué son las variables de entorno
Las variables de entorno son un mecanismo utilizado por los sistemas operativos para almacenar información y configuraciones globales que afectan el comportamiento de procesos y aplicaciones que se ejecutan en ese sistema. Estas variables contienen información sobre el entorno del sistema, como la ubicación de directorios, las configuraciones de red, credenciales, preferencias de usuario, entre otras.

### Para crear un contenedor con variables de entorno?

```
docker run -d --name <nombre contenedor> -e <nombre variable1>=<valor1> -e <nombre variable2>=<valor2>
```

### Crear un contenedor a partir de la imagen de nginx:alpine con las siguientes variables de entorno: username y role. Para la variable de entorno rol asignar el valor admin.

![Imagen](img/ing8.png) 
# CAPTURA CON LA COMPROBACIÓN DE LA CREACIÓN DE LAS VARIABLES DE ENTORNO DEL CONTENEDOR ANTERIOR
![Imagen](img/img9.png) 

### Crear un contenedor con mysql:8 , mapear todos los puertos
![Imagen](img/img10.png) 


### ¿El contenedor se está ejecutando?
No!
![Imagen](img/img11.png) 


### Identificar el problema
![Imagen](img/img12.png) 


### Eliminar el contenedor creado con mysql:8 
![Imagen](img/img13.png) 


### Para crear un contenedor con variables de entorno especificadas
- Portabilidad: Las aplicaciones se vuelven más portátiles y pueden ser desplegadas en diferentes entornos (desarrollo, pruebas, producción) simplemente cambiando el archivo de variables de entorno.
- Centralización: Todas las configuraciones importantes se centralizan en un solo lugar, lo que facilita la gestión y auditoría de las configuraciones.
- Consistencia: Asegura que todos los miembros del equipo de desarrollo o los entornos de despliegue utilicen las mismas configuraciones.
- Evitar Exposición en el Código: Mantener variables sensibles como contraseñas, claves API, y tokens fuera del código fuente reduce el riesgo de exposición accidental a través del control de versiones.
- Control de Acceso: Los archivos de variables de entorno pueden ser gestionados con permisos específicos, limitando quién puede ver o modificar la configuración sensible.

Previo a esto es necesario crear el archivo y colocar las variables en un archivo, **.env** se ha convertido en una convención estándar, pero también es posible usar cualquier extensión como **.txt**.
```
docker run -d --name <nombre contenedor> --env-file=<nombreArchivo>.<extensión> <nombre imagen>
```
**Considerar**
Es necesario especificar la ruta absoluta del archivo si este se encuentra en una ubicación diferente a la que estás ejecutando el comando docker run.

### Crear un contenedor con mysql:8 , mapear todos los puertos y configurar las variables de entorno mediante un archivo
![Imagen](img/img14.png) 


# CAPTURA CON LA COMPROBACIÓN DE LA CREACIÓN DE LAS VARIABLES DE ENTORNO DEL CONTENEDOR ANTERIOR 
![Imagen](img/img15.png) 

### ¿Qué bases de datos existen en el contenedor creado?
![Imagen](img/img16.png) 
