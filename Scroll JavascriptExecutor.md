Scroll JavascriptExecutor
========================

**SCROLL** 
JavascriptExecutor js= (JavascriptExecutor)driver;

PASOS:
1-	Abrir: Más herramientas/Herramientas del desarrollador/apartado console.
2-	Con la palabra **window** accedes a los métodos de la ventana en cuestión.
3-	Y con punto y seguido especificas el método a realizar a partir de la ventana.
Ejemplo: window.scroll(0,200)
4-	Con la palabra **document.querySelector** accedes a un elemento especifico de la página pasándole entre paréntesis el localizador, en el siguiente ejemplo se accede al elemento a partir de la clase.
5-	Ejemplo: document.querySelector(".tableFixHead").scrollTop=200

Luego haces uso de estos métodos a partir de JavascriptExcecutor:
**Ejemplo1:** js.executeScript("window.scroll(0,650)");
