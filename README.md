# P9.Showz_MarketingAnalytics

## 📌 Descripción breve

Análisis de negocio para Showz (venta de entradas). Objetivo: medir comportamiento de usuarios, calcular LTV y CAC por canal, y recomendar dónde invertir el presupuesto de marketing.

## 📂 Datasets

/datasets/visits_log_us.csv — sesiones: uid, device, start_ts, end_ts, source_id.

/datasets/orders_log_us.csv — pedidos: uid, buy_ts, revenue.

/datasets/costs_us.csv — gastos marketing: source_id, dt, costs.

## 🎯 Objetivos principales

Preparar y optimizar los datos para análisis.

Calcular métricas clave: usuarios activos (día/semana/mes), sesiones, duración de sesión, retención.

Analizar ventas: time-to-first-purchase (conversion lag), número/patterns de pedidos, ticket promedio, LTV.

Marketing: gasto total y por fuente, CAC por fuente, ROMI (o ROAS).

Visualizar resultados por dispositivo y por fuente; recomendar dónde invertir.

## 🧭 Estructura sugerida del notebook

Carga y revisión: leer CSVs, head(), info(), tipos de datos.

Preprocesamiento:

Convertir timestamps, calcular session_duration.

Normalizar source_id.

Manejar duplicados y missing.

Métricas de visitas:

Usuarios por día/semana/mes.

Sesiones por día y duración media.

Retención/cohortes (time-to-return).

Análisis de ventas:

Time-to-first-purchase (Conversion 0d, 1d, …).

Pedidos por usuario y ticket promedio.

LTV (por cohortes y por fuente).

Marketing & ROI:

Costos por fuente y periodo.

CAC = (costos por fuente) / (nuevos clientes por fuente).

ROMI = (ingresos atribuibles − costos) / costos.

Visualizaciones:

Series temporales, barras comparativas, cohort heatmaps.

Conclusión y recomendaciones:

Fuentes y dispositivos prioritarios para invertir.

KPIs a monitorear regularmente.

## 📈 Métricas clave a reportar

Usuarios activos diarios/semanales/mensuales (DAU/WAU/MAU).

Sesiones por usuario y duración media.

Conversion lag (días hasta 1ª compra) por cohorte y canal.

Ticket promedio y LTV por cohorte/canal.

CAC y ROMI por fuente de adquisición.
## 🛠 Herramientas recomendadas

Python (Pandas, NumPy), Matplotlib/Seaborn, Jupyter Notebook.

Opcional: Plotly para gráficos interactivos.
