Azure
=====
PASOS:
1-  Ir a Repos y subir 
$(System.DefaultWorkingDirectory)

newman run API REST.postman_collection.json --reporters cli,junit --reporter-junit-export junit-report.xml