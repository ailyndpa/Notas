Actividades de prueba y sus respectivas tareas: 
=================================

**1- Planificación de las pruebas**: se debe asegurar la comprensión de las expectativas del usuario y otros implicados, cuáles son sus metas y definir los objetivos y los riesgos que las pruebas deberán considerar, así como la estrategia a seguir para cumplir dichos objetivos tomando en cuenta las restricciones que puede haber.
	Nota: La planificación de las pruebas garantiza que el nivel de detalles en los procedimientos de prueba sea apropiado para la ejecución de pruebas.
 
    **Actividades de la planificación de pruebas:**
    ·	Determinar el alcance, objetivos, riesgos y enfoque de pruebas.
    ·	Integrar y coordinar las actividades de prueba.
    ·	Tomar decisiones sobre que se va a probar, quien lo va a probar y como lo va a probar.
    ·	Establecer calendario de prueba.
    ·	Determinar como medir el avance de la prueba.
    ·	Establecer el presupuesto.
    ·	Determinar el nivel de detalle.

**2- Monitoreo y control de las pruebas**: es un proceso que sigue el progreso del plan para establecer acciones correctivas en caso de ser necesarias.

**3- Análisis**: ¿Qué se debe probar con los recursos disponibles? se debe analizar la base de prueba para ver qué características se pueden probar y transformarlas en condiciones de pruebas.

    **Actividades principales del análisis de prueba:**
    ·	Analizar las bases de prueba: especificaciones de requisitos, información de 
        diseño e implementación, implementación del componente o sistema, informes de análisis de riesgo.
    ·	Evaluar la base de prueba para identificar defectos.
    ·	Identificación de las prestaciones que se probaran.
    ·	Definir y priorizar las condiciones de prueba.
    ·	Garantizar la trazabilidad bidireccional entre la base de prueba y las condiciones de 
        pruebas asociadas.
        
  	**4- Diseño**: ¿Cómo se debe probar? Durante esta actividad las condiciones de prueba se transforman en escenarios también llamado caso de prueba de alto nivel. Un diseño de pruebas es la especificación de los casos de pruebas requeridos para probar una característica.
  	
  	**Ejemplo:**
  	Paso		Actividad		                                                            Resultado esperado
	1		    Ingresar en el sistema satelital con un usuario válido		El sistema permite la entrada
		
		**Actividades principales del diseño de prueba:**
    ·	Diseñar y priorizar casos y conjuntos de prueba.
    ·	Identificar los datos de prueba necesarios.
    ·	Diseñar el entorno de prueba e identificar la infraestructura y herramientas necesarias.
    ·	Capturar la trazabilidad bidireccional entre las bases de prueba, condiciones de prueba y
     casos de prueba.

**5- Implementación**: ¿Está todo listo para ejecutar las pruebas? aquí se crean o completan los productos de prueba necesarios para la ejecución de la prueba, incluyendo la creación de una secuencia de casos de prueba para convertirlos en procedimientos de prueba.
    
    **Actividades principales de la implementación de las pruebas:**
    ·	Desarrollar y priorizar procedimientos de prueba, y potencialmente crear script 
      de pruebas automatizados. Los procedimientos de prueba son una secuencia de 
      acciones para la ejecución de las pruebas, conocidos como scripts de prueba.
    ·	Crear suite o juegos de prueba a partir de los procedimientos de prueba.
    ·	Organizar los juegos de prueba dentro de un cronograma de ejecución.
    ·	Creación del entorno de prueba (incluye arneses de prueba, virtualización de servicios,
      simuladores y otros elementos de infraestructura y verificar que se haya configurado 
      todo lo necesario correctamente).
    ·	Preparación de datos de prueba.
    ·	Verificación y actualización de la trazabilidad entre las bases de prueba, condiciones 
      de prueba, casos de prueba, procedimientos de prueba y juegos de prueba.
    
    **Ejemplos de arneses de prueba:** marcos de trabajo o frameworks de automatización de prueba 
      (selenium, cypress, más).

**6- Ejecución**

    **Actividades principales de la ejecución de las pruebas:**
    ·	Registrar identificadores, versiones de objetos y herramientas.
    ·	Ejecutar las pruebas ya sea manual o con herramientas de ejecución de pruebas.
    ·	Comparar resultados obtenidos con resultados esperados.
    ·	Analizar anomalías y establecer causas probables, por ejemplo, falsos positivos. 
    ·	Informar sobre defectos en función de las fallas observadas.
    ·	Registrar resultados de la ejecución de las pruebas.
    ·	Repetir pruebas para verificar que defectos encontrados fueron corregidos.
    ·	Verificar trazabilidad entre las bases de prueba, condiciones de prueba, 
      casos de prueba, procedimientos de prueba y resultados de prueba.
      
**7- Compleción**: estas actividades suceden cuando finaliza la iteración de un proyecto ágil, se completa un nivel de prueba o un mantenimiento.
	
    **Actividades principales de la compleción de pruebas:**
    **1- Evaluación de criterios de salida e informes**. En esta actividad se evalúa si los resultados 
      de las pruebas cumplen con los requisitos establecidos,	recordando que cada nivel de 
      prueba tiene una serie de objetivos definidos. Esta actividad consta de una serie de
      tareas principales como: comprobar los registros de prueba con los criterios de salida
      previstos en la planificación de las pruebas, evaluar si se requieren más pruebas o si
      deberían modificarse los criterios de salida establecidos y elaborar un resumen de las
      pruebas para las partes interesadas.
    **2- Actividades de cierre de prueba** consisten en un subconjunto de tareas principales como: 
      comprobar productos entregados, cerrar informes de incidencias o aportar modificaciones
      a aquellos que siguen abiertos, documentar la aceptación del sistema, finalizar y archivar
      los productos del soporte de prueba, el entorno de prueba y la infraestructura de pruebas
      para su posterior reutilización; entregar productos a mantenimiento, analizar lecciones
      aprendidas para determinar los cambios necesarios en futuras versiones del proyecto.
      
**NOTA**: El desarrollo ágil implica pequeñas iteraciones de diseño de software, construir y probar suceden de forma continua, las actividades de prueba también suceden de forma iterativa y continua.

