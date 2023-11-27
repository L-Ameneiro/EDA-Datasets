# Perfiles de consumo eléctrico y transición energética

### Realizado en el marco del Curso Ingenias DataScience - 2023

## Integrantes: 
Luciana Carvajal ([LucianaCarvajal](https://github.com/LucianaCarvajal)) <br>
Leila Luna Ameneiro ([L-Ameneiro](https://github.com/L-Ameneiro))

## Breve descripcion del proyecto
[Comience brindando una breve descripción general del proyecto, de qué se trata y qué pretende lograr. Esto ayudará a los lectores a comprender rápidamente de qué se trata el proyecto.]


## Preguntas generales

Cuanto dependemos de los combustibles fosiles para abastecer de electricidad a la poblacion y a la industria? 
Como se encuentra posicionada la Argentina en los intentos de transicion energetica? 

## Objetivo 


## Notebooks


[Explique la estructura del código y cómo está organizado, incluidos los archivos importantes y sus propósitos. Esto ayudará a otros a comprender cómo navegar por su proyecto y encontrar componentes específicos.]

1. EDA.ipynb: Analisis exploratorio inicial de los datos. 

2. limpieza_procesamiento.ipynb --> Limpieza de datos nulos. Seleccion de variables de interes. Creacion de datasets para los modelos supervisado y no supervisado. 

3. modelo_no_supervisado.ipynb --> Estudio de la dependencia de fuentes fosiles usando un algoritmo de clustering DBSCAN. 

4. modelo_supervisado.ipynb --> Proyeccion de consumo de energia eolica en paises de Sudamerica mediante regresion lineal.
   
5. visualizaciones.ipynb --> Produccion de graficos para presentacion final. 

   

## Datasets

[List all the data sources used in the project, including links to the original data, descriptions of the data, and any pre-processing steps that were taken.]

## Glosario

| Término                                | Definición                                                    |
|-----------------------------------------|--------------------------------------------------------------|
| iso_code:                               | códigos de países de tres letras ISO 3166-1 lfa-3. |   
| population:                             | Población total, meido en millones de habitantes.|
| low_carbon_share_elec:                  | Proporción del consumo de electricidad que proviene de fuentes bajas en carbono. Medido en teravatios-hora.|
| country:                                | Ubicación geográfica del país.|
| fossil_share_elec:                      | Proporción de generación de electricidad que proviene de combustibles fósiles (carbón, petróleo y gas combinados).|
| renewables_share_elec:                  | Proporción de generación de electricidad que proviene de energías renovables.|
| nuclear_share_elec:                     | Proporción de generación de electricidad que proviene de la energía nuclear.|
| fossil_cons_per_capita:                 | Consumo de combustibles fósiles per capita, medido en Kilovatios-hora. Esta es la suma de la energía primaria procedente del carbón, el petróleo y el gas.|
| per_capita_electricity:                 | Generación de electricidad per cápita, medida en kilovatios-hora.|
| continente:                             | Agrupamiento de países según la extensión de tierra separada por los océanos y, en general, por determinados accidentes geográficos.|
| year:                                   | Año de observación.|
| coal_share_elec:                        | Proporción de generación de electricidad que proviene del carbón.|
| acceso_elec:                            | Porcentaje de la población con acceso a la electricidad.|
| coal_elec_per_capita:                   | Demanda de electricidad, medida en teravatios-hora.|
| biofuel_electricity:                    | Generación de electricidad a partir de combustibles fósiles, medida en teravatios-hora. Esta es la suma de la generación de electricidad a partir de carbón, petróleo y gas.|
| coal_electricity:                       | Generación de electricidad a partir de carbón, medida en teravatios-hora.|
| fossil_electricity:                     | Generación de electricidad a partir de combustibles fósiles, medida en teravatios-hora. Esta es la suma de la generación de electricidad a partir de carbón, petróleo y gas.|
| gas_electricity:                        | Generación de electricidad a partir de gas, medida en teravatios-hora.|
| hydro_electricity:                      | Generación de electricidad a partir de energía hidroeléctrica, medida en teravatios-hora.|
| nuclear_electricity:                    | Generación de electricidad a partir de energía nuclear, medida en teravatios-hora.|
| oil_electricity:                        | Generación de electricidad a partir de petróleo, medida en teravatios-hora.|
| other_renewable_electricity:            | Generación de electricidad a partir de otras fuentes renovables, incluidos los biocombustibles, medida en teravatios-hora.|
| other_renewable_exc_biofuel_electricity:| Generación de electricidad per cápita a partir de otras energías renovables, excluidos los biocombustibles, medida en kilovatios-hora.|
| renewables_electricity:                 | Generación de electricidad a partir de energías renovables, medida en teravatios-hora.|
| solar_electricity:                      | Generación de electricidad a partir de energía solar, medida en teravatios-hora.|
| wind_electricity:                       | Generación de electricidad a partir del viento, medida en teravatios-hora.|
| energy_per_capita:                      | Consumo de energía primaria per cápita, medido en kilovatios-hora.|
| fossil_cons_per_capita:                 | Consumo de combustibles fósiles per cápita, medido en kilovatios-hora. Esta es la suma de la energía primaria procedente del carbón, el petróleo y el gas.|
| gas_share_elec:                         | Proporción de generación de electricidad que proviene del gas.|
| gas_elec_per_capita:                    | Generación de electricidad per cápita a partir de gas, medida en kilovatios-hora.|
| hydro_share_elec:                       |Proporción de generación de electricidad que proviene de la energía hidroeléctrica.|
| hydro_elec_per_capita:                  | Generación de electricidad per cápita a partir de fuentes bajas en carbono, medida en kilovatios-hora.|
| low_carbon_electricity:                 | Generación de electricidad a partir de fuentes bajas en carbono, medida en teravatios-hora. Esta es la suma de la generación de electricidad a partir de energías renovables y energía nuclear.|
| low_carbon_elec_per_capita:             | Generación de electricidad per cápita a partir de fuentes bajas en carbono, medida en kilovatios-hora.|
| oil_share_elec:                         | Proporción de generación de electricidad que proviene del petróleo.|
| oil_elec_per_capita:                    | Generación de electricidad per cápita a partir de petróleo, medida en kilovatios-hora.|
| other_renewables_elec_per_capita:       | Generación de electricidad per cápita a partir de otras energías renovables, incluidos los biocombustibles, medida en kilovatios-hora.|
| other_renewables_share_elec:            | Proporción de generación de electricidad que proviene de otras energías renovables, incluidos los biocombustiblesla Revisión europea de electricidad.|
| primary_energy_consumption:             | Consumo de energía primaria, medido en teravatios-hora.|
| renewables_elec_per_capita:             | Generación de electricidad per cápita a partir de energías renovables, medida en kilovatios-hora.|
| solar_share_elec:                       | Proporción de generación de electricidad que proviene de la energía solar.|
| solar_elec_per_capita:                  | Generación de electricidad per cápita a partir de energía solar, medida en kilovatios-hora.| 
| wind_share_elec:                        | Proporción de generación de electricidad que proviene del viento.|
| wind_elec_per_capita:                   | Generación de electricidad per cápita a partir del viento, medida en kilovatios-hora.|
| biofuel_electricity:                    | Generación de electricidad a partir de biocombustibles, medida en teravatios-hora.|


De todas las variables numericas se calculo la media por pais desde el anio 2010.



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
Todo el proyecto fue desarrollado en Python notebooks (ipynb). Version de Python  3.11.5. <br>
Para correrlas debe tenerse instalado Python 3.11.5.

## Librerias utilizadas

**Todas las notebooks** <br>
`pandas` <br>
`numpy` <br>
`plotly.express` <br>
`matplotlib.pyplot` <br>
<br>
**Clustering DBSCAN** <br>
`sklearn.cluster`<br>
`sklearn.metrics`<br>
<br>
**Regresion lineal**<br>


## Licencia

Los datos, las visualizaciones y el codigo producido por las autoras de este repositorio es de acceso completamente abierto bajo la licencia [Creative Commons BY](https://creativecommons.org/licenses/by/4.0/). Se puede descargar, compartir y modificar siempre que la fuente original sea citada.  <br>
A noviembre de 2023, la misma licencia aplica a los datasets utilizados, producidos por **Our World in Data**. 

## Agradecimientos
Este trabajo no hubiera sido posible sin el programa YPF-Ingenias y las instructoras de Jump! Media Chicas. <br>
Gracias a Irina, Charly, Gianella y Tamara por la paciencia y a todxs lxs que hacen su aporte para llevar adelante el programa.  <br>
Tambien queremos reconocer el enorme aporte de **Our World in Data** por proveer y mantener el dataset fuente utilizado. 



