Azure
=====
PASOS:
1-  Subir a repos la coleccion de postman, la data y el envaironment en caso de necesitarlos
2- Ir a pipelines y crear un nuevo pipelines
3- Seleccionar la opción "Use the classic editor"
4- Seleccionar el team project, el repositorio y presionar el boton continuar
5- Seleccionar el link empty job
6- Seleccionar el icono + al lado de Agent job 1
7- Poner en el campo de busqueda Command line y adicionarlo
8- Editar el comando adicionado:
    *Se le asigna un nombre descriptivo
    *En script adicionar: npm install -g newman
    *En Advenced Adicionar en working directory: $(System.DefaultWorkingDirectory)
9- Repetir paso 6 y 7
10- Editar el comando adicionado:
    *Asignarle un nombre descriptivo
    * En script adicionar: newman run apiRest.postman_collection.json -d data.json --reporters cli,junit --reporter-junit-export junit-report.xml
    *En Advenced Adicionar en working directory: $(System.DefaultWorkingDirectory)

$(System.DefaultWorkingDirectory)

newman run API REST.postman_collection.json --reporters cli,junit --reporter-junit-export junit-report.xml