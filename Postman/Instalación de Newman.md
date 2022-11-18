Instalación de Newman
=================

1- Se debe ejecutar “Símbolo del sistema” como administrador y typear**npm install -g newman**
2- Instalar newman-reporter-htmlextra desde la línea de comandos ejecutando **npm install -g newman-reporter-htmlextra**
3-Exportar desde Postman la colletion que se desea ejecutarSeleccionar la opción recomendada y exportar el archivo JSON guardándolo en el directorio de su preferencia.
5- Si hace uso de variables de entorno exportarlas tambien
5-Ejecutar el postman colletion con newman desde la línea de comando **newman run PruebaGoogle.postman_collection.json** Se puede visualizar el resultado de la ejecución en la consola.
6- Para obtener el reporte de los resultados en un HTML se debe ejecutar la siguiente instrucción en la línea de comandos **newman run PruebaGoogle.postman_collection.json -r htmlextra --reporter-htmlextra-title "Informe Prueba Google"** este generará un archivo en formato HTML.