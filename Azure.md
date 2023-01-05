Azure
=====
PASOS:

$(System.DefaultWorkingDirectory)

newman run API REST.postman_collection.json --reporters cli,junit --reporter-junit-export junit-report.xml