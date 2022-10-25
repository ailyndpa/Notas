DATA PROVIDER
========================

**@DataProvider**: permite asignar múltiples condiciones a una prueba, devolviendo un objeto que contiene en si las condiciones. 
    Object [][] data= new Object [ cant. de condiciones][cant. de columnas de cada condicion]

**El objeto que devuelve este método está formado por 2 condiciones con dos valores cada una.**
@DataProvider
	public Object[][] getData(){
		Object [][] data= new Object[2][2];
		data[0][0]="user1";
		data[0][1]="pass1";
		data[1][0]="user2";
		data[1][1]="pass2";
		return data;
	}
	
	
   @Test(dataProvider="getData")
	public void SecondTest(String usuario, String Contraseña) {
		System.out.println("1.0" + usuario);
		System.out.println("1.1" + Contraseña);
	}