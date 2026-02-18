

# Análisis de Riesgo Crediticio y Morosidad en Escenarios de Estrés (2020–2021)

---
# Descripción del proyecto

Este proyecto tiene como objetivo realizar un análisis exploratorio del riesgo crediticio, con foco en la morosidad y su concentración, utilizando datos correspondientes a los años 2020 y 2021, un período caracterizado por alta incertidumbre económica.
El análisis busca identificar patrones de riesgo, segmentar clientes y evaluar el impacto de la morosidad desde una perspectiva analítica, más allá de la visualización de datos. Como Analista Junior, mi enfoque no fue solo reportar el índice de morosidad, sino identificar los segmentos de mayor riesgo y proyectar el impacto económico de una nueva estrategia de admisión mediante Forecasting.

---
# Objetivos del análisis

* Analizar el comportamiento de la morosidad en un contexto de estrés económico.
* Evaluar la severidad y frecuencia del riesgo crediticio.
* Identificar segmentos de clientes con mayor exposición al riesgo.
* Analizar la concentración geográfica y por canal de la morosidad.
* Brindar insights que puedan apoyar la gestión de cartera de crédito.


---
# Enfoque analítico

El proyecto prioriza el pensamiento analítico por sobre la complejidad técnica, abordando el riesgo crediticio desde distintas dimensiones:
* Índice de morosidad como indicador principal de deterioro de cartera.
* Tramos de atraso para diferenciar mora temprana, crítica y cartera perdida.
* Análisis de monto vencido vs cantidad de clientes, distinguiendo severidad del riesgo.
* Comparación por canal de originación, producto y región.
* Análisis temporal para identificar tendencias y picos de riesgo.


---
# Herramientas utilizadas

* Power BI
* Power Query
* Modelado dimensional (Modelo estrella)
* Análisis exploratorio de datos (EDA)

---
# Principales insights y recomendaciones

* Concentración de mora en tramos > 90 días:
  
     Se identifica que una parte relevante del monto en mora se concentra en atrasos severos, indicando riesgo elevado de incobrabilidad. **Recomendación**: reforzar alertas tempranas y acciones preventivas antes de los 60 días de atraso.
* Impacto del contexto 2020–2021 en la morosidad:

  El período analizado muestra niveles elevados de morosidad asociados a un contexto económico adverso. **Recomendación**: utilizar estos datos como escenario de stress testing y ajustar criterios de otorgamiento.
* Mejora interanual en la cantidad de clientes en mora:

  Se observa una reducción de clientes morosos respecto al año anterior. **Recomendación**: replicar prácticas de originación y gestión que mostraron mejor desempeño.
* Diferencias de riesgo por producto y línea de crédito:

  Algunas líneas concentran mayor proporción de cartera vencida.**Recomendación**: revisar condiciones de otorgamiento y límites crediticios por producto.
* Concentración geográfica del riesgo:

  La morosidad no se distribuye de forma homogénea entre regiones.**Recomendación**: ajustar políticas de crédito considerando variables geográficas.

  ---
  # Análisis Predictivo y Estratégico:

  1.**Escenarios de Evolución de Mora (Forecast a 6 meses)**:
  * **Horizonte de Predicción**: Implementé una proyección de 6 meses para priorizar la exactitud estadística. En el sector financiero, los pronósticos a corto plazo permiten una reacción más ágil ante la volatilidad del mercado.
  * **Gestión de Incertidumbre**: Utilicé un intervalo de confianza del 95% para visualizar escenarios probables de riesgo. En el segmento de Score Bajo, la amplitud de la sombra de incertidumbre justifica la necesidad de una intervención urgente.
  * **Insight de Negocio**: El modelo identifica que los próximos dos trimestres son críticos para estabilizar la cartera y evitar que la tendencia alcista impacte el flujo de caja.

  2. **Medida de Impacto: "Optimización de Cartera" (Ahorro Estimado)**: Para hablar el lenguaje de negocio, creé una medida DAX personalizada que cuantifica el éxito de una posible intervención técnica:
  * **Lógica**: Si se reduce la exposición en los Scores 1 y 2 (donde la mora supera el 50%) en un 20%, ¿cuánto capital protegemos?
  * **Resultado**: Identifiqué un Ahorro Potencial de $4.65 millones, permitiendo al área de riesgos visualizar el beneficio económico de endurecer las políticas de admisión.

  ---
  # Conclusiones y Propuesta de Valor:

  * **Identificación de Riesgo**: El segmento "Cliente Bajo" posee un índice de morosidad del 51.4%, lo que requiere una acción de mitigación inmediata.
  * **Estrategia recomendada** : Utilizar el forecast semestral como ventana de oportunidad para ajustar los límites de crédito en los sectores de mayor riesgo.
  * **Impacto Fianl** : Este proyecto muestra cómo el análisis de datos ayuda a la empresa a tomar mejores decisiones. Gracias a este dashboard, podemos identificar a tiempo qué clientes tienen más riesgo de no pagar y actuar rápido. El resultado es un ahorro real de $8.3 millones (Score 1 y 2 ), dinero que la empresa deja de perder al ser más precavida con sus préstamos.

---
# Plan de Acción Basado en Insights : 
1. **Ajuste Dinámico de Políticas de Admisión (Filtros de Entrada)** :
* **La Acción** : Endurecer los requisitos para los segmentos identificados como Score 1 y 2.
* No se trata de rechazar a todos los clientes, sino de elevar el "piso" de entrada. Por ejemplo, si un "Cliente Bajo" antes calificaba con un ingreso mínimo de $500, la nueva política exigiría $850.
* **Objetivo** : Filtrar a los candidatos con mayor probabilidad de default antes de que el crédito sea otorgado, reduciendo la entrada de nueva mora.

2. **Recalibración de Límites de Crédito** :
* **La Acción**: Implementar una reducción proactiva en las líneas de crédito para los perfiles de riesgo alto.
* Si el modelo detecta que un cliente pertenece al segmento con un Índice de Morosidad del 51.4%, el sistema reduciría automáticamente su límite de crédito disponible (ej. de $1,000 a $400).
* ** Obejetivo** : Al disminuir la exposición financiera por cliente, el impacto económico en caso de impago es significativamente menor, materializando el Ahorro Estimado de $8.3 M.

3. ** Implementación de un Sistema de "Alerta Temprana"**:
* ** La Acción** : Usar el Forecast de 6 meses para disparar campañas de cobranza preventiva.
* Dado que el forecast identifica meses con tendencias alcistas, el área de cobranzas puede iniciar contactos recordatorios con los clientes de Score Regular/Bajo antes de que venzan sus cuotas en esos periodos críticos.
* **Objetivo** : Adelantarse a la curva de impago proyectada, utilizando los datos predictivos para optimizar el esfuerzo del equipo de operaciones de cobranza.
