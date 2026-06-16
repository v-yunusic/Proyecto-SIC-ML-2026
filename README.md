# Proyecto-SIC-ML-2026

Repositorio para desarrollo de herramienta integral diseñada para simplificar y automatizar el ciclo de vida inicial de los proyectos de ciencia de datos. Este programa toma bases de datos crudas y automatiza el tratamiento de valores nulos (MV), el preprocesamiento de características y la evaluación de algoritmos de Machine Learning para encontrar el modelo base (*baseline*) más adecuado.

## 🚀 Características Principales

* **🔍 Tratamiento de Valores Faltantes (MV):** * Detección automática de *Missing Values*.
    * Estrategias de imputación configurables (Media, Mediana, Moda, o KNN).
    * Eliminación inteligente de columnas/filas con umbrales personalizables.
* **⚙️ Preprocesamiento de Datos:**
    * Codificación de variables categóricas (One-Hot Encoding, Label Encoding).
    * Escalado y normalización de variables numéricas (StandardScaler, MinMaxScaler).
    * Manejo de valores atípicos (*Outliers*).
* **🧠 Selección de Algoritmos (Machine Learning):**
    * Soporte para problemas de **Clasificación** y **Regresión**.
    * Entrenamiento rápido de múltiples algoritmos populares (Random Forest, SVM, Regresión Logística, XGBoost, etc.).
    * Generación de métricas comparativas (Accuracy, F1-Score, RMSE, R2) para elegir el mejor modelo.
