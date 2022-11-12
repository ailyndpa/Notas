Capturar pantalla
========================
**Ejemplo**: 
File foto=((TakesScreenshot)driver).getScreenshotAs(OutputType.FILE);
FileUtils.copyFile(foto, new File("C:/Users/user/git/2-ocutubre/src/resources/lily1.jpeg"));

Si no deja importar el archivo **FileUtils**
1-Dirigirse a la ruta  https://commons.apache.org/proper/commons-io/download_io.cgi
2- Descargar *commons-io-2.11.0-bin.zip*
3- Descomprimir zip
4- Importar librerias en el proyecto
		