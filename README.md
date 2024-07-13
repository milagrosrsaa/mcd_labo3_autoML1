Este repositorio corresponde al equipo de AutoML1 de la materia Laboratorio de Implemenetación III de la maestría en Ciencia de Datos de la Universidad Austral, cohorte 2022 virtual. El mismo contiene los datasets de entrada y salida, en conjunto con los experimentos de modelado, para la competencia de Kaggle de la materia, vinculada con un problema de forecasting para una empresa de consumo masivo comercializadora de productos de diversa indole. 

El equipo AutoML1 se centró en la especialidad AutoML, en particular la subespecialidad de pruebas con AWS Forecast, DARTS y AutoGluon. Dado que las librerias de AutoML tienen poco margen para pruebas sobre el modelado en sì, los experimentos se vincularon mayoritariamente con pruebas de:
- Mejor forma de agrupamiento de los datos
- Feature Engineering
- Preprocesamiento de tipo clustering para detectar patrones de series

Sobre la estructura del repositorio:
- EDA y armado datasets; contiene analisis exploratorio de los datos y la notebook en donde se generaron los datasets input del modelo
- DARTS: modelos de DARTS
- AWS Forecast: modelos de AWS Forecast
- AutoGluon: modelos de AutoGluon
- Datasets: data cruda y preprocesada (output de punto 1), inputs para los modelos
- Outputs: salidas cargadas a Kaggle

Resumen de principales Experimentos:


|Exp|	Descripcción	|Kaggle |
|---|---|------|
|1	|**Mejor modelo en el public leaderboard:** [Modelo básico (no incluye data de productos ni relacionada)](https://github.com/milagrosrsaa/mcd_labo3_autoML1/blob/main/4.%20AutoGluon/Exp1%20Modelo%20b%C3%A1sico.ipynb)	|0.245|
|2	|Modelo básico - 3 periodos val|    0.249|
|2	|V1. Idem 2 pero con datos desde 2018|	0.261|
|2	|V3. Idem 2 pero customizando función de error|	0.251|
|2	|V4. Idem 2 acotando outliers inferiores y superiores|	0.249|
|2	|**Modelo elegido por el equipo:** [V5. Idem 2 acotando outliers superiores 0.95](https://github.com/milagrosrsaa/mcd_labo3_autoML1/blob/38bc157e75a84e3929e08a5d49b5d1a93b4f9380/4.%20AutoGluon/Exp2_v5%20Modelo%20b%C3%A1sico%20+%20Ventana%20validaci%C3%B3n%20-%20Acotar%20outliers%20sup.ipynb)|	0.247|
|2	|V5_1. Idem EXP2 V5 aumentando validación a 6 ventanas|	0.255|
|2	|V6. Idem 2 acotando outliers superiores 0.90|	0.256|
|3	|Modelo básico - 3 periodos  val - Optimización hiperparametros|	0.277|
|4	|Modelo con data de productos|	0.263|
|4	|V1. Idem 4 pero con target acotado y data productos con corr|	0.263|
|5	|Modelo completo - 3 periodos val|	0.27|
|6	|Modelo completo (nuevos features relacionados) - 3 periodos val|	0.321|
|7	|Modelo básico - Nivel producto-cluster cliente|	0.26|
|8	|Modelo básico - Data estandarizada|	0.5|
|9	|Modelo básico - Uso modelos pre-entrenados de Chronos|	0.29|
|10	|Modelo básico - 7 clusters de series|	0.29|
|11	|Modelo básico - Predicción por cat2|	0.263|
|12	|Modelo básico - Clustering completo de productos|	0.268|
|13	|Modelo básico - Clustering completo de productos 10 clusters|	0.257|
|13	|V1. Idem 13 pero solo cluster de series, 10 clusters|	0.285|
|13	|V2. Idem 13 considerando 20 cluster de series, 30 clusters finales|	0.273|
|14	|Modelo completo - Target acotado, nueva data producto y relacionada|	0.314|
|14	|V1. Optimizando TFT|	0.364|
|15	|Modelo completo - Target acotado, nueva data producto y relacionada - Cluster 10 series|	0.307|
|16	|Idem 13 pero con target acotado por outliers|	0.27|
|17	|Idem 13_v1 pero con target acotado y 25 clusters|	0.283|


Integrantes del equipo AutoML1:
- Garcia Matias
- Martignoni Franco
- Rodriguez Saa Milagros