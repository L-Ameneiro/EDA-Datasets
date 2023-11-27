# Perfiles de consumo electrico

### Realizado en el marco del Curso Ingenias DataScience - 2023

## Integrantes: 
Luciana Carvajal ([LucianaCarvajal](https://github.com/LucianaCarvajal)) <br>
Leila Luna Ameneiro ([L-Ameneiro](https://github.com/L-Ameneiro))

## Breve descripcion del proyecto
[Start by providing a brief overview of the project, what it is about, and what it aims to achieve. This will help readers quickly understand what the project is all about.]


## Preguntas generales

Cuanto dependemos de los combustibles fosiles para abastecer de electricidad a la poblacion y a la industria? 
Como se encuentra posicionada la Argentina en los intentos de transicion energetica? 

## Objetivo 


## Notebooks

[Explain the code structure and how it is organized, including any significant files and their purposes. This will help others understand how to navigate your project and find specific components.]

1. EDA: Analisis exploratorio inicial de los datos. 

2. Limpieza y procesamiento:

3. Modelo no supervisado: Estudio de la dependencia de fuentes fosiles

4. Modelo supervisado. Proyeccion de consumo de energia eolica en paises de Sudamerica. 

## Datasets

[List all the data sources used in the project, including links to the original data, descriptions of the data, and any pre-processing steps that were taken.]

**Datos fuente**

- World_Energy_Consumption.csv
Dataset sobre energia mantenido por la organizacion [Our World in Data](https://ourworldindata.org/). Contiene cientos de metricas relevantes sobre consumo y produccion energetica por anio para cada pais del mundo. Algunas columnas contienen gran proporcion de datos nulos.  
Descargado de https://www.kaggle.com/datasets/pralabhpoudel/world-energy-consumption/data.
https://github.com/owid/energy-data

- acces to electricity (si lo usamos)

consumption-co2-per-capita-vs-gdppc.csv

**Datos procesados**
- wec_ns.csv
Contiene datos de porcentaje de consumo electrico proveniente de distintas fuentes (medias de los anios 2010-2020 para cada pais del mundo).
Generado a partir de World_Energy_Consumption.csv en notebook de limpieza y procesamiento. 

## Resultados

Provide an overview of the results of your project, including any relevant metrics and graphs. Include explanations of any evaluation methodologies and how they were used to assess the quality of the model. You can also make it appealing by including any pictures of your analysis or visualizations.


## Instrucciones
[Provide detailed instructions on how to set up the project on a local machine. This includes any necessary dependencies, software requirements, and installation steps. Make sure to include clear and concise instructions so that others can easily replicate your setup.]

## Librerias utilizadas

**Todas las notebooks**
pandas
numpy
plotly.express
matplotlib.pyplot

**Clustering DBSCAN**
sklearn.cluster.
sklearn.metrics

**Regresion lineal**


## Licencia

Los datos, las visualizaciones y el codigo producido por las autoras de este repositorio es de acceso completamente abierto bajo la licencia [Creative Commons BY](https://creativecommons.org/licenses/by/4.0/). Se puede descargar, compartir y modificar siempre que la fuente original sea citada. 

A noviembre de 2023, la misma licencia aplica a los datasets utilizados, producidos por **Our World in Data**. 

## Agradecimientos
Este trabajo no hubiera sido posible sin el programa YPF-Ingenias y las instructoras de Jump! Media Chicas. 
Gracias a Irina, Charly, Gianella y Tamara por la paciencia y a todxs lxs que hacen su aporte para llevar adelante el programa.  

Tambien queremos reconocer el enorme aporte de **Our World in Data** por proveer y mantener el dataset fuente utilizado. 



