Este proyecto forma parte de la estrategia de análisis de datos de **ConnectaTel**, empresa de telecomunicaciones líder con operaciones en México y Colombia. El objetivo principal es transformar datos de uso crudos en conocimiento accionable para optimizar la oferta comercial y mejorar la experiencia del usuario.

## 🎯 Objetivo del Proyecto
El propósito central es entender cómo los clientes utilizan realmente los servicios móviles (llamadas y mensajes). A través de este análisis, se busco:
* **Identificar patrones de uso:** Determinar tendencias generales de consumo.
* **Detección de anomalías:** Localizar comportamientos atípicos que sugieran fraude, errores de registro o necesidades extremas.
* **Segmentación de clientes:** Diferenciar grupos de usuarios para personalizar la oferta comercial.
* **Optimización:** Brindar recomendaciones basadas en datos para el diseño de nuevos planes.

## 📊 Datasets Utilizados
El análisis se basa en tres fuentes de datos integradas:
1.  **`plans.csv`**: Catálogo de planes vigentes, incluyendo precios mensuales, cuotas de minutos/GB y costos por consumos excedentes.
2.  **`users_latam.csv`**: Base de datos de clientes con atributos demográficos (edad, ciudad), fecha de registro y el plan suscrito.
3.  **`usage.csv`**: Registro detallado de la actividad real, conteniendo la duración de las llamadas y la longitud de los mensajes enviados.

## 🚀 Etapas del Análisis
El proyecto sigue un flujo de trabajo estructurado para garantizar la integridad de los resultados:
1.  **Carga y Exploración:** Lectura inicial de los datos y revisión de estructuras.
2.  **Identificación de Calidad:** Detección de valores nulos, valores centinela (sentinels) y validación de rangos de fechas.
3.  **Limpieza de Datos:** Tratamiento de valores faltantes, conversión de tipos de datos y corrección de inconsistencias.
4.  **Estadística Descriptiva:** Cálculo de medidas de tendencia central y dispersión para variables clave.
5.  **Análisis de Outliers:** Uso de histogramas y diagramas de caja (boxplots) para identificar valores extremos.
6.  **Segmentación:** Agrupación de usuarios bajo reglas de negocio y visualización de proporciones mediante *countplots*.
7.  **Insights Ejecutivos:** Generación de conclusiones estratégicas y recomendaciones para la toma de decisiones.

## 💻 Cómo ejecutar el Notebook
Para visualizar y ejecutar el análisis, se recomienda el uso de **Google Colab** por su facilidad para manejar entornos de Python:

1.  Accede a [https://colab.research.google.com/drive/1mVwwQMjEuVqwG1X5FudntV-itt4kV8oM]
2.  Ejecuta las celdas secuencialmente presionando `Shift + Enter`.

## 🛠️ Guía de Reproducción
Para replicar este análisis en un entorno local:
1.  **Clonar el repositorio** o descargar los archivos fuente.
2.  **Ejecución:** Abre tu editor preferido (Jupyter Notebook, VS Code o PyCharm) y corre el script completo para generar los gráficos y el reporte final.
