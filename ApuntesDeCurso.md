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




  
