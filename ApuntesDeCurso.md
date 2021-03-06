# Apuntes de Curso

Artículo [Los peores sistemas](http://www.nacion.com/opinion/foros/peores-sistemas_0_1534446546.html) de Roberto Sasso

Para el análisis
 1. ¿Está de acuerdo con la afirmación: "El programa no se gasta ni se rompe, simple y sencillamente, está mal escrito."
 2. De acuerdo al artículo, ¿cuáles atributos determinan la calidad (o falta de ella) de un software? ¿cuál es su interpretación de dichos atributos?
 3. ¿Por qué se dice que los sistemas más viejos tienden a ser los peores? ¿Cuál sería una solución a esta problemática?
 4. ¿Está de acuerdo con el "método Singapur" para determinar el tiempo de vida útil de un sistema?
 5. ¿A qué se refiere la afirmación "ellos –al contrario de nosotros– son obsesivos en no desarrollar sistemas internamente..."?

# Definición de calidad

- Grado de excelencia
- Superioridad en comparación con otros
- *ISO8402:* Conjunto de propiedades y características de un producto o servicio que le confieren su aptitud para satisfacer unas necesidades expresas.

# Calidad en el software

- Factores Externos
  - Eficiencia
  - Robustez
  - Portabilidad
  - etc (Mayer)

- Factores Internos
  - Legibilidad de código
  - Testability (Susceptibilidad a ser probado)
  - Mantenibilidad

# Definición de defecto o *pulga*
(Patton)
Un defecto de software ocurre cuando una o más de las siguientes reglas se cumple:
1. El software *no hace* algo que la especificación dice que *debería hacer*
2. El software *hace* algo que la especificación dice que *no debería hacer*
3. El software *hace* algo que la especificación *no menciona*
4. El software *no hace* algo que la especificación no menciona pero que *debería*
5. El software es *difícil de entender, difícil de usar o, según la perspectiva del probador, será considerado como incorrecto por parte del usuario final*

# Aseguramiento de la calidad:
- Esfuerzo **total** para planear, dirigir y controlar los productos y procesos de manera que los resultados sean de calidad
- Concepto más amplio que el de pruebas de software
- En la práctica, para algunas organizaciones QA = pruebas de software

# Costos en la calidad
- Costo de Calidad = Costo de Control + Costo de Fallos en Control
- Costo de Control = Costo de Prevención + Costo de Evaluación
**Costo de Prevención:** esfuerzos para *prevenir* defectos: QA, planeación, entrenamiento, etc.
**Costo de Evaluación** esfuerzos para *detectar* defectos: pruebas, verificación y validación
- Costo de Fallos en Control = Costo de Fallos Internos + Costo de Fallos Externos
**Costo de Fallos Internos**: defectos detectados internamente. Implican *retrabajo*
**Costo de Fallos Externos**: detectados por el cliente o usuario externo: implican costo de servicio, relanzamiento/redistribución, penalizaciones, imagen, etc.

# Costo relativo de solucionar defectos
(Barry Boehm)

| Etapa                  | Costo Relativo |
|------------------------|----------------|
| Requerimientos         | 1x             |
| Diseño                 | 5x             |
| Codificación           | 10x            |
| Pruebas Internas       | 20x            |
| Pruebas de Aceptación  | 50x            |
| Producción             | >150x          |

# Control de la calidad

- En productos tradicionales: inspecciones. ¿El producto/servicio cumple con las especificaciones?

- En el software: pruebas de software.

- (Patton) El objetivo: encontrar defectos (pulgas)
  - lo antes posible
  - .. y asegurarse de que sean corregidos.

- Imposible probar un software completamente
  - muchas entradas posibles
  - muchas salidas posibles
  - muchas rutas dentro del código
  - subjetividad en:
    - interpretación de especificaciones
	- qué es o qué no es una pulga

# Características de las pruebas

- Requieren tiempo y esfuerzo (entre 20% y 50% de los proyectos)

- Requieren habilidades:
  - Técnicas
  - Perseverancia
  - Persuasión
  - Diplomacia

- Se integran durante todo el ciclo de vida del desarrollo

- Originan una profesión disciplinada y de características técnicas

# Requerimientos

- Especificación de producto: acuerdo entre el equipo de desarrollo que define el producto que se crea:
  - ¿Qué es?
  - ¿Cómo se comporta?
  - ¿Qué   hace?
  - ¿Qué no hace?

- Diferentes grados de formalidad
  - acuerdo verbal
  - correos
  - apuntes
  - documentos detallados y estandarizados / herramientas automatizadas

# Roles y Responsabilidades en las Pruebas

## Desarrolladores
  - Pruebas unitarias, requiere conocimiento del código
  - Pruebas de integración, requerimiento conocimiento de requerimientos y de interfaces entre módulos

## Equipo de Pruebas
  - Especializado
  - Conocimiento
    - Técnicas de pruebas
	- Errores más comunes
  - "Visión externa"
  - Roles dentro del equipo de pruebas: Test Engineer, Senior Test Engineer, Test Lead, Test Architect, Test Manager, etc.

## Beneficios de QA
  - Calidad
  - Competitividad
  - Reducir costos y riesgos
  - Incremento de la productividad
  - Retención de clientes / beneficios de imagen


# Terminología

## Defecto vs Falla
  - **Error Humano** puede generar **Defecto**
  - **Defecto** puede generar **Falla**
  - **Falla** es manifestación visible de **Defecto**
  - **Defectos** y **Fallas** se pueden clasificiar
  - Al ocurrir una **Falla** se requiere identificar cuál es el **Defecto**
  - **Defectos** requieren **Corrección**

## Verificación vs. Validación


| Fuente         | Verificación / Inspección                                       | Validación                                     |
|----------------|-----------------------------------------------------|------------------------------------------------|
| Patton y Otros | ¿Sistema cumple con espec. de requerimientos?       | ¿Sistema cumple con expectativas del cliente?  |
| Boehm y Otros  | ¿Estamos construyendo el producto correctamente?    | ¿El producto en construcción es el correcto?   |
|                | Revisiones Estáticas                                | Revisiones Dinámicas                           |
|                | Aplicado al proceso y los componentes en desarrollo | Aplicado al producto final o parciales         |

### CMM / IEEE

#### Verificación:
Evaluar el software para determinar si los productos de una fase satisfacen las condiciones impuestas al inicio de la fase
#### Validación:
Evaluar el software al final del desarrollo para determinar si satisface los requerimientos

## Artículos sobre fracasos de proyectos de software y su relación con los requerimientos y otros factores

*Standish Group's Chaos Report (1995)*
https://www.projectsmart.co.uk/white-papers/chaos-report.pdf
- Pag 6: Excesos en términos de costo y tiempo
- Pag 8. Criterios de éxito
- Pag 9. Factores de fracaso para proyectos fallidos o afectados (challenged)

*Standish Group 2015 Chaos Report*
https://www.infoq.com/articles/standish-chaos-2015
- Gráfico de resulución para todos los proyectos (successful, challenged, failed)
- Resolución en metodologías ágiles vs. cascada
- Factores de éxito

*The Non-Existent Software Crisis: Debunking the Chaos Report*
http://www.drdobbs.com/architecture-and-design/the-non-existent-software-crisis-debunki/240165910
- Números más positivas, estadísticas según varios paradigmas (lean, agile, iterative, ad hoc, traditional)


# Actitudes con respecto a las pruebas de software

## Desarrolladores
- Presión por producir
- Orgullo de "nuestro" trabajo
 -  Lo restante "no es mi culpa"
- Mostrar las bondades de su obra

## Encargados de pruebas
- Presión por encontrar Fallos
 - o por "confirmar" el software
- Poco conocimiento del sistema o de los detalles técnicos

## Soluciones al conflicto
- Trabajo en equipo: distintos roles, mismo objetivo
- Se evalúa al producto, no a la persona
- Voluntad de mejora: personal y del equipo

# Pruebas dinámicas de Caja Blanca (Material Suplementario)

*Escenario:*
- Módulo A de nivel 1  depende de módulo B de nivel 2
- Módulo B depende de módulos E y F de nivel 3
- Se desea probar módulo B

*Necesidad*: Verificar las llamadas que se pueden hacer a B (por parte de A y otros)
- Técnica: uso del Driver
- Definir un conjunto de casos de prueba aceptable

*Necesidad*: Simular el uso que hace B de los módulos E y F
- Técnica: uso de Stubs/Mocks

## Driver
- Simula el uso o invocación del módulo a probar
- Usualmente más sencillo de desarrollar que el stub
- Se desarrolla a la medida o apoyado por herramientas

## Stub
- Simplificado, con respecto al módulo real
- Implica costo de desarrollo
- Si está excesivamente simplificado (ej. devolver siempre los mismos valores) entonces puede afectar la verificar correcta del módulo que lo usa.

*Tanto los Drivers como los Stubs no necesariamente son código para desechar*

#  Estrategias de Integración de un sistema multinivel

## "Big Bang"
- No incremental (sin integraciones parciales)
- Se prueba cada módulo de forma aislada y luego se prueba la combinación de todos los módulos a la vez

*Pros y Contras*
- :) Permite mucho paralelismo en el desarrollo
- :( Requiere mucho desarrollo de stubs y drivers
- :( Difícil detectar orígen del defecto una vez que se hace la integración total
- No recomendable para sistemas grandes

## Bottom-Up
- Comenzar por los módulos que no dependen de ningún otro, Continuar hacia arriba
- Requiere desarrollo de Drivers para pruebas pero no de Stubs
 - Para probar un módulo, todas sus dependencias deben estar probadas previamente
- Permite localizar defectos y una sólida integración parcial
- Puede dificultar la planeación del cronograma y visibilidad del avance

## Top-Down
- Comenzar por el módulo superior y continuar hacia abajo
- Requiere de Stubs, pero no de Drivers
 - Mayor complejidad
- Facilita la visibilidad del avance
- Puede afectar el paralelismo

*En la práctica* se usa un esquema híbrido top-down y bottom-up, según la definición de módulos críticos y la planificación del avance

# Diseño de pruebas

Considerar
- Especificación de requerimientos
- Técnicas de pruebas funcionales (caja negra

## Determinar Conjunto de Casos de Prueba (CCP) según el enfoque de caja negra
- Reducir a clases de equivalencia
- Identificar límites
- Pruebas de estandarizados

Ejemplo 1:

*CP05*: Dada la precondición de que existe el usuario 'usr' con la contraseña 'password', al ejecutar el procedimiento de prueba PP07 con los datos usuario: usr, contraseña: password:
- La autenticación debe ser exitosa (correctitud)
- El usuario debe ser llevado a la pantalla principal (transición correcta de estados)

Ejemplo 2:

*CP06*: Digitar la dirección de la pantalla principal sin haber pasado previamente por la pantalla de autenticación (PP09)
- No se muestra la pantalla principal (correctitud)
- El usuario es llevado a la pantalla de login (y/o se muestra un mensaje de error) (transiciones correctas)

## Depurar el CCP según el enfoque de caja blanca
- Eliminar CPs redundantes
- Determinar CPs faltantes
- CPs que manipulan estado interno para forzar condiciones
- CP adicionales que mejoren la cobertura de código

## Casos de prueba negativos (Test-to-Fail)
- Utilizar el software de una manera para la cual no fue creado

Ejemplos
- Entradas de tipo incorrecto
- Entradas no introducidas
- Entradas fuera de rango o con valores irreales
- Uso no esperado de controles de interfaz de usuario
- Tratar de forzar errores de seguridad

*Resultado del diseño de pruebas:* especificación de casos de prueba y de procedimientos de prueba
- Siguiendo un formato estructurado (Patton cap 18)

# Tipos de pruebas

## Pruebas de especificación
## Pruebas unitarias
## Pruebas de integración
- Top down
- Bototm up

## Pruebas funcionales
Verifica que una parte del sistema, o el sistema completo, realiza las funciones especificadas en el documento de especificación de requerimientos (ERS)

Se prueban:
- Funciones individuales
- Combinaciones o rutas dentro del estado o flujos del sistema (pruebas de estado)

A partir de:
- Requerimientos
- Casos de uso
- Diseño de pruebas

## Pruebas de regresión
Asegurarnos de que un cambio o nueva funcionalidad no ha descompuesto lo que ya funcionaba

## Pruebas de Rendimiento
Verificar que el sistema cumpla criterios de rendimiento/desempeño

Tipos:
- *Pruebas de carga/estrés:* aumentar paulatinamente la carga (usuarios,transacciones,etc) hasta determinar el punto en el que sistema "se rompe ante la carga"
- *Pruebas de estabilidad (soak testing):* determinar si la aplicación puede soportar una carga esperada por un largo de tiempo. Ej: tratar de detectar fugas de memoria
- *Pruebas de volumen/picos:* someter el sistema a una carga alta, pero probable, por cortos periodos de tiempo. Ej: cantidad de peticiones/usuarios concurrentes.

## Pruebas de usabilidad
Verificar facilidad y conveniencia en el uso del software.
- Pueden realizarse de forma temprana por medio de prototipos.

## Pruebas de recuperación
Forzar fallo en el software y verificar que la recuperación se lleve a cabo adecuadamente

## Pruebas de seguridad
Verificar que los mecanismos de protección incorporados al sistema los protejan adecuadamente. "Intentar hackear el sistema"

## Pruebas de confiabilidad
Verificar la confiabilidad del sistema, cuando existen requerimientos específicos al respecto.
*Ejemplo:* "uptime de 99.5%" (solamente 3 horas y 40 minutos puede estar el sistema 'offline' al mes)
- Difícil de verificar
- Se puede *estimar* a partir de datos previos. Ej: tiempo entre fallas de 20 horas y recuperación de falla en 15 minutos

## Pruebas alfa
Llevadas a cabo por el cliente o algún stakeholder en un entorno controlado y observado por los desarrolladores

## Pruebas beta
Llevadas a cabo por usuarios finales en un entorno similar al de producción, sin la presencia constante del desarrollador

## Pruebas de aceptación
Realizadas por el cliente para aceptar un sistema de software según criterios establecidos (en un contrato).
Criterios de aceptación:
- funcionales
- rendimiento
- interfaz/usabilidad/adaptabilidad
- otros

Las pruebas de aceptación pueden originar cambios (considerables) previo al acuerdo de aceptación


# Matriz resumen de tipos de pruebas


Referencia: [Test First](http://www.scaledagileframework.com/test-first/)

|                             | Soporte al Desarrollo | Evaluación de la Solución |
|-----------------------------|-----------------------|---------------------------|
| **De cara al negocio**      | Q2                    | Q3                        |
| **De cara a la tecnología** | Q1                    | Q4                        |

De cara al negocio:
  - Entendibles por el usuario final
  - Descritas formal o informalmente en lenguajes de negocio

De cara a la tecnología:
  - Escritas en lenguajes técnicos / de desarrollo
  - Usadas para validar que el código presente el comportamiento esperado por los desarrolladores

Soporte al desarrollo
  - Evaluar productos internos / código

Evaluación de la solución
  - Evaluar el sistema contra los requerimientos del usuario

## Q1: De cara a la tecnología, soporte al desarrollo
- Pruebas de regresión
- Pruebas de unidad
- Pruebas de integración

## Q2: De cara al negocio, soporte al desarrollo
- Pruebas de especificación
- Pruebas funcionales
- Pruebas de usabilidad tempranas (prototipos)

## Q3: De cara al negocio, evaluación de la solución
- Pruebas de usabilidad sobre el producto
- Pruebas alfa/beta
- Pruebas de aceptación


## Q4: De cara a la tecnología, evaluación de la solución
- Pruebas de rendimiento (estrés, estabilidad, volumen)
- Pruebas de recuperación
- Pruebas de seguridad
- Pruebas de confiabilidad

**Automatización** Usualmente presente  en Q1, Q4 y, en la medida de lo posible Q2

**Pruebas manuales** Usualmente presentes en Q3 y, cuando es necesario, Q2

# Jerarquía de Automatización de Pruebas


| Nivel | Tipos de Pruebas                        | Tipos de Herramientas               | Ejemplos de Herramientas           |
|-------|-----------------------------------------|-------------------------------------|------------------------------------|
|0      | Pruebas manuales                        | Apoyo a las pruebas                 | Wiki                               |
|1      | Pruebas funcionales, UI                 | Herramientas específicas            | Selenium                           |
|2      | Pruebas de API, Integración, Aceptación | Lenguajes cercanos al usuario (DSL) | Fitnesse, herramientas a la medida |
|3      | Pruebas unitarias / de componentes      | Mismo lenguaje de la aplicación     | JUnit                              |

- Conforme se baja en la jerarquía la automatización es menos costosa
- Conforme se sube en la jerarquía la automatización es más costosa

- Conforme se baja en la jerarquía se tiene un mayor retorno sobre la inversión
- Conforme se sube en la jerarquía se tiene un menor retorno sobre la inversión

- Conforme se baja en la jerarquía la automatización es más estable / robusta
- Conforme se sube en la jerarquía la automatización es menos estable / robusta

## ¿Quién automatiza?
Escenario ideal requiere colaboración entre equipo de QA y desarrolladores

## ¿Qué se puede automatizar?

### Pruebas unitarias
No tiene sentido que sean manuales si queremos detectar problemas de regresión

### Pruebas de APIs / Web Services / Lógica de Negocios
Capa inferior a Interfaz de usuario

### Pruebas funcionales desde la UI
- Con lógica de negocios real o stubs
- Empezar por lo más básico

### Pruebas de rendimiento
- Pruebas de carga, estabilidad, volumen, por medio de herramientas especializadas

### Integración contínua, builds y deployment
- Builds/deployment periódicos o disparados con cada cambio efectuado
- Notificaciones automáticas indicando los resultados y los cambios incorporados
  - Equipo de QA no tiene que esperar para probar
  - Desarrolladores reciben retroalimentación temprana de defectos y sugerencias
- Puebas automatizadas incorporadas al proceso de build
  - Balance entre automatización vs. tiempo que toma el build
- Es lo primero que se debe automatizar!

### Otros automatizaciones posibles
- Inspecciones y comparaciones de archivos de salida, tablas de bases de datos, etc.
- Tareas repetitivas
- Generación de código
- Creación o configuración de los datos de los sistemas, scripts de bases de datos, limpiar datos de pruebas previas, etc.

## Estrategias para automatizar

Analizar
 - Requerimientos
 - Factores críticos de calidad del software
 - riesgos

¿Dónde ganamos más?
 - Usualmente pruebas de unidad generan Robustez

¿Dónde "nos duele más"? ¿Dónde es más tedioso el trabajo?

Reconocer el tiempo y esfuerzo requerido

Considerar la jerarquía de automatización de pruebas
 - Usualmente se procede de abajo hacia arriba

Reconocer pruebas como **producto ingenieril**: requieren diseño cuidadoso para:
  - minimizar esfuerzos de mantenimiento
  - minizar duplicaciónn
  - incorporar en control de configuración
  - etc.

Considerar la clasificación y organización de muchas (decenas/centenas/miles) pruebas y de sus resultados
  - visibilidad de pruebas y resultados

## Generación de datos

Evaluar uso de herramientas vs scripts internos

No siempre se requieren datos al nivel de la BD
 - Uso de stubs para sustituir el acceso a nivel de la BD en las pruebas
   - Mejora en tiempos de ejecución de pruebas

En caso de que se requieran pruebas utiizando la BD
 - Escenarios setup/teardown
 - Evaluar uso de BDs "canónicas"
 - Considerar que algunas pruebas requieren escenarios muy similares a los de producción

Migraciones de datos también deben probarse

## Criterios para escoger herramientas

- Identificar requerimientos para las herramientas y tipo de automatización deseada
- Evaluar integración con los componentes y herramientas existentes
- Considerar posibilidad de desarrollo internos
- Considerar experiencia y habilidades en el equipo
- Escoger e integrar una herramienta a la vez
