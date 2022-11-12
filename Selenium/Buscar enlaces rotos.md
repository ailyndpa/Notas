Buscar enlaces rotos
========================
**El siguiente ejemplo recorre una lista de link y obtiene el href de cada link**
**luego obtiene el código de estado de cada link**

WebElement footer = driver.findElement(By.id("gf-BIG"));
List<WebElement> lista = footer.findElements(By.tagName("a"));

SoftAssert s = new SoftAssert(); **ver en la nota assertions**

for (int i = 0; i < lista.size(); i++) {
	String url = lista.get(i).getAttribute("href");
	
HttpURLConnection conection = (HttpURLConnection) new URL(url).openConnection();
	// conection.setRequestMethod("GET");
	// conection.connect();
	int code = conection.getResponseCode();
	s.assertTrue(code < 400, "El enlace '" + lista.get(i).getText() + "' esta roto");
}
s.assertAll();**ver en la nota assertions**