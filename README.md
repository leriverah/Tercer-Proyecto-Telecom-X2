# Análisis de Cancelación de Clientes - Proyecto Telecom

## 📄 Descripción del Proyecto

Este proyecto tiene como objetivo identificar los factores más influyentes en la cancelación (churn) de clientes en una empresa de telecomunicaciones, mediante el análisis exploratorio de datos y la aplicación de modelos de machine learning. Se busca, además, proponer estrategias de retención basadas en los hallazgos.

## 📊 Metodología

1. **Limpieza y preparación de los datos:**  
   Se realizó un preprocesamiento que incluyó imputación de valores faltantes, codificación de variables categóricas y normalización de variables numéricas.

2. **Selección de variables relevantes:**  
   Se seleccionaron variables como:
   - Tiempo de contrato (`tenure`)
   - Tipo de contrato (`contract.type`)
   - Servicios contratados (e.g., `internet.service`, `tech.support`)
   - Cargos mensuales y totales (`monthly.charges`, `total.charges`)
   - Método de pago (`payment.method`)

3. **Modelado predictivo:**  
   Se entrenaron y compararon varios modelos de clasificación, entre ellos:
   - Regresión logística
   - Árboles de decisión
   - Random Forest
   - XGBoost

   El rendimiento de los modelos fue evaluado utilizando métricas como Accuracy, Precision, Recall, F1-score y AUC-ROC.

## 🔍 Principales Factores que Afectan la Cancelación

Los análisis y modelos identificaron los siguientes factores como los más determinantes en la cancelación:

- **Tipo de contrato:** Clientes con contratos mensuales tienen mayor probabilidad de cancelar.
- **Soporte técnico:** La ausencia de soporte técnico incrementa la tasa de cancelación.
- **Servicio de Internet:** Clientes con servicio de fibra óptica muestran tasas de churn más elevadas.
- **Cargos mensuales elevados:** Se relacionan con mayor cancelación.
- **Método de pago electrónico automático:** Se asocia con menor cancelación, posiblemente por mayor comodidad o fidelización.

## 💡 Estrategias de Retención Propuestas

A partir de los hallazgos, se proponen las siguientes estrategias:

- **Incentivar contratos a largo plazo** con descuentos o beneficios adicionales.
- **Mejorar el soporte técnico** como factor de satisfacción y fidelización.
- **Ofrecer planes personalizados** según patrones de uso y presupuesto del cliente.
- **Promover el pago automático** mediante campañas de educación o bonificaciones.
- **Monitorear clientes con cargos altos** para ofrecerles alternativas antes de que decidan cancelar.

## 📁 Archivos del Proyecto

- `Proyecto_Telecom_X_2.ipynb`: Notebook con el análisis completo, visualizaciones y resultados de los modelos.
- `README.md`: Este documento.

## ✅ Requisitos

- Python 3.x
- Bibliotecas: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `xgboost`

## 🧠 Conclusiones

El análisis mostró que las decisiones de los clientes de cancelar están fuertemente influenciadas por aspectos contractuales y económicos. Al comprender estos patrones, la empresa puede implementar acciones proactivas para reducir el churn y mejorar la retención.