# EMPEZANDO CON JENKINS

Jenkins en general es una aplicación creada en java y se usa para integración continua  y general Entregables. 



Jenkins, como servidor de integración continua, permite planificar y realizar multitud de tareas, simplificando los procesos involucrados en el ciclo de vida de un proyecto. Algunas de sus características más importantes son:

* Comprobación cada cierto periodo de tiempo si se ha realizado algún commit en el repositorio de control de versiones (GIT), y en caso de ser así, compilar el código y ejecutar las pruebas para testearlo.
* Notificación de errores que se hayan detectado tras las ejecución de pruebas, por ejemplo vía mail, twitter, chat, etc.
* Generación y publicación de binarios.
* Ejecución de métricas de calidad y visualización los resultados.
* Generación de documentación asociada a un proyecto.

Para mas información ver este excelente [Tutorial](http://www.robertocrespo.net/kaizen/aprende-a-montar-un-entorno-de-integracion-continua-iv-jenkins/)


## Instalando Jenkins

PASO 1: [Descargar jenkins](https://jenkins.io/download/).

PASO 2: Ir a la carpeta donde tengas descargado el instalador de jenkins(.war(mejor opción), .msi).

    Nota: Si es .msi solo tienes que darle clic y siguiente siguiente. inicias jenkins en el navegador http://localhost:8080

PASO 3: Ir a la ventana de comando de tu sistema operativo(si es .war)
       -- posicionarse en carpeta donde tienes el .war
	   -- Escribir el comando **java -jar jenkins.war**
	   -- En esta ventana cuando se esta realizando el despliegue del jenkins se mostrar una clave que te la pedirá jenkins la primera vez que entres en el navegador con la url de jenkins.
	   
PASO 4: Ir al navegador y poner la siguiente url:http://localhost:8080
       -- Diguitar la clave de contingencia sumistrada en el paso anterior.
	   -- Al dar clic en el boton continua te mostrara una ventana donde te pide que instales los pluggines por defecto(Recomendado) o seleccionar los plugigin deseado. 
       -- Después de esto se cargara una nueva ventana donde te pide que digites las credenciales de acceso como administrador.

PASO 5: Ir a la ventana de login de jenkins y loggearse para empezar.



## Cambiando de directorio[opcional]

## Configurando Jenkins 



