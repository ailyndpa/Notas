Ejecutar desde distintos SO
========================

**Para ver en que sistema operativo estamos corriendo los test->** System.out.println(System.getProperty("os.name"));
       
    if (System.getProperty("os.name").contains("Windows")) {
			System.setProperty("webdriver.chrome.driver", "./src/resources/chromedriver.exe");
		} else {
			System.setProperty("webdriver.chrome.driver", "./src/resources/chromedriver");
		}