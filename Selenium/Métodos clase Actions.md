Métodos clase Actions
========================
	Actions accion= new Actions(driver);
	
**moveByOffset(int xOffset, int yOffset)**: xOffset(desplazamiento horizontal), si es mayor que 0 es hacia la derecha. yOffset(desplazamiento vertical), si es mayor que 0 es 
                                                                        hacia abajo.
                                                                        
**moveToElement(WebElement elemento)**: mueve el cursor hasta el elemento pasado por parametro.

**click(WebElement elemento)**:realiza click sobre el elemento pasado por parametro, si no recibe ningun elemento hace click en donde se encuentre ubicado el cursor.

**doubleClick(WebElement elemento)**:realiza doble click sobre el elemento pasado por parametro, si no recibe ningun elemento hace doble click en donde se encuentre ubicado 
                                                                    el cursor.
                                                                    
 **contextClick(WebElement elemento)** :simula la accion del usuario al realizar click derecho sobre un elemento pasado por parametro; si no recibe ningun elemento hace 
                                                                     click derecho en donde se encuentre ubicado el cursor.
**clickAndHold(WebElement elemento)**: simula la acción de realizar un click sobre un elemento web pulsando sin soltar el click izquierdo.

**release(WebElement elemento)**: simula la accion de soltar el boton izquierdo del raton.

**dragAndDropBy(WebElement elemento, int xOffset, int yOffset)**: simula la accion de arrastrar un elemento web de una posición a otra de la pantalla.

**dragAndDrop(WebElement elemento1, WebElement elemento2)**: simula la accion de arrastrar el elemento1 hasta el elemento2.

**KeyDown(WebElement elemento, Keys theKey)**: simula la accion de mantener pulsada una tecla especifica. Se hace uso del metodo KeyUp para liberar la tecla.
    Ejemplo:
    1- accion.KeyDown(Keys.SHIFT)
    2- accion.KeyDown(WebElement elemento, Keys.SHIFT)
    
**KeyUp(WebElement elemento, Keys theKey)**: libera la tecla seleccionada a partir de KeyDown.
   
**sendKeys(WebElement elemento, String cadena)**: simula la acción de teclear una cadena en un elemento web especificado o donde se encuentre el cursor