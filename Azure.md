Azure
=====
PASOS:
1-  Subir a repos la coleccion de postman, la data y el envaironment en caso de necesitarlos
2- Ir a pipelines y crear un nuevo pipelines
3- Seleccionar la opción "Use the classic editor"
4- Seleccionar el team project, el repositorio y presionar el boton continuar
5- Seleccionar el link empity job
6- 
$(System.DefaultWorkingDirectory)

newman run API REST.postman_collection.json --reporters cli,junit --reporter-junit-export junit-report.xml