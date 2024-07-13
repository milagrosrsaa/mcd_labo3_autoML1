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

|Exp	|Descripcción	|Error Val	|Kaggle |
|---|---|---|------|
|1	|[Modelo básico (no incluye data de productos ni relacionada)](https://github.com/milagrosrsaa/mcd_labo3_autoML1/blob/main/4.%20AutoGluon/Exp1%20Modelo%20b%C3%A1sico.ipynb)	|0.1760	|0.245|
|2	|[Modelo básico - 3 periodos val](https://github.com/milagrosrsaa/mcd_labo3_autoML1/blob/38bc157e75a84e3929e08a5d49b5d1a93b4f9380/4.%20AutoGluon/Exp2%20Modelo%20b%C3%A1sico%20+%20Ventana%20validaci%C3%B3n.ipynb)	|0.1819	|0.249|
|3	|[Modelo básico - 3 periodos  val - Optimización hiperparametros](https://github.com/milagrosrsaa/mcd_labo3_autoML1/blob/38bc157e75a84e3929e08a5d49b5d1a93b4f9380/4.%20AutoGluon/Exp3%20Modelo%20b%C3%A1sico%20+%20Optimizaci%C3%B3n%20hiperparametros.ipynb)	|0.1733	|0.277|
|4	|[Modelo con data de productos](https://github.com/milagrosrsaa/mcd_labo3_autoML1/blob/38bc157e75a84e3929e08a5d49b5d1a93b4f9380/4.%20AutoGluon/Exp4%20Modelo%20con%20data%20de%20productos.ipynb)	|0.1779	|0.263|
|5	|[Modelo completo - 3 periodos val](https://github.com/milagrosrsaa/mcd_labo3_autoML1/blob/38bc157e75a84e3929e08a5d49b5d1a93b4f9380/4.%20AutoGluon/Exp5%20Modelo%20con%20data%20de%20productos%20+%20relacionada%20(completo).ipynb)	|0.1754	|0.27|
|6	|Modelo completo (nuevos features relacionados) - 3 periodos val	|0.05	|0.321|
|7	|Modelo básico - Nivel producto-cluster cliente	|0.2126	|0.26|
|8	|Modelo básico - Data estandarizada	|0.51	|-|
|9	|Modelo básico - Uso modelos pre-entrenados de Chronos	|-	|0.29|
|10	|Modelo básico - 7 clusters de series	|<20 salvo 1 cluster	|0.29|
|11	|Modelo básico - Predicción por cat2	|	|0.263|
|12	|Modelo básico - Clustering completo de productos	|	|0.268|


Integrantes del equipo AutoML1:
- Garcia Matias
- Martignoni Franco
- Rodriguez Saa Milagros