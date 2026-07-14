# ⚡ EcoEnergy Solutions — Análisis Exploratorio de Datos Energéticos

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
- `EcoEnergy_EDA.ipynb` — notebook con el flujo completo de EDA: carga
  automática del dataset (sin pasos manuales), limpieza, chequeos de
  calidad, estadísticas descriptivas y visualizaciones, cada una con su
  justificación metodológica. Ejecutable de principio a fin con
  "Run All".
- `Documentacion_EcoEnergy_Solutions.pdf` — informe metodológico completo
  (objetivo, metodología, calidad de datos, estadísticas). 3 páginas.
- `Informe.pdf` — exportación del dashboard interactivo (Looker Studio) con
  los KPIs y gráficos principales. 1 página.

## Dashboard en vivo

El panel interactivo de Looker Studio está disponible en:
https://datastudio.google.com/reporting/1e696b98-a484-48bb-bc27-ee921e66d459

> ⚠️ Verificar que el enlace tenga permisos de "Cualquier persona con el
> enlace puede ver" antes de compartirlo para revisión.

## 🚀 Mejoras a futuro

- Automatizar la actualización del dashboard si en el futuro se dispone de
  datos reales y no solo del snapshot estático actual.
- Reemplazar la URL de carga del CSV en el notebook por la definitiva una
  vez subido el proyecto a GitHub (ver primera celda de código).
