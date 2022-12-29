Instalación de Newman
=================

1- Se debe ejecutar “Símbolo del sistema” como administrador y typear**npm install -g newman**
2- Instalar newman-reporter-htmlextra desde la línea de comandos ejecutando **npm install -g newman-reporter-htmlextra**
3-Exportar desde Postman la colletion que se desea ejecutar(Seleccionar la opción recomendada y exportar el archivo JSON guardándolo en el directorio de su preferencia)
4- Si hace uso de variables de entorno exportarlas tambien desde postman.
5-**Ejecutar la colección de postman con newman desde la línea de comando para el caso de no necesitar variables de entorno:**
    newman run Movies.postman_collection.json 
6- **Si precisa variable de entorno sería:** 
    newman run Movies.postman_collection.json -e Movie.postman_environment.json
7- **Si hace uso de un archivo json externo sería:**
newman run Movies.postman_collection.json -e Movie.postman_environment.json -d data.json
8-  **Para obtener el reporte de los resultados en un HTML se debe ejecutar la siguiente instrucción en la línea de comandos** 
newman run Movies.postman_collection.json -e Movie.postman_environment.json -d data.json -r htmlextra --reporter-htmlextra-title "E"

**-r htmlextra --reporter-htmlextra-title "Easy POC" --insecure**

C:\Users\adelpino.CHF\AppData\Roaming\npm>

newman run EasyPOC.postman_collection.json -e DEV.postman_environment.json -d E2E.json -r htmlextra --reporter-htmlextra-title "EasyPOC" --insecure
