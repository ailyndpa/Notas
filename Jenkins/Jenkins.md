Jenkins
========================

**Paso 1**: Descargue el archivo Jenkins.war y colóquelo en la ruta deseada.

**Paso 2**: Abra el símbolo del sistema y navegue hasta la carpeta que contiene el archivo war.

**Paso 3**: Introduzca el comando java -jar Jenkins.war. Esto iniciará el servidor Jenkins.

**Paso 4**: Jenkins suele iniciarse en el puerto 8080 por defecto. En caso de que el puerto esté siendo utilizado por cualquier otro servicio, se puede definir un puerto alternativo utilizando el siguiente comando: java -jar jenkins.war --httpPort=8081

**Paso 5**: Inicie su navegador y navegue hasta el localhost. Por defecto, el número de puerto sería 8080. En mi caso, he definido el puerto como 8081 y por lo tanto utilizar ese puerto al navegar a la localhost.
Ahora se lanzará la página de configuración de Jenkins, que se utiliza para crear la cuenta de administrador para Jenkins.

**Paso 6**: Introduzca la contraseña secreta que fue generada y mostrada en la consola anteriormente en la página de configuración y haga clic en Continuar.

**Paso 7**: Después de introducir la contraseña secreta, se le pedirá que instale los plugins.

**Paso 8**:Seleccionar "Instalar plugins sugeridos", que instalaría una lista de plugins de uso común. Pero si conoce los plugins en función de los requisitos, puede seleccionar la opción de plugins a instalar y hacer clic en los plugins necesarios.

Ahora los plugins serán descargados e instalados.

**Paso 9:** Una vez que los plugins se instalen con éxito, se le pedirá que cree una cuenta de administrador proporcionando un nombre de usuario, una contraseña y una dirección de correo electrónico. Una vez creado el perfil de administrador, se le dirigirá al panel de control de Jenkins.