# Ecommerce Growth & A/B Testing Analysis
🧠 Contexto

Como analista en una tienda online, el departamento de marketing recopiló una serie de hipótesis para aumentar los ingresos del negocio.
El proyecto tiene como objetivo:

Priorizar hipótesis mediante métodos cuantitativos

Seleccionar la más prometedora

Ejecutar una prueba A/B comparando la landing actual vs. mejorada

Analizar resultados con métricas de negocio y significancia estadística

Tomar una decisión basada en evidencia

🥇 Parte 1 — Priorización de hipótesis (ICE & RICE)

Se utilizó el archivo hypotheses_us.csv, que contiene:

Alcance

Impacto

Confianza

Esfuerzo

Se aplicaron las fórmulas:

ICE = Impacto × Confianza / Esfuerzo
RICE = Alcance × Impacto × Confianza / Esfuerzo

📌 Resultado
RICE permitió identificar con mayor claridad la hipótesis con mejor retorno previsto por el tamaño de audiencia.
Esa hipótesis fue seleccionada para ejecutar el experimento.

🧪 Parte 2 — Análisis del test A/B

La prueba dividió a los usuarios:

A – versión original

B – versión con mejora sugerida

Se analizaron las métricas utilizando orders_us.csv y visits_us.csv.

🔍 Análisis realizado

Métricas principales

Ingresos acumulados por grupo

Tamaño de pedido promedio acumulado

Diferencia relativa en ticket y conversión

Tasa de conversión por usuario

Distribución y calidad de datos

Dispersión de pedidos por usuario

Dispersión de ingresos por pedido

Identificación de outliers (percentil 95 y 99)

Definición de umbral para anomalías

Significancia estadística
Se evaluó la diferencia entre grupos:

Ticket promedio (datos crudos)

Conversión (datos filtrados)

Ticket promedio (datos filtrados)

🎯 Conclusiones del experimento

📌 Hallazgos clave

El grupo B obtuvo mayores ingresos acumulados

El ticket promedio fue consistentemente superior en B

La tasa de conversión también favoreció a B

La significancia estadística confirmó que estas diferencias no son aleatorias

Tras filtrar valores atípicos, el grupo A mejora ligeramente, pero B sigue siendo más sólido

📌 Decisión final
Parar la prueba y seleccionar el grupo B como ganador.

📌 Justificación

Consistencia en ingresos y ticket promedio

Conversión superior

Significancia estadística favorable

Tendencia estable al cierre del experimento

📌 Consideraciones adicionales
El grupo A mostró crecimiento y mejora después del filtrado, lo que sugiere que:

La hipótesis beneficia a usuarios de mayor valor

Podrían explorarse variantes futuras para distintos segmentos

🚀 Próximos pasos recomendados

Extender despliegue del grupo B a toda la plataforma

Ejecutar pruebas para nuevos segmentos / variantes UI

Investigar comportamiento de usuarios excluidos por outliers

Medir impacto en métricas a más largo plazo (LTV, CAC, retención)

🧰 Tecnologías utilizadas

Python · Pandas · NumPy · SciPy
Matplotlib · Seaborn
Jupyter Notebook
