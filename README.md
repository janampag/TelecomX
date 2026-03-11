# 📉 Análisis de Evasión de Clientes (Churn) - Telecom X

Este proyecto forma parte de un desafío de análisis de datos para una empresa de telecomunicaciones. El objetivo principal es identificar patrones de comportamiento en los clientes que cancelan sus servicios y proponer estrategias basadas en datos para mejorar la retención.



## 🛠️ Tecnologías y Herramientas
* **Lenguaje:** Python 3.12
* **Librerías:** Pandas, NumPy, Matplotlib, Seaborn
* **Entorno:** Google Colab / Jupyter Notebook
* **Formato de datos:** JSON (Normalizado a Tabular)

## 📋 Resumen del Proyecto

### 1. Limpieza y Transformación (ETL)
El dataset original contenía datos anidados en formato de diccionario. Se realizaron las siguientes tareas:
* **Normalización:** Desglose de información técnica, personal y financiera.
* **Tratamiento de nulos:** Identificación de strings vacíos y manejo de datos faltantes en cargos totales.
* **Feature Engineering:** Creación de la métrica `Cuentas_Diarias` (costo diario del servicio).
* **Estandarización:** Traducción de variables al español y codificación binaria ($0$ y $1$) para análisis estadístico.

### 2. Hallazgos Clave (Insights)
Tras el Análisis Exploratorio de Datos (EDA), se identificaron los siguientes puntos críticos:
* **Factor de Riesgo:** Los clientes con contratos **mes a mes** representan el mayor volumen de deserción.
* **Sensibilidad al Precio:** Existe una correlación positiva entre los cargos mensuales elevados y la probabilidad de abandono.
* **Periodo Crítico:** Los primeros **6 meses** de antigüedad son determinantes; si el cliente supera este periodo, la probabilidad de fuga disminuye significativamente.



## 📈 Visualizaciones Principales
En este repositorio encontrarás gráficos que detallan:
1. La distribución porcentual de la evasión.
2. Comparativa de abandono por tipo de contrato y método de pago.
3. Boxplots de cargos mensuales vs. permanencia.
4. Matriz de correlación de variables financieras.

## 💡 Recomendaciones Estratégicas
* **Incentivos de Contrato:** Migrar clientes de planes mensuales a anuales mediante bonificaciones.
* **Fidelización Temprana:** Implementar campañas de soporte prioritario para clientes nuevos.
* **Venta Cruzada:** Fomentar la adopción de servicios adicionales para aumentar las barreras de salida.
