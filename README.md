# ProyectoParteIII-SuarezLeonardo
Análisis y clasificación de salud fetal mediante Machine Learning. Incluye exploración de datos, selección de características y modelo Random Forest con 93 % de precisión para predecir riesgo fetal a partir de registros cardiotocográficos.

# 🧠 Proyecto Final - Clasificación de Salud Fetal

Este proyecto forma parte del curso **Data Science**, y tiene como objetivo aplicar las etapas del proceso de *Data Science* — desde el análisis exploratorio hasta el modelado predictivo — utilizando técnicas de **Machine Learning** para predecir el estado de salud fetal a partir de registros cardiotocográficos.

---

## 📋 Descripción del proyecto

Se trabajó con el dataset **Fetal Health Classification**, disponible en Kaggle, que contiene más de 2.000 registros de exámenes de cardiotocografía fetal con 21 variables clínicas.  
Cada registro fue clasificado por expertos en tres categorías:
- **1:** Normal  
- **2:** Sospechoso  
- **3:** Patológico  

El objetivo fue desarrollar un modelo capaz de **clasificar automáticamente** el estado de salud fetal y analizar los factores más relevantes que influyen en dicha clasificación.

---

## 🧩 Fases del proyecto

### **Fase I – Análisis Exploratorio (EDA)**
- Carga y descripción del dataset.
- Verificación de valores faltantes y análisis de correlaciones.
- Visualizaciones univariadas y multivariadas con **Matplotlib** y **Seaborn**.
- Identificación de patrones entre frecuencia cardíaca, aceleraciones, variabilidad y estado fetal.

### **Fase II – Modelado Predictivo**
- **Selección de características:** método *SelectKBest (ANOVA F-test)* para reducir dimensionalidad.
- **Entrenamiento:** algoritmo **Random Forest Classifier**.
- **Evaluación:** métricas de *accuracy, precision, recall, f1-score* y matriz de confusión.
- **Resultados:**  
  - Accuracy: **93 %**  
  - Mejor desempeño en clase *Normal*, desempeño sólido en *Patológico*.

---

## 🔍 Resultados clave

- Las variables más influyentes fueron:
  - `abnormal_short_term_variability`
  - `percentage_of_time_with_abnormal_long_term_variability`
  - `mean_value_of_short_term_variability`
- El modelo Random Forest logró una clasificación equilibrada entre las tres categorías, demostrando alta capacidad predictiva y coherencia con la evidencia clínica.

---

## 🧠 Tecnologías utilizadas
- Python 3  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- Google Colab  
- GitHub  

---

## 📈 Métricas principales
| Métrica | Valor |
|----------|--------|
| **Accuracy** | 0.93 |
| **Precision (promedio)** | 0.93 |
| **Recall (promedio)** | 0.89 |
| **F1-score (promedio)** | 0.91 |

---

## 🚀 Conclusiones

El proyecto demuestra cómo integrar **análisis exploratorio, selección de variables y aprendizaje supervisado** para resolver un problema de clasificación real.  
El modelo de Random Forest resultó ser una herramienta robusta y confiable para la **detección temprana de riesgo fetal**, confirmando la relevancia de la variabilidad cardíaca como indicador clínico principal.

---
