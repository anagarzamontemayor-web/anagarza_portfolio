#  Aprendizaje estadístico-automático
En la actualidad, los niveles de obesidad en la población ha trascendido a ser una problemática de salud pública de relevancia, particularmente en países de Latinoamérica. Ante esta situación, investigadores de la Universidad de la Costa en Colombia analizaron información de individuos provenientes de Colombia, Perú y México con el objetivo de estudiar y evaluar factores relacionados con dichos niveles.

Asimismo, se hará uso de la base de datos perteneciente a la *UCI Machine Learning Repository* bajo el nombre ***“A1.1 Obesidad.csv”***, presentándose variables demográficas de hábitos y de salud, donde, a partir del índice de masa corporal, se determinará una variable
categórica que describe el nivel de obesidad de cada individuo.

La base de datos cuenta con la siguiente información:
- `Sexo` indica *Female* para mujeres y *Male* para hombres.
- `Edad` indica la edad de los individuos en un rango de 14 a 61 años.
- `Estatura` indica la estatura de los individuos en *Metros*.
- `Peso` indica el peso de los individuos en *Kilogramos*.
- `FamiliarConSobrepeso` indica si el individuo tiene un pariente con sobrepeso: *yes* indica que si hay parientes con dicha condición y *no* indica lo contrario.
- `ComeMuchasCalorias` indica los hábitos de consumo de calorías del individuo: *si* indica que su ingesta de calorías es alta y *no* indica lo contrario.
- `ComeVegetales` indica los hábitos de consumo de vegetales del individuo: *si* indica que los vegetales forman parte de su dieta y *no* indica lo contrario.
- `Fumador` indica sus hábitos de consumo de cigarros del individuo: *si* indica que es fumador  y *no* indica lo contrario.
- `ConsumoDeAgua` indica la cantidad de agua consumida por el individuo en *Litros*.
- `NivelDeObesidad` indica la categoría de peso del individuo:
  1. Insufficient_Weight* indica que su peso se encuentra bajo el umbral clínico de normalidad.
  2.  *Normal_Weight* indica que su peso se encuentra dentro de la normalidad.
  3.  *Overweight_Level I* indica que el peso está de manera moderada por encima del rango normal.
  4.   Overweight_Level II* indica que el exceso de peso es más notable.
  5. *Obesity_Type_I* indica que el peso ha superado el umbral clínico de obesidad.
  6. *Obesity_Type_II* indica que la obesidad es más severa y riesgoso para la salud.
  7. *Obesity_Type_III* indica que la obesidad es grave y es necesario tomar acciones en la brevedad.
 
  Este proyecto incluye los siguientes documentos:

- [Reporte en formato ipynb](A1_1_Analisis_exploratorio_de_Obesidad.ipynb)
- [Reporte en formato html](A1_1_Analisis_exploratorio_de_Obesidad.html)
- [Base de datos](Obesidad.csv)

#  Regresión lineal
  
Dede 2012 el World Happiness Report (WHR) ha propuesto una metodología para estimar un concepto tan complejo y dificil de medir, la felicidad. De manera que, a partir de estos estudios, factores económicos, sociales y de salud han sido analizados con posibles explicaciones basandose en las diferencias presentes entre países. Entre ellos, el producto interno bruto (GDP) y otros elementos relevantes. Para ello, el Centro de Investigación del Bienestar de la Universidad de Oxford, en colaboración con Gallup, la SDSN y un consejo editorial independiente clasifica anualmente a 146 países la evaluación del promedio de la calidad de vida de la población. Pidiendo a los encuestados calificar su vida actual en una escala del 0 al 10, donde 10 representa la mejor vida posible y 0 la peor.

Asimismo, se hará uso de la base de datos bajo el nombre “A1.2 Felicidad y GDP.csv”, presentándose información sobre el nivel de felicidad reportado en 2022 y el GDP correspondiente a 2020 para distintos países. De esta forma, se llevará a cabo un análisis de la relación entre la felicidad y variables económicas y sociales mediante modelos de regresión lineal, explorando tanto un enfoque de regresión lineal simple como uno de regresión lineal múltiple. 

Cabe destacar que, al trabajar con variables económicas, se considerarán transformaciones adecuadas para así trabajar con variables lineales. Analizando así, la conveniencia de utilizar o no una transformación.
 

El conjunto de datos disponible cuenta con tres variables principales:

- `País` variable categórica que indica el país representante.
- `Felicidad` variable cuantitativa que indica la perceoición de felicidad en una escala de 0-10.
- `GDP` variable cuantitativa que indica el producto interno bruto de cada país con dolares como unidad.

   Este proyecto incluye los siguientes documentos:

- [Reporte en formato ipynb](A1_2_Regresion_lineal.ipynb)
- [Reporte en formato html](A1_2_Regresion_lineal.html)
- [Base de datos original](A1_2_Felicidad_y_GDP.csv)
- [Base de datos adicional](Variables_Adicionales.csv)


# Solución de problemas y selección de características
En aplicaciones reales de ciencia de datos, rara vez se encuentran conjuntos preparados para utilizarse directamente en modelos predictivos. Presentándose en ocasiones escalas inconsistentes, valores atípicos y relaciones redundantes entre variables. Por lo cual, es esencial la selección adecuada de características que aporten información relevante para la predicción de una variable de interés; paso fundamental para la construcción de modelos interpretables.

Asimismo, se hará uso de la base de datos bajo el nombre “Calificaciones.csv”, presentándose información demográfica y académica de estudiantes de un curso, así como sus calificaciones parciales y finales.

De manera que, se buscará desarrollar un modelo de regresión lineal múltiple que permita predecir la calificación final. Analizando y enfrentando retos relacionados con el uso de datos reales y la adecuada selección de variables explicativas.

La base de datos cuenta con la siguiente información:
*  `Escuela` indica la escuela a la que pertenece el estudiante: *"Gabriel Pereira" (GP)* y *"Mousinho da Silveira" (MS)* .
*  `Sexo`  indica *F* para femenino y *M* para masculino.
*  `Edad`  indica la edad de los estudiantes en un rango de 15 a 22 años.
*  `HorasDeEstudio`  indica las horas de estudio del estudiaente:
      -  *1* representa menos de 2 horas.
      -  *2* representa de 2 a 5 horas.
      - *3* representa de 5 a 10 horas.
      -  *4* representa más de 10 horas.
*  `Reprobadas`  indica el número de materias reprobadas:
      -  *0* representa que no hay reprobación.
      -  *1*  representa que se ha reprobado una materia.
      - *2*  representa que se han reprobado dos materias.
      -  *4* representa tres o más materias reprobadas.
*  `Internet` indica si un estudiante tiene acceso a internet en casa: *yes* para los estudiantes con acceso y *no* para estudiantes que no tienen acceso.
*  `Faltas` indica el número de faltas de los estudiantes.
*  `G1` indica la calificación del primer periodo en una escala de 0 a 20.
*  `G2` indica la calificación del segundo periodo en una escala de 0 a 20.
*  `G3` indica la calificación del tercer periodo en una escala de 0 a 20.
 
  Este proyecto incluye los siguientes documentos:

- [Reporte en formato ipynb](A1_3_Solucion_de_problemas.ipynb)
- [Reporte en formato html](A1_3_Solucion_de_problemas.html)
- [Base de datos](Calificaciones.csv)

