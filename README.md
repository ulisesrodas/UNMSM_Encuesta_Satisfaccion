# Encuesta de satisfacción a estudiantes
Este repositorio presenta un ecosistema completo de Ciencia de Datos aplicada a la gestión universitaria. El proyecto automatiza el procesamiento de encuestas de satisfacción a estudiantes de una facultad de la UNMSM, transformando datos crudos en un informe dinámico (Quarto) y un dashboard interactivo (Power BI) en torno a, principalmente, a la satisfacción o no de tres temáticas:
* Plan de estudios.
* Infraestructura.
* Oportunidades laborales.

La base de datos cruda es el archivo `CONOCIMIENTOS.xslx`. Está anonimizada, pero ello no quita fuerza al análisis ni las conclusiones. Para que corra el archivo `SCRIPT.R`, el Excel debe estar en la misma carpeta local.

## 📈 Hallazgos Clave del Análisis:
El informe revela dimensiones críticas que requieren atención inmediata:
* **Perfil de la Muestra**: Predominantemente femenina (62.2%) con una fuerte concentración en la Carrera 1 (46.3%).
* **Infraestructura (Prioridad Crítica)**: Es la dimensión con mayor insatisfacción (44.5%), principalmente por falta de laboratorios y espacios de estudio.
* **Brecha Académica:** Un 42.2% de insatisfacción en el Plan de Estudios debido a una percepción de clases "excesivamente teóricas".
* **Desafío Laboral:** Incertidumbre en empleabilidad (37.4% de insatisfacción), donde los estudiantes demandan mejores puentes con el mercado laboral y la red de egresados.

## 🚀 Flujo de trabajo integrado
El proyecto no solo limpia datos, sino que genera productos de valor para la toma de decisiones:
* Motor de Procesamiento (R): Limpieza lógica, consolidación de bases (Left Joins) y cálculo de parámetros muestrales ($n=270$ con 95% de confianza).
* Informe Automatizado (INFORME.qmd): Generación de un reporte con estética profesional utilizando Quarto, que incluye visualizaciones de perfil demográfico y análisis de percepción.
* Visualización (AVANCE.pbix): Modelado de datos para exploración interactiva en Power BI. **[VER DASHBOARD]]**

## 🛠️ Stack Tecnológico
* R & Quarto: tidyverse, kableExtra para tablas estilizadas, ggplot2 para gráficos de semáforo y stringr para manejo de textos cualitativos.
* Power BI: Modelado relacional y DAX para el dashboard interactivo.
* Metodología: Análisis de sentimientos/motivos mediante técnicas de text-wrapping en visualizaciones horizontales.
