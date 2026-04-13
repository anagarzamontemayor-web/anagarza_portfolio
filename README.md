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



# La deserción escolar: análisis de sus determinantes socioeconómicos

*La deserción escolar en México conlleva historias que van más allá de cifras, estas se miden en niñas y niños que dejan de ir a clases y familias con incertidumbre por un futuro truncado.*

De acuerdo con la Red por los Derechos de la Infancia en México (REDIM), entre 2016 y 2024 el abandono escolar ha sido una problemática constante que refleja desigualdades estructurales. 

En estados como Chiapas, Guerrero y Oaxaca, la deserción escolar se ha convertido en parte de la vida cotidiana, marcada por la pobreza, la violencia y la falta de oportunidades. Mientras tanto, entidades como la Ciudad de México o Nuevo León muestran realidades distintas, donde los niveles de abandono escolar son menores y las políticas educativas tienen mayor alcance. 

*Entonces, la deserción escolar no es solo una decisión individual, sino un fenómeno estructural que moldea comunidades enteras.*

Es en este punto donde el análisis estadístico de la deserción escolar cobra relevancia. Este tipo de modelos sintetiza, permiten comparar qué tan profundamente la deserción atraviesa la estructura social y económica de cada entidad federativa. 

De manera que, el presente estudio parte de esta realidad: analizar, a nivel estatal, cómo condiciones económicas, sociales y de bienestar se asocian con distintos niveles de deserción escolar en México. Buscando identificar qué variables contribuyen de manera significativa a explicar las diferencias territoriales observadas. Adicionalmente, mediante un ejercicio de simulación, se modificarán variables socioeconómicas clave para evaluar cómo podrían variar los niveles estimados de deserción escolar ante distintos contextos.

