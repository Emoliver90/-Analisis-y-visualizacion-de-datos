# -Analisis-y-visualizacion-de-datos
El presente análisis tiene como objetivo explorar el conjunto de datos de consumo energético de sus clientes para
identificar patrones de uso, factores de coste, comportamiento emisor y oportunidades concretas de
optimización y reducción de huella de carbono.
## Proceso de análisis
#### Carga e inspección inicial: forma del dataset, tipos de datos, valores nulos y duplicados.
#### Limpieza: conversión de billing_date a formato fecha válido; verificación de tipos numéricos.
#### Calidad de datos: detección de valores negativos, categorías inconsistentes y fechas inválidas.
#### Estadísticas descriptivas: media, mediana, desviación estándar, mínimos y máximos de las cinco variables clave.
#### Análisis segmentado: comparación de métricas por región y tipo de contrato.
#### Correlaciones: matriz de Pearson y heatmap para identificar relaciones entre variables.
#### Detección de outliers: método IQR (rango intercuartílico) aplicado a consumo, emisiones, coste y renovables.
#### Tendencia temporal: agrupación mensual del consumo para identificar patrones estacionales.
#### Visualizaciones: gráficos de barras, dispersión, boxplots, histogramas y línea temporal.
## Herramientas utilizadas
Google Colab · Python 3 · pandas · matplotlib · seaborn · Google Looker Studio.
