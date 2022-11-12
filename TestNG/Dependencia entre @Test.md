Dependencia entre @Test
========================

Normalmente los test se ejecutan en orden alfabéticos en este caso primero se ejecutaba el metodo SecondTest y luego Zemo, para que se ejecute al revés especificamos en el segundo test que depende del método Zemo y de esta forma se ejecuta el test Zemo y luego SecondTest.

    @Test()
    public void Zemo() {
    	System.out.println("Primera prueba en la clase day1");
    }
	
    	@Test(dependsOnMethods= {"Zemo"})
    	public void SecondTest(String usuario, String Contraseña) {
    		...
    	}