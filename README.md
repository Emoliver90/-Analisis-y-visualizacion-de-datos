⚡ EcoEnergy Solutions — Análisis Exploratorio de Datos Energéticos

Proyecto de análisis exploratorio de datos (EDA) para un cliente ficticio,
**EcoEnergy Solutions**, empresa europea de energías renovables y eficiencia
energética. El objetivo es explorar el consumo energético de sus clientes
para identificar patrones de uso, factores de coste, comportamiento emisor
de CO₂ y oportunidades de optimización.

## Dataset

`ecoenergy-consumption-data.csv` contiene registros de clientes con los
campos: `client_id`, `client_name`, `region`, `contract_type`,
`consumption_kwh`, `billing_date`, `co2_emissions`, `cost_per_kwh`,
`total_cost` y `renewable_energy_percentage`.

`ecoenergy_clean.csv` es el resultado del proceso de limpieza, con una
columna adicional `mes` (agregación mensual de `billing_date`) para facilitar
el análisis de evolución temporal.

## Metodología

1. **Carga e inspección inicial:** forma del dataset, tipos de datos,
   valores nulos y duplicados.
2. **Limpieza:** conversión de `billing_date` a un formato de fecha válido y
   verificación de los tipos numéricos.
3. **Calidad de datos:** detección de valores negativos, categorías
   inconsistentes y fechas inválidas.
4. **Estadísticas descriptivas:** media, mediana, desviación estándar,
   mínimos y máximos de las cinco variables clave (consumo, emisiones,
   coste, coste por kWh, % renovable).
5. **Visualización e informe:** construcción de un dashboard interactivo en
   Looker Studio y un informe formal en PDF con los hallazgos.

## Hallazgos principales (ver dashboard/informe para el detalle completo)

- Consumo total agregado, consumo promedio, emisiones totales de CO₂, coste
  total, coste promedio por kWh y porcentaje renovable promedio a nivel
  global.
- Desglose de consumo por región, emisiones por tipo de contrato
  (residencial vs. comercial) y evolución mensual del consumo a lo largo del
  año.
- Ranking de clientes por consumo total, con su porcentaje de energía
  renovable asociado.

## Entregables

- `ecoenergy-consumption-data.csv` — dataset original.
- `ecoenergy_clean.csv` — dataset limpio con la columna `mes` añadida.
- `Documentacion_EcoEnergy_Solutions.pdf` — informe metodológico completo
  (objetivo, metodología, calidad de datos, estadísticas).
- `Informe.pdf` — exportación del dashboard interactivo (Looker Studio) con
  los KPIs y gráficos principales.

## 🚀 Mejoras a futuro

- Incluir el notebook de Google Colab usado para el análisis, no solo los
  informes exportados, para que el proceso sea totalmente reproducible.
- Enlazar el dashboard de Looker Studio en vivo (URL pública) además de la
  captura en PDF, para que se pueda interactuar con los filtros.
- Añadir un análisis de correlación entre `renewable_energy_percentage` y
  `cost_per_kwh` para cuantificar si la energía renovable resulta más cara o
  más barata para el cliente en este dataset.
- Automatizar la actualización del dashboard si en el futuro se dispone de
  datos reales y no solo del snapshot estático actual.
la de carbono.

