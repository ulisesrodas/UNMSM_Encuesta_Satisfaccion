# Encuesta de satisfacción a estudiantes
Este repositorio presenta un ecosistema completo de Ciencia de Datos aplicada a la gestión universitaria. El proyecto automatiza la limpieza, informe y visualización de encuestas en torno a la satisfacción de la enseñanza recibida en el pregrado. Sus resultados se dividen en tres bloques:
* **Perfil del estudiante:** Se presentan las características inherentes a los integrantes de la facultad, como son Sexo, Nivel curricular cursado y Carrera elegida.
* **Satisfacción del estudiante:** Valoración de los servicios de la facultad (Plan de estudios, Infraestrucutra y Oportunidades laborales)
* **¿Por qué hay insatisfacción con los servicios?:** Se presenta como complemento a lo anterior. Aquí veremos las respuestas más frecuentes de por qué no están satisfechos los estudiantes con los servicios ofrecidos. Desde luego, esta insatisfacción tiene un sesgo negativo dado que solo analiza a los insatisfechos, pero da un excelente feedback a la facultad para saber áreas de mejoría.

## 📈 Hallazgos Clave del Análisis:
El informe revela dimensiones críticas que requieren atención inmediata:
* **Perfil de la Muestra**: Predominantemente femenina (62.2%) con una fuerte concentración en la Carrera 1 (46.3%).
* **Infraestructura (Prioridad Crítica)**: Es la dimensión con mayor insatisfacción (44.5%), principalmente por falta de laboratorios y espacios de estudio.
* **Brecha Académica:** Un 42.2% de insatisfacción en el Plan de Estudios debido a una percepción de clases "excesivamente teóricas".
* **Desafío Laboral:** Incertidumbre en empleabilidad (37.4% de insatisfacción), donde los estudiantes demandan mejores puentes con el mercado laboral y la red de egresados.

## 🚀 Secuencia de ejección
* Para ejecutar el proyecto, el archivo `CONOCIMIENTOS.xslx` debe estar en la carpeta local de trabajo. No se toca porque son los datos de los alumnos anonimizados en crudo.
* **SCRIPT.R:** Hace la limpieza lógica, consolidación de bases (Left Joins), cálculo de parámetros muestrales ($n=270$ con 95% de confianza) y tablas insumos.
* **INFORME.qmd:** Generación de un reporte con estética profesional utilizando Quarto, usando las tablas insumos del script anterior. Incluye visualizaciones de perfil demográfico y análisis de percepción.
* **AVANCE.pbix:** Modelado de datos para exploración interactiva en Power BI. Está de acuerdo como se solicita en el archivo xslx: con un corte para ver cómo avanza todo.

## 🛠️ Stack Tecnológico
* R & Quarto: tidyverse, kableExtra para tablas estilizadas, ggplot2 para gráficos de semáforo y stringr para manejo de textos cualitativos.
* Power BI: Modelado relacional y DAX para el dashboard interactivo.
* Metodología: Análisis de sentimientos/motivos mediante técnicas de text-wrapping en visualizaciones horizontales.
