# 📞 ConnectaTel: Optimización de Oferta Comercial y Detección de Anomalías de Uso

> **Enfoque de Negocio:** Análisis cuantitativo de patrones de consumo para reducir la fricción en la experiencia del cliente, detectar desviaciones operativas/fraude y maximizar el margen de beneficio por usuario (ARPU).

---

## 💼 Problema de Negocio

En la industria de las telecomunicaciones en LATAM (México y Colombia), **ConnectaTel** enfrenta dos desafíos comerciales críticos:
1. **Ineficiencia en la oferta de planes:** Diseñar paquetes tarifarios sin entender el comportamiento real del usuario genera insatisfacción, riesgo de migración de clientes (*churn*) y pérdida de ingresos por cobros excedentes no optimizados.
2. **Riesgo operativo y anomalías:** Registros atípicos de consumo (llamadas de duración cero, picos extremos de mensajes o datos) representan posibles fallas de facturación, uso fraudulento o errores en los sistemas de captura de datos.

**Pregunta Estratégica:** ¿Cómo podemos segmentar a los usuarios según su patrón real de uso para rediseñar la oferta comercial y neutralizar anomalías de registros antes de que afecten la rentabilidad?

---

## 🎯 Objetivos de la Investigación

* **Diagnóstico de Patrones de Consumo:** Analizar la distribución de minutos y mensajes para identificar brechas entre las cuotas contratadas y el uso real.
* **Detección de Anomalías y Outliers:** Aislar sesgos de medición (como valores *sentinel* o tráfico atípico) para garantizar la calidad del dataset y prevenir discrepancias en facturación.
* **Segmentación Estratégica:** Agrupar clientes bajo reglas de negocio específicas para adaptar campañas de *upselling* o *cross-selling*.
* **Recomendaciones Ejecutivas:** Proporcionar al equipo comercial guías basadas en datos para el diseño de planes de nueva generación.

---

## 📊 Arquitectura de Datos

El análisis integra tres fuentes de información operativa y demográfica:

* `plans.csv`: Estructura financiera de planes (precios base, límites de minutos/mensajes y tarifas por consumo excedente).
* `users_latam.csv`: Atributos demográficos de clientes (edad, ciudad, fecha de alta y plan suscrito).
* `usage.csv`: Registros transaccionales de uso real (duración de llamadas y volumen de mensajes enviados).

---

## 🛠️ Metodología y Flujo de Trabajo

El proyecto implementa un pipeline analítico riguroso para asegurar la confiabilidad de los hallazgos:

1. **Gobernanza y Calidad de Datos:** Identificación y tratamiento de valores nulos, registros duplicados, valores *sentinel* y estandarización de formatos temporales.
2. **Tratamiento de Outliers y Estadística Descriptiva:** Análisis de dispersión y tendencias centrales mediante diagramas de caja (*boxplots*) e histogramas para definir límites operativos normales.
3. **Segmentación y Agrupación por Negocio:** Categorización de usuarios mediante reglas condicionales y visualización de proporciones con `countplots`.
4. **Modelado de Recomendaciones:** Traducción de métricas estadísticas en iniciativas comerciales accionables para la toma de decisiones.

---

## 🚀 Herramientas Utilizadas

* **Entorno:** Jupyter Notebook
* **Lenguaje:** Python
* **Librerías Analíticas:** `pandas`, `numpy`
* **Visualización:** `seaborn`, `matplotlib`

---
## 💻 Cómo ejecutar el Notebook
Para visualizar y ejecutar el análisis, se recomienda el uso de **Google Colab** por su facilidad para manejar entornos de Python:

1.  Accede a [https://colab.research.google.com/github/gabrielabustamantealarcon/telecom-analysis/blob/main/S7_Version_Estudiante_Project_ConnectaTel.ipynb#scrollTo=1a87415b]
2.  Ejecuta las celdas secuencialmente presionando `Shift + Enter`.

## 🛠️ Guía de Reproducción
Para replicar este análisis en un entorno local:
1.  **Clonar el repositorio** o descargar los archivos fuente.
2.  **Ejecución:** Abre tu editor preferido (Jupyter Notebook, VS Code o PyCharm) y corre el script completo para generar los gráficos y el reporte final.
