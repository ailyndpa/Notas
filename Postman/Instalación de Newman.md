Instalación de Newman
=================

1- Se debe ejecutar “Símbolo del sistema” como administrador y typear**npm install -g newman**
2- Instalar newman-reporter-htmlextra desde la línea de comandos ejecutando **npm install -g newman-reporter-htmlextra**
3-Exportar desde Postman la colletion que se desea ejecutar(Seleccionar la opción recomendada y exportar el archivo JSON guardándolo en el directorio de su preferencia)
4- Si hace uso de variables de entorno exportarlas tambien desde postman.
5-**Ejecutar la colección de postman con newman desde la línea de comando para el caso de no necesitar variables de entorno:**
newman run COLECCIÓN.json
6- **Si precisa variable de entorno sería:** 
newman run COLECCIÓN.json -e ** 
6- Para obtener el reporte de los resultados en un HTML se debe ejecutar la siguiente instrucción en la línea de comandos **newman run PruebaGoogle.postman_collection.json -r htmlextra --reporter-htmlextra-title "Informe Prueba Google"** este generará un archivo en formato HTML.