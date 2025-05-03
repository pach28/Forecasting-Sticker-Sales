# Forecasting Sticker Sales | Kaggle Competition Analysis

[![Kaggle](https://kaggle.com/static/images/site-logo.svg)](https://www.kaggle.com/competitions/demand-forecasting-for-a-sticker-company)

Este repositorio contiene el análisis y los notebooks desarrollados para la competencia "[Forecasting Sticker Sales](https://www.kaggle.com/competitions/demand-forecasting-for-a-sticker-company)" en Kaggle. El objetivo de la competencia fue predecir las ventas futuras de stickers para diferentes productos, basándose en datos históricos de ventas.

## Objetivo de la Competencia

El desafío principal consistió en construir un modelo de pronóstico preciso para la demanda de stickers, considerando la naturaleza de las series de tiempo, posibles estacionalidades, tendencias y la presencia de valores faltantes (NaNs) en los datos. Una predicción precisa de la demanda es crucial para la gestión de inventario, la planificación de la producción y la optimización de la cadena de suministro.

## Notebooks Incluidos

Este repositorio incluye los siguientes notebooks, que representan diferentes etapas del análisis y modelado:

1.  **`forecasting sticker sales Eda & classification plus ml model.ipynb`**:
    * **Análisis Exploratorio de Datos (EDA) Detallado:** Este notebook realiza una exploración exhaustiva de los datos de ventas. Se examinan las distribuciones de las ventas por producto, las tendencias temporales y la presencia de patrones.
    * **Segmentación por Histograma y Regresión:** Se observa una distinción visual en los histogramas de ventas de diferentes productos. Basándose en esta observación, los productos se clasifican en dos grupos. Posteriormente, se aplican modelos de regresión para intentar comprender las relaciones entre las variables y las ventas, considerando esta segmentación inicial.

2.  **`forecasting sticker sales NaN analysis & feat treatment.ipynb`**:
    * **Análisis del Comportamiento de los Valores Faltantes (NaN):** Este notebook se centra en el análisis de los valores faltantes en los datos de ventas. Se investiga el patrón de estos NaNs y se evalúan diferentes estrategias para su tratamiento.
    * **Ingeniería de Características (Feature Engineering):** Se implementan técnicas de codificación one-hot para manejar variables categóricas y se crean nuevas características que podrían ser relevantes para el modelado.
    * **Modelado Específico por Producto:** Dada la posible heterogeneidad en los patrones de demanda entre los diferentes productos, se exploran y aplican modelos de pronóstico individuales para cada producto. Esto permite capturar las características únicas de la serie de tiempo de cada sticker.

3.  **`sticker forecast kaggle stationary treatment & weighted sales.ipynb`**:
    * **Tratamiento Estacionario de NaNs:** Este notebook aborda el tratamiento de los valores faltantes considerando la naturaleza de la serie de tiempo. Se exploran métodos de imputación que tienen en cuenta la estacionalidad y las tendencias.
    * **Solución Ponderada de Características:** La solución final propuesta en este notebook implica una estrategia donde las predicciones se basan en una ponderación de diferentes características o modelos. Esto busca combinar la información de diversas fuentes para obtener un pronóstico más robusto y preciso.

## Cómo Utilizar este Repositorio

Para explorar el análisis y los modelos desarrollados, simplemente navega por los notebooks en este repositorio. Cada notebook está comentado para explicar el razonamiento detrás de cada paso y las técnicas aplicadas.
