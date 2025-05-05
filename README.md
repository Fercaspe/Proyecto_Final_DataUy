# Proyecto Final - Clasificación de Ingresos con Datos del Censo (Adult Dataset)

Este proyecto tiene como objetivo predecir si el ingreso anual de una persona supera los USD 50.000 utilizando técnicas de Machine Learning. Se desarrolló como parte de una formación técnica en Análisis de Datos y Aprendizaje Automático.

## 📌 Descripción del Proyecto

Se utilizó el dataset **"Adult Census Income"** proveniente del censo de EE.UU. de 1994. Este conjunto de datos incluye variables demográficas, educativas y laborales. El objetivo es construir un modelo predictivo que clasifique a los individuos según si su ingreso anual es superior a USD 50.000.

Se compararon dos enfoques de clasificación:
- **Regresión Logística** (modelo base)
- **XGBoost** (modelo avanzado basado en árboles de decisión)

## 🔍 Metodología

1. **Análisis Exploratorio de Datos (EDA):**
   - Tipos de variables, valores faltantes, balance de clases
   - Distribuciones de variables numéricas y categóricas
   - Evaluación ética del uso de variables sensibles (género y raza)

2. **Preprocesamiento de Datos:**
   - Imputación de valores faltantes
   - Normalización de variables numéricas
   - One-Hot Encoding de variables categóricas
   - Eliminación de variables con riesgo ético o redundantes

3. **Modelado:**
   - Implementación de Pipelines con `sklearn` y `imblearn`
   - Aplicación de SMOTE para corregir desbalance de clases
   - Optimización de hiperparámetros con `RandomizedSearchCV` para XGBoost

4. **Evaluación:**
   - Métricas utilizadas: Accuracy, Precision, Recall, F1-Score y Matriz de Confusión
   - Comparación de desempeño entre modelos

## ⚙️ Tecnologías y Herramientas

- Python (pandas, numpy, matplotlib, seaborn, plotly)
- Scikit-learn
- XGBoost
- Imbalanced-learn (SMOTE)
- Google Colab

## 📈 Resultados

El modelo XGBoost superó en rendimiento al modelo de Regresión Logística, logrando mejores métricas en precisión y recall, especialmente para la clase minoritaria (>50K), demostrando su capacidad para manejar datos complejos y desbalanceados.

## ⚖️ Consideraciones Éticas

Se identificaron variables sensibles como `race` y `sex`. Para evitar sesgos en los modelos y respetar buenas prácticas éticas, estas columnas fueron excluidas del entrenamiento.


## 📬 Contacto

Fernando Caspe  
📧 fercaspe@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/fercaspe)  


---

Este proyecto forma parte de mi portfolio como Analista de Datos en proceso de transición profesional desde el área de Operaciones y Logística. ¡Gracias por tu interés!
