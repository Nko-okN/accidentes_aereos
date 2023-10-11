# Proyecto Individual Data Analytics: Accidentes aéreos

Este proyecto consiste en analizar los accidentes aéreos ocurridos desde 1908 y hasta 2021 y presentar los insights más importantes es un dashboard de Power BI.

<br>

![Static Badge](https://img.shields.io/badge/Python-gray?style=flat&logo=python)
![Pandas](https://img.shields.io/badge/-Pandas-gray?style=flat&logo=pandas)
![Matplotlib](https://img.shields.io/badge/-Matplotlib-gray?style=flat&logo=matplotlib)
![Seaborn](https://img.shields.io/badge/-Seaborn-gray?style=flat&logo=seaborn)



<br>

## Índice

- [Introducción](#Introducción)
- [Objetivo](#Objetivo)
- [Repositorio](#Repositorio)
- [Pasos para la realización de este proyecto](#Pasos)
- [ETL](#ETL)
- [EDA: Exploratory Data Analysis](#EDA)
- [Dashboard](#Dashboard)
- [Conclusiones](#Conclusiones)
- [Herramientas utilizadas](#Herramientas)
- [Disclaimer](#Disclaimer)


<br>

## Introducción

Este proyecto se enfoca en analizar datos históricos recopilados de fuentes públicas sobre accidentes de aviación que ocurrieron entre 1908 y 2021. Según la definición de la Organización de Aviación Civil Internacional, un accidente es cualquier evento relacionado con la operación de una aeronave en el que:

- Cualquier persona sufre lesiones graves o fatales.
- La aeronave sufre daños o fallos estructurales que requieren reparación.
- La aeronave se considera desaparecida.

Los accidentes de aviación son eventos inesperados y no deseados que involucran aeronaves, resultando en daño a personas y daños materiales a la propia aeronave.

Estos accidentes pueden ser causados por diversos factores, como errores humanos, fallos en el equipamiento, condiciones climáticas adversas, problemas de mantenimiento, deficiencias en la gestión del tráfico aéreo, problemas de diseño o defectos de fabricación. Por lo tanto, la industria de la aviación, las autoridades reguladoras y los investigadores trabajan juntos para mejorar la seguridad de la aviación y prevenir futuros accidentes. Comprender las causas de los accidentes y aprender a prevenirlos es fundamental para evitar pérdidas humanas y daños materiales.

## Objetivo

El objetivo principal de este proyecto es realizar un análisis de datos relacionados con la comprensión de los accidentes de aviación a lo largo de la historia y tomar acciones preventivas en consecuencia. Los resultados se presentarán junto con dos Indicadores Clave de Desempeño (KPI) propuestos en un panel de visualización que complementa el análisis con visualizaciones.

## Repositorio

El repositorio de este proyecto consta de los siguientes archivos:

- El archivo [ETL.ipynb](ETL.ipynb) muestra el proceso de Extracción, Transformación y Carga (ETL) y proporciona un enfoque inicial para el análisis exploratorio de datos del conjunto de datos.
- El archivo [EDA.ipynb](EDA.ipynb) presenta un análisis exploratorio de datos que busca identificar relaciones entre variables y patrones en los datos.


## Pasos para completar este proyecto
### ETL (Extracción, Transformación y Carga)

Después de un examen inicial de los datos en el archivo [AccidentesAviones.csv](AccidentesAviones.csv), procedimos a investigar las columnas del conjunto de datos. Según la información proporcionada, el diccionario de datos del conjunto de datos se puede resumir de la siguiente manera:

- **Unnamed: 0:** Índice para cada registro de accidente de aeronave.
- **fecha:** Fecha en la que ocurrió el accidente de aeronave.
- **HORA declarada:** Hora declarada del accidente de aeronave.
- **Ruta:** Ubicación geográfica donde ocurrió el accidente de aeronave.
- **OperadOR:** Compañía aérea operadora del vuelo.
- **flight_no:** Número de vuelo.
- **route:** Ruta de vuelo, indicando puntos de partida y destino.
- **ac_type:** Tipo de aeronave involucrada en el accidente.
- **registration:** Número de registro o número de serie de la aeronave.
- **cn_ln:** Número de construcción o número de línea de la aeronave.
- **all_aboard:** Número total de personas a bordo (pasajeros y tripulación).
- **PASAJEROS A BORDO:** Número total de pasajeros a bordo.
- **crew_aboard:** Número total de miembros de la tripulación a bordo.
- **cantidad de fallecidos:** Número total de personas fallecidas en el accidente (pasajeros y tripulación).
- **passenger_fatalities:** Número total de pasajeros fallecidos en el accidente.
- **crew_fatalities:** Número total de miembros de la tripulación fallecidos en el accidente.
- **ground:** Número total de personas en tierra fallecidas en el accidente.
- **summary:** Resumen del accidente de vuelo y circunstancias.

Después del proceso de ETL, que involucró la normalización de los nombres de las columnas, eliminación de duplicados, reemplazo de '?' por NaN, manejo de valores faltantes, corrección de errores tipográficos, cambios de tipo de datos según sea necesario y creación de columnas adicionales con información valiosa, obtuvimos el archivo [Accidentes_final.csv](Accidentes_final.csv).

### EDA: Análisis Exploratorio de Datos

En el archivo [EDA.ipynb](EDA.ipynb), realizamos un análisis estadístico y presentamos visualizaciones detalladas de los datos procesados. Esto incluyó análisis estadísticos y matrices de correlación para variables cuantitativas, así como varios tipos de visualizaciones que exploran relaciones y tendencias, como accidentes por año, país, operador de aerolínea, tipo de aeronave, categoría de vuelo y más. Además, realizamos análisis comparativos, exploración de variables y la identificación de valores atípicos.

### Panel de Visualización

El proyecto incluye un panel de visualización que muestra información visual resultante del análisis de datos previo. El panel consta de las siguientes secciones:

#### Resumen:

En esta sección, proporcionamos información general sobre accidentes de aviación, que incluye el número total de accidentes, fatalidades, sobrevivientes, la cantidad de accidentes por período y las principales aeronaves y operadores de aerolíneas con más accidentes.

#### KPIs Propuestos

1. KPI 1: Evaluar una reducción del 10% en la tasa anual global de accidentes durante los años 2002-2021.
2. KPI 2: Evaluar el aumento del 10% de la tasa de supervivencia en los últimos 10 años, comparado con la década anterior.

## Herramientas utilizadas
- Python
- Pandas
- Matplotlib
- Seaborn
- Power BI
