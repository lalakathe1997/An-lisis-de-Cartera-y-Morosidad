📉 **Análisis de Riesgo de Cartera y Morosidad**
Dashboard desarrollado en Power BI para evaluar el comportamiento de la cartera de clientes, identificar niveles de riesgo y apoyar la gestión de cobro mediante el análisis de morosidad.

🎯 **Objetivo**
Medir el riesgo crediticio de la cartera de clientes, calcular métricas clave de mora y segmentar los clientes por nivel de riesgo, con el fin de facilitar decisiones estratégicas en la gestión de cobro.

📸 **Vista del dashboard**
adjunto en los archivos del repositorio

📌 **Principales hallazgos**

63.24% de la cartera se encuentra en mora — señal de alto riesgo crediticio
La morosidad se concentra en ciertas ciudades específicas, lo que permite focalizar esfuerzos de cobro
Se identificaron segmentos de clientes por nivel de riesgo (alto, medio, bajo)
El análisis permite priorizar la gestión de cobro sobre los clientes de mayor exposición


🗂️ **Contenido del repositorio**
ArchivoDescripciónAnálisis de riesgo de cartera y morosidad.pbixArchivo Power BI con el dashboard completoAnálisis de riesgo de cartera y morosidad.pdfExportación en PDF del dashboardCaptura de pantalla 2026-04-28 075353.pngVista previa del dashboard

📊 **Métricas calculadas**

Cartera total — Suma del saldo total de clientes activos
Cartera en mora — Saldo de clientes con pagos vencidos
Porcentaje de mora — Proporción de la cartera en estado de incumplimiento
Segmentación por riesgo — Clasificación de clientes según nivel de exposición


🔄 **Proceso de análisis**

Carga de datos desde Excel con información de clientes y saldos
Limpieza y transformación en Power Query (normalización de fechas, manejo de nulos, tipado de columnas)
Modelado de relaciones entre tablas
Creación de medidas DAX para KPIs de mora y segmentación
Visualización del dashboard con enfoque en riesgo y geografía


🛠️ **Herramientas utilizadas**

Power BI Desktop — Dashboard y visualizaciones interactivas
Power Query — Limpieza y transformación de datos
DAX — Cálculo de métricas de cartera y mora
Excel — Fuente de datos original


💡 **Medidas DAX destacadas**
dax-- Total de cartera
Cartera Total = SUM(Cartera[Saldo])

-- Cartera en mora
Cartera en Mora = 
CALCULATE(SUM(Cartera[Saldo]), Cartera[Estado] = "Mora")

-- Porcentaje de mora
% Mora = DIVIDE([Cartera en Mora], [Cartera Total])

👩‍💻 **Autora**
Laura Katherine Cuevas Alba
Data Analyst en formación | SQL · Python · Power BI
LinkedIn · GitHub
