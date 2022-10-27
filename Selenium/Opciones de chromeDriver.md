https://chromedriver.chromium.org/capabilities

Opciones de chromeDriver
========================

**Uso de la clase ChromeOptions**
Puedes crear una instancia de ChromeOptions, que tiene métodos convenientes para establecer las capacidades específicas de ChromeDriver. Luego puedes pasar el objeto ChromeOptions al constructor de ChromeDriver:

ChromeOptions options = new ChromeOptions();

 **adiciona una extensión**
options.addExtensions(new File("/path/to/extension.crx"));
ChromeDriver driver = new ChromeDriver(options);

**Trabajando con Proxy**
Proxy proxy = new Proxy();
proxy.setHttpProxy("myhttpproxy:3337");
options.setCapability("proxy", proxy);

**Utilizar un perfil personalizado para indicar a Chrome qué perfil debe utilizar**
Si la ruta no existe, Chrome creará un nuevo perfil en la ubicación especificada
A partir de la url chrome://version puede ver qué perfil está utilizando Chrome.

ChromeOptions options = new ChromeOptions();
options.addArguments("user-data-dir=/path/to/your/custom/profile");

**Iniciar Chrome maximizado**
ChromeOptions options = new ChromeOptions();
options.addArguments("start-maximized");

**Bloquear las ventanas emergentes**
Por defecto, ChromeDriver configura Chrome para permitir las ventanas emergentes. Si quieres bloquear las ventanas emergentes (es decir, restablecer el comportamiento normal de Chrome cuando no está controlado por ChromeDriver), haz lo siguiente:

ChromeOptions options = new ChromeOptions();
options.setExperimentalOption("excludeSwitches", Arrays.asList("disable-popup-blocking"));

**Establecer el directorio de descarga**
No se puede utilizar la carpeta del escritorio como directorio de descarga.
En Windows, utilice "\" como separadores de ruta. El uso de "/" no es fiable en Windows.

ChromeOptions options = new ChromeOptions();
Map<String, Object> prefs = new HashMap<String, Object>();
prefs.put("download.default_directory", "/directory/path");
options.setExperimentalOption("prefs", prefs);