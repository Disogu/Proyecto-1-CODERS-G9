# Breast Cancer Classification with Traditional Machine Learning

## 🎯 Objetivo del Proyecto
Clasificar tumores como benignos o malignos utilizando algoritmos clásicos de machine learning, con un flujo de trabajo modular y reproducible.

## 📂 Descripción del Dataset
Se utiliza el dataset de cáncer de mama de Wisconsin, disponible en `sklearn.datasets.load_breast_cancer`. Contiene 569 muestras y 30 características numéricas extraídas de imágenes digitales de biopsias.

## ⚖️ Decisiones Tomadas en el Modelado
- Selección de características basada en ganancia de información mutua y comparación con chi-cuadrado.
- Comparación automática de modelos con LazyPredict.
- Métrica principal: F1-score, por el balance entre precisión y recall en problemas médicos.
- Registro y gestión de experimentos con MLflow.

## 📈 Resultados y Métricas Principales
- Mejor modelo: RandomForestClassifier
- Accuracy: 0.97
- F1-score: 0.96

## ⚙️ Instrucciones para Ejecutar el Proyecto

1. Clona este repositorio:
```bash
git clone https://github.com/tu_usuario/breast_cancer_ml_project.git
cd breast_cancer_ml_project
```

2. Instala las dependencias:
```bash
pip install -r requirements.txt
```

3. Ejecuta los notebooks en orden:
   - `1_EDA.ipynb`: análisis exploratorio de datos.
   - `2_preprocessing.ipynb`: preparación de datos y selección de características.
   - `3_train_validate_model.ipynb`: entrenamiento con LazyPredict, selección del mejor modelo y logging con MLflow.
   - `4_evaluation_export.ipynb`: evaluación final y exportación del modelo.

4. Opcionalmente, inicia el servidor MLflow para visualizar los resultados:
```bash
mlflow ui
```
Visita `http://localhost:5000` en tu navegador.

---

Este proyecto sigue las buenas prácticas de desarrollo de ML propuesto por Pau Labarta.