La base de datos utilizada en este estudio fue obtenida a partir de la integración de fuentes oficiales. Todas las variables socioeconómicas y de bienestar fueron recopiladas del portal estatal del [INEGI](https://www.inegi.org.mx/app/estatal/),con el fin de capturar condiciones estructurales relevantes en las 32 entidades federativas. 

La base de datos cuenta con la siguiente información:


*  `Entidad`  Nombre oficial de la entidad federativa.
*  `Desercion`  Porcentaje de deserción escolar.
*  `Sat_vida` Nivel promedio de satisfacción con la vida.
*  `Pobreza`  Porcentaje de la población en situación de pobreza.
*  `Pm25` Concentración promedio de partículas PM2.5 (µg/m³).
*  `Homicidios` Tasa de desocupación (%).
*  `Desocupacion` Tasa de homicidios por cada 100 mil habitantes.
*  `Serv_salud` Porcentaje de población con acceso a servicios de salud.
*  `Red_apoyo` Porcentaje de población que reporta contar con redes de apoyo.
*  `Analfabeta_15` Número de personas mayores de 15 años que no saben leer ni escribir.
*  `No_electricidad` Número de viviendas sin acceso a electricidad.
*  `Viv_habitadas` Número total de viviendas habitadas en la entidad.


Las variables expresadas en porcentaje representan proporciones relativas al total de viviendas de cada entidad federativa, lo cual permite comparabilidad territorial independientemente del tamaño poblacional.

Este proyecto incluye los siguientes documentos:

- [Reporte en formato ipynb](P1_Desercion_escola.ipynb)
- [Reporte en formato html](P1_Desercion_escola.html)
- [Base de datos](Desercion.csv)


  
# Regresión logística y validación cruzada

La pobreza en México conlleva historias que van más allá de cifras. De acuerdo con el INEGI, en 2024 29.6% de la población nacional (38.5 millones de personas) se encontraba en situación de pobreza multidimensional, mientras que 7 millones vivían en pobreza extrema. Estas cifras reflejan desigualdades estructurales que atraviesan comunidades enteras y condicionan su futuro. 

La base de datos empleada en este estudio proviene de la integración de fuentes oficiales, con variables socioeconómicas y de bienestar recopiladas del portal estatal del INEGI. 

Se trata de la misma base de datos utilizada en el trabajo previo “La deserción escolar: análisis de sus determinantes socioeconómicos”, correspondiente al periodo 2020–2022. Esto permite evaluar cómo factores estructurales recientes se relacionan con distintos niveles de abandono escolar en las 32 entidades federativas. Para la presente actividad se emplea la versión ya depurada del dataset, es decir, con el proceso de tratamiento y preparación de datos previamente realizado.

Teniendo como objetivo el adaptar el análisis de la pobreza a un escenario de clasificación binaria, evaluando rigurosamente la calidad del modelo de regresión logística mediante métricas como la exactitud, la sensibilidad y la especificidad. Asimismo, introduciendo el uso de la validación cruzada como herramienta metodológica para obtener estimaciones más sólidas y confiables.

La base de datos cuenta con la siguiente información:
*  `Entidad`  Nombre oficial de la entidad federativa.
*  `Pobreza`  Porcentaje de la población en situación de pobreza.
*  `Pm25` Concentración promedio de partículas PM2.5 (µg/m³).
*  `Homicidios` Tasa de desocupación (%).
*  `Desocupacion` Tasa de homicidios por cada 100 mil habitantes.
*  `Serv_salud` Porcentaje de población con acceso a servicios de salud.
*  `Red_apoyo` Porcentaje de población que reporta contar con redes de apoyo.
*  `Analfabeta_15` Número de personas mayores de 15 años que no saben leer ni escribir.
*  `No_electricidad` Número de viviendas sin acceso a electricidad.
*  `Viv_habitadas` Número total de viviendas habitadas en la entidad.
*  `Desercion`  Porcentaje de deserción escolar.
*  `Sat_vida` Nivel promedio de satisfacción con la vida.


Las variables expresadas en porcentaje representan proporciones relativas al total de viviendas de cada entidad federativa, lo cual permite comparabilidad territorial independientemente del tamaño poblacional.

Este proyecto incluye los siguientes documentos:

- [Reporte en formato ipynb](A2_1_Regresion_Logistica.ipynb)
- [Reporte en formato html](A2_1_Regresion_Logistica.html)
- [Base de datos](Desercion_depurado.csv)


# LDA y árboles de decisión

 De acuerdo con el INEGI, en 2024 29.6% de la población nacional (38.5 millones de personas) se encontraba en situación de pobreza multidimensional, mientras que 7 millones vivían en pobreza extrema. Estas cifras reflejan desigualdades estructurales que atraviesan comunidades enteras y condicionan su futuro. [1]

La base de datos empleada en este estudio proviene de la integración de fuentes oficiales, con variables socioeconómicas y de bienestar recopiladas del portal estatal del [INEGI](https://www.inegi.org.mx/app/estatal/). [2]

Se trata de la misma base de datos utilizada en el trabajo previo **“La deserción escolar: análisis de sus determinantes socioeconómicos”**, correspondiente al periodo 2020–2022.

 Para la presente actividad se emplea la versión ya depurada del dataset, es decir, con el proceso de tratamiento y preparación de datos previamente realizado y utilizado en proyectos anteriores.

Teniendo como objetivo el adaptar el análisis de la pobreza a un escenario de clasificación binaria, evaluando la calidad de dos enfoques: **Linear Discriminant Analysis (LDA) y árboles de decisión** . Aplicando ambos modelos sobre el mismo conjunto de datos y estableciendo la variable *Pobreza* como clase objetivo con el resto de las variables como predictoras.

En el presente análisis, la variable de salida seleccionada es `Pobreza`, que representa el porcentaje de población en situación de pobreza multidimensional en cada entidad federativa.

La base de datos cuenta con la siguiente información:

| Variable          | Descripción                                                                 |
|-------------------|-----------------------------------------------------------------------------|
| **Entidad**       | Nombre oficial de la entidad federativa.                                    |
| **Pobreza**       | Porcentaje de la población en situación de pobreza.                         |
| **Pm25**          | Concentración promedio de partículas PM2.5 (µg/m³).                         |
| **Homicidios**    | Tasa de homicidios por cada 100 mil habitantes.                             |
| **Desocupacion**  | Tasa de desocupación (%).                                                   |
| **Serv_salud**    | Porcentaje de población con acceso a servicios de salud.                    |
| **Red_apoyo**     | Porcentaje de población que reporta contar con redes de apoyo.              |
| **Analfabeta_15** | Número de personas mayores de 15 años que no saben leer ni escribir.        |
| **No_electricidad** | Número de viviendas sin acceso a electricidad.                           |
| **Viv_habitadas** | Número total de viviendas habitadas en la entidad.                          |
| **Desercion**     | Porcentaje de deserción escolar.                                            |
| **Sat_vida**      | Nivel promedio de satisfacción con la vida.                                 |


Las variables expresadas en porcentaje representan proporciones relativas al total de viviendas de cada entidad federativa, lo cual permite comparabilidad territorial independientemente del tamaño poblacional.


Este proyecto incluye los siguientes documentos:

- [Reporte en formato ipynb](A2_2_LDA_Arboles.ipynb)
- [Reporte en formato html](A2_2_LDA_Arboles.html)
- [Base de datos](Desercion_depurado.csv)

# Modelos de ensamble, SVM y redes neuronales

De acuerdo con el INEGI, en 2024 29.6% de la población nacional (38.5 millones de personas) se encontraba en situación de pobreza multidimensional, mientras que 7 millones vivían en pobreza extrema. Estas cifras reflejan desigualdades estructurales que atraviesan comunidades enteras y condicionan su futuro. 

La base de datos empleada en este estudio proviene de la integración de fuentes oficiales, con variables socioeconómicas y de bienestar recopiladas del portal estatal del [INEGI](https://www.inegi.org.mx/app/estatal/). 

Se trata de la misma base de datos utilizada en el trabajo previo **“La deserción escolar: análisis de sus determinantes socioeconómicos”**, correspondiente al periodo 2020–2022.

Para la presente actividad se emplea la versión ya depurada del dataset, es decir, con el proceso de tratamiento y preparación de datos previamente realizado y utilizado en proyectos anteriores.

Teniendo como objetivo *entrenar y comparar distintos modelos avanzados de clasificación (basados en ensambles, márgenes máximos y redes neuronales) evaluando su desempeño en el mismo conjunto de datos* y reflexionando sobre las diferencias observadas en términos de capacidad predictiva, estabilidad y complejidad del modelo.

La base de datos cuenta con la siguiente información:

| Variable          | Descripción                                                                 |
|-------------------|-----------------------------------------------------------------------------|
| **Entidad**       | Nombre oficial de la entidad federativa.                                    |
| **Pobreza**       | Porcentaje de la población en situación de pobreza.                         |
| **Pm25**          | Concentración promedio de partículas PM2.5 (µg/m³).                         |
| **Homicidios**    | Tasa de homicidios por cada 100 mil habitantes.                             |
| **Desocupacion**  | Tasa de desocupación (%).                                                   |
| **Serv_salud**    | Porcentaje de población con acceso a servicios de salud.                    |
| **Red_apoyo**     | Porcentaje de población que reporta contar con redes de apoyo.              |
| **Analfabeta_15** | Número de personas mayores de 15 años que no saben leer ni escribir.        |
| **No_electricidad** | Número de viviendas sin acceso a electricidad.                           |
| **Viv_habitadas** | Número total de viviendas habitadas en la entidad.                          |
| **Desercion**     | Porcentaje de deserción escolar.                                            |
| **Sat_vida**      | Nivel promedio de satisfacción con la vida.                                 |


Las variables expresadas en porcentaje representan proporciones relativas al total de viviendas de cada entidad federativa, lo cual permite comparabilidad territorial independientemente del tamaño poblacional.

Este proyecto incluye los siguientes documentos:

- [Reporte en formato ipynb](A2_3_Modelos_de_ensamble_SVM_y_redes_neuronales.ipynb)
- [Reporte en formato html](A2_3_Modelos_de_ensamble_SVM_y_redes_neuronales.html)
- [Base de datos](Desercion_depurado.csv)

# Análisis comparativo de modelos de clasificación para la detección de pobreza en entidades de México

En México, la pobreza continúa siendo una de las problemáticas sociales más relevantes, al reflejar desigualdades estructurales que afectan directamente la calidad de vida de millones de personas. De acuerdo con el INEGI, en 2024 el 29.6% de la población nacional (38.5 millones de personas) se encontraba en situación de pobreza multidimensional, mientras que alrededor de 7 millones vivían en pobreza extrema.

### **Enfoque del estudio**
El presente trabajo tiene como propósito analizar el nivel de pobreza a partir de variables socioeconómicas, utilizando modelos de clasificación que permitan asignar cada observación a una categoría específica (pobreza alta o pobreza baja).

### **Ficha técnica del estudio**

*Fuente de datos:*
Datos obtenidos de fuentes oficiales del [INEGI](https://www.inegi.org.mx/app/estatal/), a través de su portal estatal.

*Periodo:*
2020 – 2022

*Origen del dataset:*
Base de datos previamente utilizada en el estudio:
“La deserción escolar: análisis de sus determinantes socioeconómicos”

*Estado de los datos:*
Dataset previamente depurados (sin modificaciones adicionales)

*Variable objetivo:*
Clasificación del nivel de pobreza:
* Pobreza alta
* Pobreza baja

*Objetivo del modelo:*
Desarrollar y comparar distintos modelos de clasificación para identificar cuál presenta mejor desempeño en la predicción del nivel de pobreza, así como analizar las diferencias entre ellos en términos de capacidad predictiva y complejidad.

La base de datos cuenta con la siguiente información:

| Variable          | Descripción                                                                 |
|-------------------|-----------------------------------------------------------------------------|
| **Entidad**       | Nombre oficial de la entidad federativa.                                    |
| **Pobreza**       | Porcentaje de la población en situación de pobreza.                         |
| **Pm25**          | Concentración promedio de partículas PM2.5 (µg/m³).                         |
| **Homicidios**    | Tasa de homicidios por cada 100 mil habitantes.                             |
| **Desocupacion**  | Tasa de desocupación (%).                                                   |
| **Serv_salud**    | Porcentaje de población con acceso a servicios de salud.                    |
| **Red_apoyo**     | Porcentaje de población que reporta contar con redes de apoyo.              |
| **Analfabeta_15** | Número de personas mayores de 15 años que no saben leer ni escribir.        |
| **No_electricidad** | Número de viviendas sin acceso a electricidad.                           |
| **Viv_habitadas** | Número total de viviendas habitadas en la entidad.                          |
| **Desercion**     | Porcentaje de deserción escolar.                                            |
| **Sat_vida**      | Nivel promedio de satisfacción con la vida.                                 |


Las variables expresadas en porcentaje representan proporciones relativas al total de viviendas de cada entidad federativa, lo cual permite comparabilidad territorial independientemente del tamaño poblacional.

Este proyecto incluye los siguientes documentos:

- [Reporte en formato ipynb](Proyecto_pobreza.ipynb)
- [Reporte en formato html](Proyecto_pobreza.html)
- [Base de datos](pobreza_depurado.csv)

# Modelos de ensamble, SVM y redes neuronales

De acuerdo con el INEGI, en 2024 29.6% de la población nacional (38.5 millones de personas) se encontraba en situación de pobreza multidimensional, mientras que 7 millones vivían en pobreza extrema. Estas cifras reflejan desigualdades estructurales que atraviesan comunidades enteras y condicionan su futuro. 

La base de datos empleada en este estudio proviene de la integración de fuentes oficiales, con variables socioeconómicas y de bienestar recopiladas del portal estatal del [INEGI](https://www.inegi.org.mx/app/estatal/). 

Se trata de la misma base de datos utilizada en el trabajo previo **“La deserción escolar: análisis de sus determinantes socioeconómicos”**, correspondiente al periodo 2020–2022.

Para la presente actividad se emplea la versión ya depurada del dataset, es decir, con el proceso de tratamiento y preparación de datos previamente realizado y utilizado en proyectos anteriores.

Teniendo como objetivo *entrenar y comparar distintos modelos avanzados de clasificación (basados en ensambles, márgenes máximos y redes neuronales) evaluando su desempeño en el mismo conjunto de datos* y reflexionando sobre las diferencias observadas en términos de capacidad predictiva, estabilidad y complejidad del modelo.

La base de datos cuenta con la siguiente información:

| Variable          | Descripción                                                                 |
|-------------------|-----------------------------------------------------------------------------|
| **Entidad**       | Nombre oficial de la entidad federativa.                                    |
| **Pobreza**       | Porcentaje de la población en situación de pobreza.                         |
| **Pm25**          | Concentración promedio de partículas PM2.5 (µg/m³).                         |
| **Homicidios**    | Tasa de homicidios por cada 100 mil habitantes.                             |
| **Desocupacion**  | Tasa de desocupación (%).                                                   |
| **Serv_salud**    | Porcentaje de población con acceso a servicios de salud.                    |
| **Red_apoyo**     | Porcentaje de población que reporta contar con redes de apoyo.              |
| **Analfabeta_15** | Número de personas mayores de 15 años que no saben leer ni escribir.        |
| **No_electricidad** | Número de viviendas sin acceso a electricidad.                           |
| **Viv_habitadas** | Número total de viviendas habitadas en la entidad.                          |
| **Desercion**     | Porcentaje de deserción escolar.                                            |
| **Sat_vida**      | Nivel promedio de satisfacción con la vida.                                 |


Las variables expresadas en porcentaje representan proporciones relativas al total de viviendas de cada entidad federativa, lo cual permite comparabilidad territorial independientemente del tamaño poblacional.

Este proyecto incluye los siguientes documentos:

- [Reporte en formato ipynb](A2_3_Modelos_de_ensamble_SVM_y_redes_neuronales.ipynb)
- [Reporte en formato html](A2_3_Modelos_de_ensamble_SVM_y_redes_neuronales.html)
- [Base de datos](Desercion_depurado.csv)

# Principal Component Analysis (PCA)

En la presente actividad se trabajará con la base de datos llamada "Breast Cancer Wisconcin" incluida en la librería scikit-learn con la función *load_breast_cancer()*, con el objetivo de aplicar el **Análisis de Componentes Principales (PCA)**.

Con ello se buscará comprender como esta reducción de dimensionalidad permite simplififcar la información sin perder su esencia, igualmente analizando la proporción de varianza explicada y la importancia de las cargas de cada variable. Utilizándose gráficos y visualizaciones que facilitan la interpretación de resultados.

Para ello se planteará el presente ejercicio como un **tutorial teórico**, explicando el proceso para aplicar PCA, tomando en cuenta desde la preparación de los datos hasta la interpretación de los resultados.

Este proyecto incluye los siguientes documentos:

- [Reporte en formato ipynb](PCA.ipynb)
- [Reporte en formato html](PCA.html)


# Sistema de Recomendación de Películas con Matrix Completion

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://anagarzamontemayor-web-recomendador-peliculas-ia.streamlit.app)

> *“La completación de matrices permite estimar valores faltantes en una matriz de ratings usuario-ítem, revelando patrones ocultos de preferencias sin necesidad de características explícitas.”*  
> — [Dharshan Kumar, *Building a Recommendation System using Matrix Completion*](https://dharshankumar.medium.com/building-a-recommendation-system-using-matrix-completion-6b2ab5fc5604)


## Objetivo
Se busca aplicar los fundamentos teóricos del matrix completion para construir, desde cero, un sistema interactivo que simule un sistema de recomendación que incluso sin atributos explícitos encuentre patrones de preferencias ocultos y ser capaz de brindar sugerencias personalizadas. 
---

## ¿Qué hace esta aplicación?

Elige tus películas favoritas, califícalas del 1 al 5 y se desplegará **10 recomendaciones personalizadas** generadas mediante **matrix completion** sobre el dataset **MovieLens 100k**.  
Lográndose mediante un modelo de imputación iterativa que completa la matriz usuario película y que encuentra recomendaciones similares a tu perfil cinematográfico.

---

## 🚀 ¡Pruébala ya!

Haz clic en el botón de abajo para acceder a la aplicación desplegada en **Streamlit Cloud**:

<p align="center">
  <a href="https://recomendador-peliculas-ia.streamlit.app/">
    <img src="https://img.shields.io/badge/🎥%20Ver%20App%20en%20Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white" alt="Abrir App">
  </a>
</p>


---

## 🔹 Paso a paso del código

| Etapa | ¿Qué hace? | Archivo |
|-------|------------|---------|
| **Carga de datos** | Lee los archivos `u.data` (ratings) y `u.item` (nombres de películas). | `recommender.py` |
| **Tabla usuario película** | Arma una matriz donde cada fila es un usuario y cada columna una película. Los huecos se establecen como `NaN`. | `recommender.py` |
| **Huecos** | Para lograr funcionamiento   en la nube, usamos solo los **50 usuarios más activos** y las **50 películas más populares**. | `recommender.py` |
| **Interfaz** | Se muestra una lista de películas populares, se eligen al menos 5 y se califican con del 1 al 5. | `app.py` |
| **Recomendación** | Cuando se presiona el botón, se busca usuarios con gustos parecidos y, basándose en sus gustos, predice qué otras películas podrían interesar. | `recommender.py` |
| **Visualización** | Se muestra un heatmap que indica los huecos originales en la tabla. | `app.py` |









