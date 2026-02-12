# Analisis-Mora-Crediticia-2020-2021
Dashboard interactivo en Power BI sobre la evolución de la morosidad y riesgo crediticio en Argentina (2020-2021)

# Análisis de Riesgo Crediticio y Morosidad en Escenarios de Estrés (2020–2021)

---
# Descripción del proyecto

Este proyecto tiene como objetivo realizar un análisis exploratorio del riesgo crediticio, con foco en la morosidad y su concentración, utilizando datos correspondientes a los años 2020 y 2021, un período caracterizado por alta incertidumbre económica.
El análisis busca identificar patrones de riesgo, segmentar clientes y evaluar el impacto de la morosidad desde una perspectiva analítica, más allá de la visualización de datos.

---
# Objetivos del análisis

* Analizar el comportamiento de la morosidad en un contexto de estrés económico.
* Evaluar la severidad y frecuencia del riesgo crediticio.
* Identificar segmentos de clientes con mayor exposición al riesgo.
* Analizar la concentración geográfica y por canal de la morosidad.
* Brindar insights que puedan apoyar la gestión de cartera de crédito.

---
# Estructura de los datos

El dataset contiene información de aproximadamente 2.000 créditos, incluyendo variables:

* Demográficas (edad, género)
* Geográficas (provincia, ciudad)
* Crediticias (score crediticio, estado de mora)
* Temporales (año y mes)
* De negocio (línea de crédito, canal de solicitud)

---
# Enfoque analítico

El proyecto prioriza el pensamiento analítico por sobre la complejidad técnica, abordando el riesgo crediticio desde distintas dimensiones:
* Índice de morosidad como indicador principal de deterioro de cartera.
* Tramos de atraso para diferenciar mora temprana, crítica y cartera perdida.
* Análisis de monto vencido vs cantidad de clientes, distinguiendo severidad del riesgo.
* Comparación por canal de originación, producto y región.
* Análisis temporal para identificar tendencias y picos de riesgo.

---
# Modelado de datos

Se diseñó un modelo estrella utilizando Power Query y Power BI, separando:

* Tabla de hechos de morosidad
* Dimensiones de:
  * Tiempo
  * Cliente
  * Producto
  * Canal
  * Geografía

---
# Herramientas utilizadas

* Power BI
* Power Query
* Modelado dimensional (Modelo estrella)
* Análisis exploratorio de datos (EDA)

---
# Conclusiones generales

El análisis muestra que, durante los años 2020–2021, la morosidad presenta una alta concentración en tramos de atraso severos, lo que indica un riesgo elevado de pérdida.
Asimismo, se observan diferencias relevantes según canal, región y producto, lo que sugiere oportunidades para políticas de crédito diferenciadas.
