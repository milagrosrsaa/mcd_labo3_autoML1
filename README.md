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

Integrantes del equipo AutoML1:
- Garcia Matias
- Martignoni Franco
- Rodriguez Saa Milagros