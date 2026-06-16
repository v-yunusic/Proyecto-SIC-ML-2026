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

## 🛠️ Tecnologías y Herramientas Utilizadas

### 1. Manipulación de Datos y Machine Learning 📊
Estas son las herramientas fundamentales para leer el archivo CSV, limpiarlo y entrenar los modelos:

* **`pandas`**: La librería reina para la manipulación de datos tabulares. Permite cargar el CSV, manejar valores nulos, filtrar y estructurar la información.
* **`scikit-learn`**: El estándar para Machine Learning clásico en Python. Incluye algoritmos de clasificación, regresión y clustering, además de herramientas para preprocesar datos (escalar, codificar) y evaluar modelos (métricas de error, precisión).
* **`numpy`**: Trabaja en conjunto con Pandas y Scikit-learn para realizar cálculos numéricos de alto rendimiento bajo el capó.

### 2. Visualización de Datos 📈
Utilizadas para crear los gráficos que luego analizará la IA:

* **`matplotlib`** y **`seaborn`**: Excelentes para crear gráficos estadísticos estáticos (matrices de confusión, mapas de calor, dispersión). Seaborn hace que los gráficos de Matplotlib se vean mucho más estéticos con menos código.
* **`plotly`**: Alternativa recomendada para gráficos interactivos. Permite al usuario interactuar con los datos y exportar fácilmente las visualizaciones como imágenes estáticas si la IA lo requiere.

### 3. Integración de Inteligencia Artificial 🧠
Para que la IA pueda "leer" los gráficos y analizar los resultados mediante capacidades multimodales (texto e imágenes):

* **APIs de Modelos de Lenguaje (LLMs)**: Uso de **Google Gemini API** o **OpenAI API (GPT-4o)** para procesar el resumen de texto de los datos (métricas del modelo) junto con las imágenes de los gráficos generados.
* **`langchain`** (Opcional): Framework que facilita la conexión del código con los modelos de IA, ayudando a estructurar los *prompts* y a crear flujos de trabajo secuenciales.

### 4. Interfaz de Usuario (UI) 💻
Para proveer una interfaz visual interactiva sin necesidad de conocimientos front-end:

* **`streamlit`**: Herramienta utilizada para crear la aplicación web. Permite desplegar una página donde el usuario puede subir su CSV, visualizar los gráficos y leer el análisis de la IA en tiempo real utilizando únicamente código Python.

### 5. Entorno y Seguridad 🔒
* **`python-dotenv`**: Librería esencial para cargar variables de entorno desde un archivo `.env`, manteniendo seguras las claves de las APIs (API Keys) fuera del código fuente.
* **Jupyter Notebook (`jupyterlab`)**: Entorno utilizado en la etapa inicial de desarrollo para realizar pruebas, ejecutar código bloque por bloque y validar los gráficos de manera inmediata.
