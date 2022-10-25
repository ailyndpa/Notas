Clase listeners
========================

A partir de esta clase( .java) se puede especificar que hacer si un test falla o es satisfactorio. Por supuesto esta clase se adiciona al archivo testng.xml

public class listeners implements ITestListener {

	@Override
	public void onTestSuccess(ITestResult result) {
		System.out.println("SUCCESS");
	}
	@Override
	public void onTestFailure(ITestResult result) {
		System.out.println("FAILURE");
	}
}

**Archivo.xml**
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE suite SYSTEM "https://testng.org/testng-1.0.dtd">
<suite name="Suite">
	<listeners>
		<listener class-name="Selenium.TestNG.listeners"/>
	</listeners>
	<test name="Test1">
		<classes>
			<class name="Selenium.TestNG.day1" />
			<class name="Selenium.TestNG.day2" />
			<class name="Selenium.TestNG.day3" />
		</classes>
	</test>
</suite>
