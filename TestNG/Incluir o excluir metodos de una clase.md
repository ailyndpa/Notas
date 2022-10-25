Incluir o excluir metodos de una clase
========================

**Esto se especifica en el archivo de configuración. Xml.** 
En este caso esta **excluyendo** de la ejecución el metodo de prueba(@Test) que contenga el nombre ploan en la clase day2.

<test name="Test2">
		<classes>
			<class name="Selenium.TestNG.day2">
				<methods>
					<exclude name="ploan"/>
				</methods>
			</class>
			<class name="Selenium.TestNG.day3" />
		</classes>
	</test>