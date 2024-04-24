# jenkins-bash
# Author: Efrain Benitez

### Descripción del Proceso
Este repositorio contiene un proyecto que utiliza Jenkins local para ejecutar un pipeline que realiza ciertas acciones en un entorno Linux. A continuación, se detalla el proceso realizado:

Configuración del Repositorio en Jenkins:
Se ha configurado un repositorio en Jenkins local.
Se proporcionó la ruta del repositorio y las credenciales de GitHub en la configuración de Jenkins para acceder al código fuente.
Pipeline en Jenkins:
Se ha creado un pipeline en Jenkins que utiliza un Jenkinsfile para definir las etapas del proceso.
El Jenkinsfile está configurado para:
Clonar automáticamente el repositorio desde GitHub utilizando la ruta y las credenciales especificadas en la configuración de Jenkins.
Otorgar permisos de ejecución al archivo main.sh.
Ejecutar el script main.sh dentro del pipeline, pasando como parámetro el nombre del proceso a buscar.
Ejecución del Pipeline:
Cuando se activa el pipeline en Jenkins, se inicia la ejecución del Jenkinsfile.
Jenkins clona el repositorio desde GitHub y ejecuta el script main.sh dentro del pipeline, utilizando el nombre del proceso proporcionado como parámetro.
Este proceso permite automatizar ciertas tareas en un entorno Linux utilizando Jenkins y GitHub de manera integrada, lo que facilita el desarrollo y la gestión de proyectos 