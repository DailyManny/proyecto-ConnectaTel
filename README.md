# Análisis de clientes ConnectaTel
Análisis del comportamiento de los clientes de ConnectaTel, empresa de telecomunicaciones en Latinoamérica, con datos hasta 2024. El objetivo es segmentar a los clientes por edad y nivel de uso para proponer estrategias de retención y mejoras en los planes

## Datasets
- `plans.csv`: 2 planes (Basico y Premium) con precio, minutos, GB y costos extra.
- `users_latam.csv`: 4,000 clientes con edad, ciudad, fecha de registro, plan y churn.
- `usage.csv`: 40,000 registros de llamadas y mensajes.

## Etapas del análisis
1.- Carga y exploración de los datos.
2.-Detección de problemas: nulos, sentinels (`age = -999`, `city = "?"`) y fechas imposibles (año 2026)
3.-Limpieza de datos
4.-Métricas de uso por usuario (mensajes, llamadas y minutos)
5.-Distribuciones y outliers (histogramas, boxplots, método IQR)
6.-Segmentación por uso (Bajo, Medio, Alto) y por edad (Joven, Adulto, Adulto Mayor)
7.-Conclusiones y recomendaciones para el negocio

## Hallazgos clave

- 74% de los clientes tiene uso medio, 19% bajo uso y 7% alto uso
- Ni la edad ni el plan explican el nivel de uso; conviene segmentar por comportamiento
- Premium no consume más que Basico, así que su valor depende del precio y los beneficios

## Cómo ejecutar
1. Abre `ConnectaTel_corregido.ipynb` en Jupyter 
2. Coloca los tres CSV en la ruta que usa el notebook (`/datasets/`) o ajusta las rutas en la celda de carga.
3. Ejecuta todo en orden: **Kernel, despues Restart Kernel and Run All Cells**.

Requisitos: Python, `pandas`, `seaborn`, `matplotlib`.

## Alumno
-Carlos Manuel Mata Rubio
