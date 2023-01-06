Azure
=====
PASOS:
1-  Subir al repos la coleccion de postman, la data y el environment en caso de necesitarlos
2- Ir a pipelines y crear un nuevo pipelines
3- Seleccionar la opción "Use the classic editor"
4- Seleccionar el team project, el repositorio y presionar el boton continuar
5- Seleccionar el link empty job
6- Seleccionar el icono + al lado de Agent job 1
7- Poner en el campo de busqueda Command line y adicionarlo
8- Editar el comando adicionado:
    *Se le asigna un nombre descriptivo: en este caso Instalar dependencias
    *En script adicionar: npm install -g newman newman-reporter-html newman-reporter-htmlextra
    *En Advenced Adicionar en working directory: $(System.DefaultWorkingDirectory)
9- Repetir paso 6 y 7
10- Editar el comando adicionado:
    *Asignarle un nombre descriptivo
    * En script adicionar **uno de los siguientes ejemplo**, ambos hacer lo mismo: 
            * newman run api.postman_collection.json -d data.json --reporters cli,junit,htmlextra --reporter-junit-export junit-report.xml --reporter-htmlextra-export report.html
            * newman run api.postman_collection.json --iteration-data data.json --reporters cli,junit,htmlextra --reporter-junit-export junit-report.xml --reporter-htmlextra-export report.html
            *PARA ADIONARLE TITULO AL REPORTE SERIA:*
            *newman run api.postman_collection.json -d data.json --reporters cli,junit,htmlextra --reporter-junit-export junit-report.xml --reporter-htmlextra-title "Ejemplo API" --reporter-htmlextra-export report.html
    *En Advenced Adicionar en working directory: $(System.DefaultWorkingDirectory)
11- Repetir paso 6
12- Poner en el campo de busqueda **Publish Test Results**  y adicionarlo
13-Asignarle un nombre. Poner en el campo Test results files => junit-report.xml
14- Especificar en el campo Search folder: $(System.DefaultWorkingDirectory)
15- Repetir paso 6
16- Poner en el campo de busqueda **Publish Html Report**
17-Especificar en el campo **HTML file Directory** => $(System.DefaultWorkingDirectory)/report.html
15- Seleccionar boton Save & requeue/Save & requeue
16- Especificar en Agent Specification: windows-latest y seleccionar boton save and run
17- Seleccionas el job y esperas a que termine la ejecucion
18- Dirigirse a publish test result y en la linea de comandos que se abre se muestran todos los resultados de las pruebas publicados. A partir de la etiqueta: Published Test Run : ...



$(System.DefaultWorkingDirectory)
newman run API REST.postman_collection.json --reporters cli,junit --reporter-junit-export junit-report.xml