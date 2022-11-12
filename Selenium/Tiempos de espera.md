Tiempos de espera
========================
**La espera implícita hace que la ejecución de la prueba sea lenta, mientras que 	la espera explícita no afecta a la velocidad de ejecución.**

**pageLoadTimeout()**: define el tiempo maximo de espera para la carga completa de la pagina web.

**Thread.sleep**: este método detendrá la ejecución del script durante el tiempo especificado, independientemente de si el elemento se encuentra o no en la página web. 
                                    Si este  elemento es encontradado antes del tiempo especificado el script seguirá esperando a que transcurra el tiempo de duración, aumentando así el 
                                    tiempo de ejecución del script. Si necesitaras encontrar varios elementos y el tiempo de carga es dinamico, tendrias tu script lleno de Thread.sleep y esto
                                    es un mal uso, para ello se recomienda el **implicit wait.**
	                                **Thread.sleep(3000);**
	                                
**Implicit wait**:  sólo comprueba la presencia de elementos en la página web para un tiempo determinado. Trabajará en todos los elementos de la secuencia de comandos 
                              una vez haya sido especificada. A diferencia de Thread.sleep(), no espera la duración completa del tiempo. En caso de que encuentre el elemento antes de 
                              la  duración especificada, pasa a la siguiente línea de ejecución de código, reduciendo así el tiempo de ejecución del script.
	                            **driver.manage().timeouts().implicitlyWait(Duration.ofSeconds(3));**
	                            
**Explicit wait**: es un concepto de espera dinámica que espera dinámicamente por condiciones específicas.
                            **WebDriverWait wait=new WebDriverWait(driver,20);**
                            **WebElement element=wait.until(ExpectedConditions.visibilityOfElementLocated(By.xpath("ur xpath here")));**
                            
**CONDICIONES ESPERADAS**
	1- visibilityOfElementLocated(): Verifica si el elemento dado está presente o no
	2- alertIsPresent(): Verifica si la alerta está presente o no.
	3- elementToBeClickable(): Verifica si el elemento dado está presente/se puede 	hacer clic en la pantalla
	4- textToBePresentInElement(): Verifica si el elemento dado tiene el texto 	requerido o  no
	5- titlels(): Verifica la condición de espera de una página que tiene un título dado
	
**Fluent Wait**: Cada instancia de FluentWait define la cantidad máxima de tiempo para esperar una condición, así como la frecuencia con 
                           la que se comprueba la condición. Además, el usuario puede configurar la espera para ignorar tipos específicos de 
                           excepciones mientras se espera, como NoSuchElementExceptions cuando se busca un elemento en la página.
                        	**Wait<WebDriver> wait = new FluentWait<WebDriver>(driver)**
                        	**.withTimeout(Duration.ofSeconds(30))**
                        	**.pollingEvery(Duration.ofSeconds(5))**
                        	**.ignoring(NoSuchElementException.class);**
                        	
**wait.until(new Function<WebDriver, WebElement>() {**
        **public WebElement apply(WebDriver driver) {**
             **if(elemento.isDisplayed()) {**
               **return elemento;**
             **}**	
             **else {**
               **return null;**
             **}**    	 
        **}**
 **});**
