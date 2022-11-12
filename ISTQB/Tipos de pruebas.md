Tipos de pruebas
========================

**Dinámica**: ejecutar el software para revisar resultados.
**Estáticas**: revisión de documentos, requerimientos y código fuente. Se basa en la revisión manual o mediante 
                        herramientas automatizadas de los productos de trabajo, incluido el código fuente sin ejecutar.
                        
NOTA: el análisis estático es parte de las pruebas estáticas y es cargo de los desarrolladores.
NOTA: el análisis estático no puede conseguir si el valor almacenado en una variable es correcto, eso se realiza en tiempo de ejecución.

**Técnicas de pruebas estáticas:**
•	Código fuente; documentos; modelos de diseño; especificaciones funcionales y especificaciones de requisitos.

**Las herramientas de análisis estático muestran:** 
•	Profundidad de anidamiento; complejidad ciclomática; estándares de codificación; flujo de control; relaciones de datos; números de rutas entre líneas de código. 

**PRODUCTOS DE TRABAJO EXAMINADOS EN PRUEBAS ESTÁTICAS**
•	Especificaciones de negocio, funcionalidades y de seguridad.
•	Épicas, historias de usuario y criterios de aceptación.
•	Especificaciones de arquitectura y diseño.
•	Código fuente.
•	Productos de prueba.
•	Páginas web.
•	Contratos, planes de proyecto, calendarios y presupuestos.
•	Modelos.

**VENTAJAS DE LAS PRUEBAS ESTÁTICAS**
•	Identifica defectos propios de la técnica (como puede ser incumplimiento de estándares en la codificación) 
•	Identifica defectos en el diseño y la codificación.
•	Incrementa la productividad del desarrollo.
•	Reduce el costo y mantenimiento de desarrollo.
•	Se reduce el costo y tiempo de prueba.
•	Reduce coste total de la calidad.
•	Mejora la comunicación del equipo.
•	Identifica defectos de mantenibilidad (por ejemplo, mala reutilización de los componentes, código difícil de analizar y modificar sin introducir nuevos defectos, etc.)
NOTA: las pruebas estáticas identifican defectos y las pruebas dinámicas identifican fallas.
NOTA: la prueba estática detecta defectos difíciles de alcanzar cuando se ejecuta el software.
NOTA: las pruebas estáticas se enfocan en la calidad interna de los productos de trabajo y las pruebas dinámicas en el comportamiento del software.

**DEFECTOS TÍPICOS EN PRUEBAS ESTÁTICAS**
•	Defectos en requisitos.
•	Defectos en diseño.
        **Acoplamiento**: se refiere a que cada módulo o funcionalidad conoce poco o nada de los otros módulos o funciones.
        **Cohesión**: hace referencia a que las funciones de un módulo guardan relación entre ellas y mantienen un único enfoque.
•	Defecto de codificación.
•	Desviaciones de estándares.
•	Especificaciones de interfaz incorrecta.
•	Vulnerabilidades de seguridad.
•	Trazabilidad o cobertura de la base de pruebas.

**Actividades:**
-Planificación
-Análisis
-Diseño
-Implementación y ejecución
-Reporte
