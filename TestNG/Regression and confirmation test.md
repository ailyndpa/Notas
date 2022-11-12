Regression test y Confirmation
========================

1-Se crea un archivo TestNG.xml y se configura de forma tal que se corran los test que contengan el grupo especificado, en este caso Regressión, pero puede ser Confirmation.

<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE suite SYSTEM "https://testng.org/testng-1.0.dtd">
<suite name="Regression">
	<groups>
		<run>
			<include name="**Regression**"/>
		</run>
	</groups>
	<test name="RegressionTest">
		<classes>
			<class name="Selenium.TestNG.day1"/>
			<class name="Selenium.TestNG.day2"/>
			<class name="Selenium.TestNG.day3"/>
		</classes>
	</test>
</suite>


      @Test(groups= {"Regression"})
	    public void ploan2(){
		    System.out.println("Segunda prueba de la clase day2");
	    }