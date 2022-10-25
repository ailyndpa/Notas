Iterar en pestañas 
========================
**EJEMPLO CON LA CLASE ITERATOR:**
Set<String> windows= driver.getWindowHandles();
	Iterator<String> it= windows.iterator();
	
String parent= it.next();
String child=it.next();
driver.switchTo().window(child);
String [] usuario= driver.findElement(By.linkText("mentor@rahulshettyacademy.com")).getText();
driver.switchTo().window(parent);
driver.findElement(By.id("username")).sendKeys(usuario);

Si desea **iterar** por las pestañas se hace uso del **While**
    While(it.hasNext()){
        codigo
    }
    
 **EJEMPLO CON JavascritpExecutor**
 JavascriptExcecutor js= (javascriptExecutor)driver;
String pag= "window.open('http://www.google.com')";
js.executeScript(pag);
tabs= new ArrayList<String>(driver.getWindowHandles());
driver.switchTo.window(tabs.get(1));// esto cambia al tab 1 (google)
