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
- Esfuerzo **total** para plantear, dirigir y controlar los productos y procesos de manera que los resultados sean de calidad
- Concepto más amplio que el de pruebas de software
- En la práctica, para algunas generaciones QA = pruebas de software

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



  
