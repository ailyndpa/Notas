Niveles de prueba
========================

**1- Pruebas de componente**: se realizan sobre cada módulo o componente del software que se pueda probar de forma independiente. También se le conoce como prueba unitaria o de módulo. Durante estas pruebas de pueden llevar a cabo pruebas funcionales y pruebas no funcionales, así como pruebas estructurales. Usualmente son responsabilidad del desarrollador porque necesita acceso al código fuente.
*Módulo*: es la unidad mínima funcional de un sistema.

        **Objetivos de las pruebas de componente:**
            ·	Conseguir defectos y fallas en objetos de prueba.
            ·	Reducir el riesgo.
            ·	Construir confianza en la calidad del componente.
            ·	Prevenir defectos que escalen a niveles de prueba más altos.
            
            **Objetos de prueba:**
            ·	Componentes, unidades o módulos.
            ·	Código o estructura de datos.
            ·	Clases.
            ·	Módulos de bases de dato.
            
            **Bases de prueba:**
            ·	Diseño detallado; Modelo de datos; Especificaciones de componentes; Código fuente.
            
            **Errores comunes:**
            ·	Funcionamiento incorrecto.
            ·	Problemas en el flujo de datos.
            ·	Código y lógica incorrecta en el código.
            
**2- Pruebas de integración**: sirven para asegurar que la comunicación, enlaces y datos compartidos entre módulos o con diferentes partes del sistema funcionan correctamente.

    **Niveles de prueba de integración:**
       *Pruebas de integración de componentes(desarrollador)*: prueban las interacciones entre componentes. Se realizan después de las 
        pruebas de componentes. Son parte del proceso de integración continua.
       *Pruebas de integración de sistemas(probador)*: prueban las interacciones entre sistemas, paquetes y servicios. Se realizan después 
        o en paralelo a las pruebas de sistema.
        
           **Objetivos de las pruebas de integración:**
            ·	Conseguir defectos y fallas en la interfaces y módulos.
            ·	Reducir el riesgo.
            ·	Construir confianza.
            ·	Prevenir que defectos escalen.
            
            **Objetos de prueba:**
            ·	Diseño de software; Diagrama de secuencia; Especificaciones de interfaz y protocolo de comunicación; Casos de uso; 
            Arquitectura; Flujo de trabajo; Definiciones de interfaces.
            
            **Bases de prueba:**
            ·	Subsistemas; Bases de datos; Infraestructura; Interfaces; Interfaces de aplicaciones; Microservicios.
            
            **Defectos comunes:**	
            ·	Defectos en los datos; Defectos en las llamadas de interfaz; Incompatibilidad de la interfaz; Fallos en la comunicación 
                de componentes; Fallos en la comunicación entre componentes; Suposiciones incorrectas.
                
**3- Pruebas de sistema**: sirve para verificar que se hayan integrado todos los elementos del sistema y que funciona apropiadamente como un todo. Deben incluir pruebas funcionales y pruebas no funcionales.

	        **Objetivos de las pruebas de sistema**
            ·	Reducir el riesgo.
            ·	Verificar y validar el sistema.
            ·	Validar que el sistema está completo.
            ·	Generar confianza.
            ·	Encontrar defectos.
            ·	Prevenir que defectos escalen.
            
        **Objetos de prueba:**
        ·	Aplicaciones; Hardware; Sistemas bajo pruebas; Configuración.
        
        **Bases de prueba:**
        ·	Especificaciones; Informes de análisis de riesgo; Casos de uso; Épicas e historias de usuario; Modelos de comportamiento; 
            Diagramas de estados; Manuales de sistema de usuario.
            
	    **Defectos comunes:**
        ·	Cálculos incorrectos; Comportamiento incorrecto; Control de datos/flujo de datos incorrecto; Flujo completo de tareas incorrecto; 
        Fallas en la validación; Fallas en la verificación.
        
