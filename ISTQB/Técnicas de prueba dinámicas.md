Técnicas de prueba dinámicas
========================

**1.	Caja negra:** también conocidas como técnicas basadas en recuadro negro, pruebas basadas en especificaciones o pruebas de entrada salida.

**CARACTERISTICAS COMUNES DE TECNICAS DE CAJA NEGRA:**
    •	Las condiciones, casos y datos de prueba se deducen de una base de pruebas.
    •	Los casos de prueba se utilizan para detectar diferencias entre los requisitos y su implementación.
    •   La cobertura se mide en función de elementos probados y la técnica aplicada.
    
**TÉCNICAS DE CAJA NEGRA**
•	*Partición de clases de equivalencia*: requiere que solo necesitemos probar una condición de cada partición; por ejemplo: tenemos dos particiones asociadas a la edad (mayores y menores)
Cobertura= (#particiones probadas) / (#particiones identificadas) =1

•	*Análisis de valores fronteras o valores limites*: es una extensión de la partición de clases de equivalencia donde se toman en cuenta solo los valores de cada extremo. Existe la técnica de dos y tres puntos 
Cobertura = (#fronteras probadas) / (#fronteras identificadas) =1

•	*Prueba de tabla de decisión*: ayudan a la selección eficiente de casos de prueba. Identifican entradas o condiciones; identifican acciones o salidas; identificar combinaciones. Se eleva 2 a la cantidad de condiciones y da como resultado la cantidad de combinaciones posibles.
Cobertura = (#condiciones probadas) / (#total de condiciones) =1

**Por ejemplo**: si se tienen 4 condiciones, habría 16 combinaciones posibles y la tabla sería de la siguiente manera:
Primero dividimos 16/2=8, que serían 8 verdaderas y 8 falsas
Luego ese valor lo dividimos entre dos 8/2=4 Y ASI SUCESIVAMENTE hasta completar la tabla.

Condición 1	V	V	V	V	V	V	V	V	F	F	F	F	F	F	F	F
Condición 2	V	V	V	V	F	F	F	F	V	V	V	V	F	F	F	F
Condición 3	V	V	F	F	V	V	F	F	V	V	F	F	V	V	F	F
Condición 4	V	F	V	F	V	F	V	F	V	F	V	F	V	F	V	F
Salidas	        V	F	F	F	F	F	F	F	F	F	F	F	F	F	F	F

•	*Prueba de transición de estado*: El sistema o proceso se maneja dentro de un número ilimitado de estados, y cada transición de un estado a otro se rigen por las reglas de la máquina. 
Cobertura = (#transiciones probadas) / (#transiciones identificadas) =1

•	*Pruebas de caso de uso*: se definen en base a lo que hace y ve el autor en lugar de las entradas y salidas del sistema.
Cobertura = (#comportamientos probados) / (#comportamientos identificados) =1

**2.	Caja blanca:** conocida como técnicas estructurales o basadas en la estructura. Estas se basan en la estructura interna del código del software y se pueden utilizar en todos los niveles de prueba.

NOTA: las pruebas de caja blanca usan conocimiento explícito del funcionamiento interno del objeto bajo prueba para seleccionar la data de prueba. Además, usan conocimiento específico del código fuente para examinar las salidas y asumen que el probador conoce la lógica del programa.
**TÉCNICAS DE PRUEBA DE CAJA BLANCA**
*·Cobertura de sentencia*: vamos a suponer que cada línea de código es una sentencia para este ejemplo.
    1.	LEER A
    2.	LEER B
    3.	C=A+B
    4.	SI C>10 ENTONCES 
    5.	IMPRIMIR C
    6. FIN SI
Cobertura de sentencia= (# de sentencias ejecutadas) / (# total de sentencias ejecutables) =1
Conjunto de prueba: A=5; B=6
Cobertura=6/6=1=100% de cobertura

*Cobertura de decisión*: son aquellas en las que interviene alguna condición a cumplir, por ejemplo: if, while, for, swite, etc.
Cobertura de decisión: (#resultados de decisión ejecutados) / (# total resultados de decisión)

NOTA: Una cobertura de decisión del 100% garantiza una cobertura de sentencia del 100% pero no al revés.

El conjunto de prueba del ejemplo anterior garantiza un 100% de cobertura de sentencia, sin embargo, para garantizar un 100% de cobertura de decisión debe incluir el caso de prueba donde C resulte en un valor inferior o igual a 10, por ejemplo: A=5, B= 5

**ELEMENTOS PRINCIPALES**
·	Análisis de la arquitectura; diseño detallado; estructura interna (código fuente)

**CARACTERISTICAS COMUNES DE TECNICAS DE CAJA BLANCA:**
    ·	Las condiciones, casos y datos de prueba se deducen de una base de pruebas.
    ·   La cobertura se mide en base a los elementos probados dentro de una estructura seleccionada
    
**3.	Basada en la experiencia**: este tipo de técnicas está basada en el conocimiento, la experiencia, la imaginación y la intuición de una persona; y dependiendo del enfoque y la experiencia del probador pueden lograr grados muy diferentes de cobertura y efectividad.

**CARACTERISTICAS COMUNES DE TECNICAS BASADA EN LA EXPERIENCIA:**
    ·	Las condiciones, casos y datos de prueba se deducen de una base de pruebas.
    ·   El conocimiento y experiencia incluye el uso esperado del software, su entorno, los posibles defectos y la distribución de dichos defectos. 
    
**TÉCNICAS DE PRUEBA BASADA EN LA EXPERIENCIA**
    ·	*Predicción de errores*: es anticipar la ocurrencia de defectos o fallas basándose en la experiencia del probador con respecto 
        al funcionamiento de la aplicación en el pasado.
    ·	*Pruebas exploratorias*: consisten en explorar, conocer el software, que hace, que no hace, que funciona y que no. 
        El probador está constantemente viendo que probar a continuación en el periodo de tiempo que tiene que generalmente esta entre 
        una o dos horas.
    ·	*Pruebas Basadas en listas de comprobación*: es un conjunto de preguntas basadas en defectos potenciales que pueden predecir en cuales áreas un sistema presenta debilidades basándose en la experiencia, el conocimiento y la compresión de lo que es importante para el usuario.
