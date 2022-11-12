Ejecución sin interfaz
========================

ChromeOptions opt = new ChromeOptions();
opt.addArguments(“--headless”);// este es el argumento que deshabilita la interfaz grafica
driver= new ChromeDriver(opt);