**4- Pruebas de aceptación**: las pruebas de aceptación se centran en determinar si el sistema es adecuado para su propósito y establecer confianza en el uso del sistema. Suelen ser responsabilidad de los clientes, usuarios del negocio, dueños del producto o los operadores del sistema.
	**Tipos de pruebas de aceptación:**
        	*1- Pruebas de aceptación de usuarios (UAT)*: se centra en validar que el sistema cumple los requisitos de funcionamiento esperado
        	     en un entorno operativo real o simulado. Dentro de sus objetivos principales está: construir confianza, cumplir requisitos, 
        	     realizar procesos de negocio.
    	*2- Pruebas de aceptación operacional (OAT)*: también llamadas como pruebas de aceptación de producción. En estas se valida si 
    	    el sistema cumple con los requisitos de operación y las realizan los usuarios y los administradores de la aplicación. Suelen 
    	    contemplar tipos de pruebas no funcionales (rendimiento; copia de seguridad y restauración; instalación; actualización; 
    	    recuperación ante desastres; tareas de mantenimiento y otras).
    	*3- Pruebas de aceptación contractuales y regulatorias*: el objetivo principal es el haber generado confianza en el cumplimiento 
    	    contractual o reglamentario.
    	*4- Pruebas de aceptación alfa y beta*: suelen ser utilizadas por desarrolladores de un producto de software comercial que desean 
    	    recibir retroalimentación de usuarios, clientes, etc.
    	    
**NOTA**: las pruebas alfa se realizan dentro de las instalaciones donde se desarrolla el código y la ejecutan probadores internos de la organización.
**NOTA**: las pruebas beta permiten encontrar fallas relacionadas a entornos reales donde se ejecutará el sistema; lo ejecutan probadores independientes.

	        **Objetivos de las pruebas de aceptación:**
            ·	Establecer confianza en la calidad del sistema.
            ·	Validar el sistema.
            ·	Verificar el sistema.
            ·	Satisfacer requerimientos legales y reglamentarios.
            
            **Objetos de pruebas:**
            ·	Sistema bajo prueba; Configuración; procesos empresariales; sistemas de recuperación; Procesos operativos y de mantenimiento; 
                formularios; reportes y datos de producción.
                
           **Bases de prueba de aceptación:**
            ·	Procesos de negocio; requisitos usuario/negocio; regulaciones; casos de uso; requisitos del sistema; documentación; 
                requisitos de instalación; Informes de riesgo.
                
	        **Bases de prueba de aceptación OPERATIVA:**
            ·	Procedimientos de respaldo y restauración; Procedimiento de recuperación; Requisitos no funcionales; 
                Documentos de operaciones; Instrucciones; Objetivos de rendimientos; Bases de dato; Regulaciones de seguridad.
                
	        **Defectos comunes:**
            ·	Flujos de trabajo incorrectos; reglas de negocio mal implementadas; regulaciones mal implementadas; fallas no funcionales. 
            
**NOTA**: Cada nivel de prueba está relacionado a su vez con otras actividades dentro del ciclo de vida de desarrollo del software.
**NOTA**: El equipo de probadores es el principal responsable de las pruebas del nivel de aceptación e integración de sistemas.

**Etapa                                     	                Pruebas**
    Desarrollo de componente	                        Pruebas de componente/unitarias
    Desarrollo de interfaces de componentes	    Pruebas de integración
    Desarrollo de interfaces de sistema	            Pruebas de sistema

**NOTA**: los niveles de prueba y tipos de prueba son temas diferentes. Los niveles de prueba se definen por la etapa de desarrollo de     software y los tipos de prueba se relacionan con las técnicas para ejecutar las pruebas en cada nivel. 

**Un tipo de prueba es un grupo de actividades que se centran en un objetivo en particular que podría ser:**
•	Evaluar características funcionales (Integridad, corrección y oportunidad).
•	Evaluar características no funcionales (seguridad, rendimiento, compatibilidad, confiabilidad y eficiencia).
•	Evaluar la estructura/arquitectura del sistema es correcta, completa y como se especifica.
•	Evaluar los efectos de los cambios. Como por ejemplo confirmar que se hayan reparados los defectos.
