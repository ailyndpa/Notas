Abrir varias pestañas a partir de links
==========================
List<WebElement> lista= driver.findElements(By. tagName("a");
    for(int i=0; i< lista.size(); i++ ){
        lista.get(i).sendKeys(Keys.chord(Keys.CONTROL, Keys.ENTER));
    }

