# Perfiles de consumo eléctrico y transición energética

### Realizado en el marco del Curso Ingenias DataScience - 2023

## Integrantes: 
Luciana Carvajal ([LucianaCarvajal](https://github.com/LucianaCarvajal)) <br>
Leila Luna Ameneiro ([L-Ameneiro](https://github.com/L-Ameneiro))

## Breve descripcion del proyecto

Este informe muestra el proceso de exploración, análisis y modelado de datos en relación a métricas de consumo y producción de electricidad a nivel mundial para determinar el nivel de dependencia de los países del mundo respecto de los combustibles fósiles utilizados para la electricidad. Para esto, se agruparán a los países de acuerdo a electricidad proveniente de fuentes renovables, fósiles y nucleares. <br>
Por otra parte, se describirán las características de los países que influyen en la producción de electricidad de bajas emisiones de carbono per cápita.


## Preguntas generales

¿ De qué fuentes proviene la electricidad que consumimos en el mundo? <br>
¿Cuánto dependemos de los combustibles fósiles para abastecer de electricidad a la población y a la industria? <br>
¿En que etapa de transición del cambio energético de fósil a renovable se encuentran los países del mundo? <br>
¿En que etapa de transición del cambio energético de fósil a renovable se encuentran los países de sudamérica? <br>
¿Qué características de un país influyen en la producción de electricidad baja en emisiones de carbono per cápita?


## Objetivo 

- Agrupar a los países del mundo respecto de la dependencia de los combustibles fósiles utilizados para la electricidad, de acuerdo a las fuentes renovables, fósiles y nucleares. <br>
- Describir las características de los países que influyen en la producción de electricidad de bajas emisiones de carbono per cápita.

## Notebooks


1. EDA.ipynb: Analisis exploratorio de los datos --> Limpieza de datos nulos. Seleccion de variables de interes. Creacion de datasets para los modelos supervisado y no supervisado.

2. clustering_perfil_energetico.ipynb  --> Estudio de la dependencia de fuentes fósiles usando un algoritmo de clustering DBSCAN. 

3. produccion_low_carbon.ipynb--> Caracterizar de las features que influyen en la producción de electricidad low-carbon per cápita de los países.



**Datos fuente**

- World_Energy_Consumption.csv
Dataset sobre energia mantenido por la organizacion [Our World in Data](https://ourworldindata.org/). Contiene cientos de metricas relevantes sobre consumo y produccion energetica por anio para cada pais del mundo. Algunas columnas contienen gran proporcion de datos nulos.  
Descargado de https://www.kaggle.com/datasets/pralabhpoudel/world-energy-consumption/data.
Fuente actualizada: https://github.com/owid/energy-data

- Nivel de ingresos de acuerdo al Banco Mundial de cuardo al año 2023 (mapeo en notebook EDA)


**Datos procesados**
- wec_ns.csv
Contiene datos de porcentaje de consumo electrico proveniente de distintas fuentes (medias de los anios 2010-2020 para cada pais del mundo).
Generado a partir de World_Energy_Consumption.csv en notebook de limpieza y procesamiento. 

## Glosario


| Término                                 |Definición                                         |
|----------------------------|----------------------------------------------------------------|
| continente:                | Agrupamiento de países según la extensión de 
| country:                   | Ubicación geográfica del país.|
| iso_code:                  | códigos de países de tres letras ISO 3166-1 lfa-3. | 
| low_carbon_share_elec:     | Proporción del consumo de electricidad que proviene de fuentes bajas en carbono. Medido en teravatios-hora.|
| low_carbon_elec_per_capita:| Generación de electricidad per cápita a partir de fuentes bajas en carbono, medida en kilovatios-hora.|
| nuclear_electricity:       | Generación de electricidad a partir de energía nuclear, medida en teravatios-hora.|
| population:                | Población total, meido en millones de habitantes.|
| renewables_electricity:    | Generación de electricidad a partir de energías renovables, medida en teravatios-hora.|


De todas las variables numericas se calculo la media por pais desde el anio 2010.

## Resultados

**Clustering por perfiles energéticos**
Los países del mundo poseen gran diversidad de perfiles energéticos. En referencia a sudamérica, se encuentran países agrupados en los 5 clusters arrojados por el modelo. En un extremo, se ubican los países como Paraguay y Uruguay; que muestran gran independencia de los combustibles fósiles para electricidad. En el otro, países como Trinidad y Tobago y Granada que muestran total dependencia de los combustibles fósiles. <br>
La producción de electricidad low-carbon per capita(teravatios-hora/habitante), mantiene una relación inversamente proporcional con la población de cada país. <br>
**Variables que determinan producción de energías low-carbon**
Las variables con mayor impacto en la producción de energía low_carbon de un país son su población y su nivel de ingresos, con menores aportes del contienente y casi sin aporte del año.


## Instrucciones

Todo el proyecto fue desarrollado en Python notebooks (ipynb). Version de Python  3.11.5. <br>
Cada notebook incluye las instrucciones para importar las librerías necesarias. 

## Librerias utilizadas

Todas las notebooks:
- `pandas` <br>
- `numpy` <br>
- `plotly.express` <br>
- `matplotlib.pyplot` <br>

**Clustering DBSCAN** <br>
- `sklearn.cluster`<br>
- `sklearn.metrics`<br>

**Regresión**
- `sklearn.linear_model`<br>
- `sklearn.ensemble`<br>
- `sklearn.svm`<br>
- `sklearn.model_selection`<br>


## Licencia

Los datos, las visualizaciones y el codigo producido por las autoras de este repositorio es de acceso completamente abierto bajo la licencia [Creative Commons BY](https://creativecommons.org/licenses/by/4.0/). Se puede descargar, compartir y modificar siempre que la fuente original sea citada.  <br>
A noviembre de 2023, la misma licencia aplica a los datasets utilizados, producidos por **Our World in Data**. 

## Agradecimientos
Este trabajo no hubiera sido posible sin el programa YPF-Ingenias y las instructoras de Jump! Media Chicas. <br>
Gracias a Irina, Charly, Gianella y Tamara por la paciencia y a todxs lxs que hacen su aporte para llevar adelante el programa.  <br>
Tambien queremos reconocer el enorme aporte de **Our World in Data** por proveer y mantener el dataset fuente utilizado. 



