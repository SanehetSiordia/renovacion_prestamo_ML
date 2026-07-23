# ✨ Proyecto ML: Predicción de Renovación de Préstamos Bancarios

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/SanehetSiordia/renovacion_prestamo_ML/blob/main/renovacion_prestamo_ML.ipynb)
![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?style=flat-square&logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit_Learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/Estado-Completado-brightgreen?style=flat-square)

Este proyecto desarrolla un flujo completo de aprendizaje automático supervisado (Supervised Machine Learning) para identificar y predecir los clientes bancarios con mayor probabilidad de aceptar la renovación de un préstamo. El objetivo principal es optimizar las campañas de conversión comercial y reducir los costos de contacto publicitario mediante un modelado predictivo preciso.

---

## 🎯 Resumen del Proyecto

- **Problema de Negocio:** Las instituciones financieras invierten recursos significativos en campañas masivas de llamadas telefónicas y marketing directo para renovar créditos. Sin embargo, contactar a toda la base sin segmentación inteligente reduce la tasa de conversión global y genera fricción en clientes con baja propensión.
- **Solución Propuesta:** Un modelo de clasificación binaria entrenado con variables sociodemográficas, financieras y de comportamiento operativo, capaz de asignar un score de probabilidad de aceptación a cada cliente.
- **Variable Objetivo (`Target`):** `FLAG_VENTA` (Binaria: `1` = Aceptó la oferta de renovación, `0` = Rechazó o no aceptó).
- **Ejecución Inmediata:**Disponible para su revisión y ejecución directa en Google Colab mediante la insignia ubicada en la parte superior y aquí: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/SanehetSiordia/renovacion_prestamo_ML/blob/main/renovacion_prestamo_ML.ipynb)

---

## 🛠️ Stack Tecnológico

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit_Learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-2A3846?style=flat-square&logo=xgboost&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat-square&logo=python&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=flat-square&logo=python&logoColor=white)

---

## 🏗️ Flujo de Trabajo y Metodología ML

El proyecto sigue una metodología estructurada de ciencia de datos:

| Parte | Descripción |
| :--- | :--- |
| **0. Objetivo, Diccionario y librerias** | Objetivo del proyecto y del negocio, carga del conjunto de datos, definición de sus atributos y definición de las librerías utilizadas dentro del proyecto. |
| **1. Entendimiento de los Datos con EDA (Análisis Exploratorio de Datos) y Tratamiento de los Datos (Preprocesamiento & Limpieza)** | Descripción estadística de cada variable cuantitativa y cualitativa, inspección de distribuciones de valores nulos y balanceo de clases. Imputación de valores negativos y nulos, tratamiento de valores atípicos (outliers), codificación de variables categóricas y escalamiento numérico (StandardScaler). |
| **2. Particion Muestral y Balanceo de los Datos** | Partición muestral de la variable objetivo (target) y aplicación de técnicas de balanceo como UnderSampling, OverSampling y SMOTE para mitigar el desequilibrio en la variable objetivo. |
| **3. Ejecucion y Evaluacion de Modelos** | Evaluación comparativa de algoritmos supervisados de clasificación: Árboles de Decisión, Random Forest y XGBoost con los diferentes conjuntos de datos balanceados (UnderSampling, OverSampling y SMOTE). Optimización de hiperparámetros con ajuste fino mediante GridSearchCV con validación cruzada (Stratified K-Fold) y evaluación de modelos mediante matrices de confusión y reportes de clasificación (exactitud, precisión, recall y F1-score).|
| **4. Despliegue del modelo mejor evaluado** | Ejecución de casos _dummy_ y exportación del modelo mejor evaluado.|

---

## ⚙️ Guía de Configuración y Ejecución

### Ejecución en Google Colab
Puedes ejecutar todo el pipeline interactivo directamente en la nube sin instalar dependencias locales haciendo clic en el siguiente botón:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/SanehetSiordia/renovacion_prestamo_ML/blob/main/renovacion_prestamo_ML.ipynb)


---
## 📂 Estructura del Repositorio
```text
.
├── data/                         # Conjunto de datos (.csv)
├── models/                       # Artefactos del modelo entrenado (.model)
├── reports/                      # Gráficas y matrices de confusión generadas
├── renovacion_prestamo_ML.ipynb  # Notebook principal con EDA, Modelado y Evaluación
├── requirements.txt              # Lista de dependencias del entorno Python
└── README.md                     # Documentación principal del proyecto
```

---
## 🚀 Actualizacion del Proyecto con CI/CD End-To-End MLOPS
Proyecto de Renovación de Préstamo Bancario con MLOps: **[renovacion_prestamo_fastapi](https://github.com/SanehetSiordia/renovacion_prestamo_fastapi.git)**.

---
### 👤 Autor
**Sinhué Siordia Millán**