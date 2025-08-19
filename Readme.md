# Proyecto: TelecomX2 LATAM

## Descripción

Este proyecto da continuidad al análisis de evasión de clientes
(**Churn**) en **TelecomX LATAM**, ahora enfocado en la construcción de
**modelos predictivos** capaces de anticipar qué clientes tienen mayor
probabilidad de cancelar sus servicios.

Se preparó un pipeline de **preprocesamiento, modelado y evaluación**
para identificar variables críticas y proponer estrategias de retención.

------------------------------------------------------------------------

## Preparación de Datos

-   **Eliminación de columnas irrelevantes**, como identificadores
    únicos.\
-   **Codificación (Encoding)** de variables categóricas a numéricas.\
-   **Verificación de la proporción de cancelación**, encontrando un
    desbalance moderado entre clientes que permanecen y los que
    cancelan.\
-   **Balanceo de clases** con técnicas de oversampling en escenarios de
    fuerte desbalance.\
-   **Normalización/Estandarización** aplicada solo en modelos sensibles
    a la escala (KNN, Regresión Logística).\
-   **Selección de variables** mediante correlación y análisis dirigido
    (ej. tiempo de contrato, gasto total, tipo de servicio).

------------------------------------------------------------------------

## Modelado Predictivo

Se entrenaron y compararon distintos modelos:

-   **Regresión Logística** (requiere normalización).\
-   **KNN (K-Nearest Neighbors)**.\
-   **Random Forest** y **Árboles de Decisión** (no requieren
    normalización).

La evaluación se realizó con métricas de **Exactitud, Precisión, Recall,
F1-score y Matriz de Confusión**, asegurando una comparación objetiva de
desempeño.

------------------------------------------------------------------------

## Interpretación y Hallazgos

-   Los **clientes con mayor riesgo de evasión** son aquellos con
    **contratos mensuales**, pagos manuales, altos cargos mensuales y
    usuarios de fibra óptica.\
-   Las **variables que más influyen** en la cancelación son:
    -   **Tenure (tiempo de contrato)**: churn más alto en los primeros
        meses.\
    -   **Método de pago**: pagos electrónicos automáticos reducen la
        evasión.\
    -   **Cargos mensuales**: tarifas elevadas incrementan la
        probabilidad de cancelación.\
    -   **Tipo de internet**: usuarios de fibra óptica muestran mayor
        propensión a cancelar.\
-   El **perfil de cliente crítico a cuidar** es el de **usuarios
    nuevos, con contrato mensual, pagos manuales y cargos altos**.

------------------------------------------------------------------------

## Conclusiones

Los modelos muestran que la **predicción de churn es viable** y permite
identificar patrones consistentes de evasión. Los factores de mayor
riesgo son: **baja antigüedad, contratos cortos, pagos manuales y altos
costos**.

La empresa puede reducir la cancelación al:

-   Implementar **programas de fidelización temprana** en los primeros
    meses.\
-   Promover **contratos anuales o bianuales** con incentivos.\
-   Ofrecer **descuentos o planes ajustados** a clientes con cargos
    elevados.\
-   Incentivar **pagos automáticos**.\
-   Mejorar la experiencia de los clientes con **servicio de fibra
    óptica**.

------------------------------------------------------------------------

## Recomendaciones Estratégicas

1.  **Segmentar clientes en riesgo** usando el modelo predictivo y
    monitorearlos activamente.\
2.  **Ofrecer promociones personalizadas** para clientes con contratos
    cortos y facturas altas.\
3.  **Fomentar la automatización de pagos** como política comercial.\
4.  **Diseñar estrategias de retención específicas** para usuarios de
    fibra óptica.

------------------------------------------------------------------------

## Conclusión Final

Con un pipeline robusto de preprocesamiento y modelos predictivos,
**TelecomX puede anticiparse a la evasión de clientes, reducir el churn
y aumentar la lealtad de su base actual**, optimizando así su
rentabilidad en el mercado LATAM.
