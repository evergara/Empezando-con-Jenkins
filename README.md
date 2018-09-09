# EMPEZANDO CON JENKINS

Jenkins en general es una aplicación creada en java y se usa para integración continua  y general Entregables. 



Jenkins, como servidor de integración continua, permite planificar y realizar multitud de tareas, simplificando los procesos involucrados en el ciclo de vida de un proyecto. Algunas de sus características más importantes son:

* Comprobación cada cierto periodo de tiempo si se ha realizado algún commit en el repositorio de control de versiones (GIT), y en caso de ser así, compilar el código y ejecutar las pruebas para testearlo.
* Notificación de errores que se hayan detectado tras las ejecución de pruebas, por ejemplo vía mail, twitter, chat, etc.
* Generación y publicación de binarios.
* Ejecución de métricas de calidad y visualización los resultados.
* Generación de documentación asociada a un proyecto.

Para mas información ver este excelente [Tutorial](http://www.robertocrespo.net/kaizen/aprende-a-montar-un-entorno-de-integracion-continua-iv-jenkins/)

**Consejo:** Antes de instalar jenkins deberías crear la variable  JENKINS_HOME(Ruta Donde quieras que se instale) en las variable de entrono esto de con el fin de evitarte algunos tropiezos con la configuración de jenkins.

## Instalando Jenkins

PASO 1: [Descargar jenkins](https://jenkins.io/download/).

PASO 2: Ir a la carpeta donde tengas descargado el instalador de jenkins(.war(mejor opción), .msi).

    **Nota:**  Si es .msi solo tienes que darle clic y siguiente siguiente. inicias jenkins en el navegador http://localhost:8080

PASO 3: Ir a la ventana de comando de tu sistema operativo(si es .war).

       -- posicionarse en carpeta donde tienes el .war

       -- Escribir el comando **java -jar jenkins.war**.

       -- En esta ventana cuando se esta realizando el despliegue del jenkins se mostrar una clave que te la pedirá 
jenkins la primera vez que entres en el navegador con la url de jenkins.
	   
PASO 4: Ir al navegador y poner la siguiente url:http://localhost:8080

       -- Digita la clave de contingencia suministrada en el paso anterior.

       -- Al dar clic en el botón continuar te mostrara una ventana donde te pide que instales los plugins por defecto(Recomendado) o seleccionar los plugins deseado. 

       -- Después de esto se cargara una nueva ventana donde te pide que digite las credenciales de acceso como administrador.

PASO 5: Ir a la ventana de login de jenkins y loggearse para empezar.
## Cambiando de Puerto a Jenkins[opcional]
  
  -- Si instalastes jenkins con .war y lo tienes que solo inicie a tu petición por consola deberías usar este comando 
**java -jar jenkins.war --httpPort=9090** al arrancarlo mientras lo usas. eso solo permite cambiar el puerto esa configuracion.
   -- Si queires un cambio permanente debes ir a la ruta donde esta instalado Jenkins y modificar los siguientes archivos 
       **jenkins.xml** propiedad httpPort
      **jenkins.model.JenkinsLocationConfiguration.xml**  nodo jenkinsUrl

**NOTA:** Jenkins se instala por defecto en el puerto 8080, pero este puerto es muy usados por varias aplicaciones así que para evitar conflictos es mejor cambiar el puerto.

## Configurando Jenkins (recomiendo buscar dependiendo de su proyecto)

   -- Para configurar jenkins debes tener en cuenta que tipo de proyecto vas integrar ya que esto puede es dependiendo que necesite el proyecto para su despliegue.

## Cambiando de directorio[opcional]






