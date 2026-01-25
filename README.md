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
  
Dede 2012 el World Happiness Report (WHR) ha propuesto una metodología para estimar un concepto tan complejo y dificil de medir, la felicidad. De manera que, a partir de estos estudios, factores económicos, sociales y de salud han sido analizados con posibles explicaciones basandose en las diferencias presentes entre países. Entre ellos, el producto interno bruto (GDP) y otros elementos relevantes.

Asimismo, se hará uso de la base de datos bajo el nombre “A1.2 Felicidad y GDP.csv”, presentándose información sobre el nivel de felicidad reportado en 2022 y el GDP correspondiente a 2020 para distintos países. Cabe destacar que, al trabajar con variables económicas, se considerarán transformaciones adecuadas para así trabajar con variables lineales. Analizando así, la conveniencia de utilizar o no una transformación.

Exploración y contextualización de los datos

Expertos en economía, psicología, sociología y otras disciplinas analizan información interdisciplinaria sobre el bienestar y la felicidad de las personas el mundo. Para ello, el Centro de Investigación del Bienestar de la Universidad de Oxford, en colaboración con Gallup, la SDSN y un consejo editorial independiente clasifica anualmente a 146 países la evaluación del promedio de la calidad de vida de la población. Pidiendo a los encuesados calificar su vida actual en una escala del 0 al 10, donde 10 representa la mejor vida posible y 0 la peor. [1]

Si bien, estos resultados se basan en autopercepción, se consideran como factor clave el producto interno bruto (GDP), es decir, el conjunto de bienes y servicios producidos por un país durante un año. [2]

El conjunto de datos disponible cuenta con tres variables principales:

País variable categórica que indica el país representante.
Felicidad variable cuantitativa que indica la perceoición de felicidad en una escala de 0-10.
GDP variable cuantitativa que indica el producto interno bruto de cada país con dolares como unidad.

