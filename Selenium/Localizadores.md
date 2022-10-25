Localizadores
========================

**<input type="password" name="password" id="password" minlength="6" >**

**CSS SELECTOR**
•	**Class Name**->tagname.classname->Button.signInBtn->. signInBtn
•	**Id**->tagname#id->input#password
•	**Tagname**-> input[type='password']
•	**tagname[attribute='valor']:nth-child(index)**-> para ir de la etiqueta padre a la hija cuando tiene varias hijas del mismo tagname
•	**parentTagname childTagname**

**XPATH**
•	**//tagname[@attribute='valor']**
•**//input[@type='password']**
•	**//tagname[@attribute='value'][index]**
•	**//parentTagname/childTagname**
•	**//tagname[contains(@atributo,'valor')]** expresión regular
•	**//tagname[@atribute='valor']/childTagname[index]**
•	**//tagname[text()=valor]**->//button[text()='Log Out']

**De padre a hijo, y de hijo a hermano seria:** 
•	**//parentTagname/childTagname[index]/following-sibling::childTagname[index]**->	//header/div/button[1]/following-sibling::button[1]

**De hijo a padre seria:**
•	**//parentTagname/childTagname[index]/parent::parentTagname**->//header/div/button[1]/parent::div

**SELECCIONAR UN ELEMENTO DINAMICO**
•	Un elemento dinámico es un elemento que se muestra a partir de otro. Si queremos acceder a este y este tiene el mismo localizador que el elemento mostrado con anterioridad entonces especificas el xpath entre paréntesis y luego entre corchetes pones el índice del elemento que quieres obtener
**Ejemplo1**: (//a[@value='HYD'])[2]
•	Otra manera sería accediendo del padre al hijo sin especificar index, solo entre padre e hijo en lugar de ir una sola / irían //.
**Ejemplo2**: //div[@id='glsctl00_mainContent_ddl_originStation1_CTNR']//a[@value='BLR']
