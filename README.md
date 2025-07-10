# 🧬 Modelado de la evolución del cáncer de páncreas como sistema adaptativo complejo

Este proyecto personal busca analizar la progresión del adenocarcinoma pancreático integrando datos clínicos y moleculares del consorcio TCGA. Se exploran trayectorias evolutivas mediante técnicas de ciencia de datos, teoría de sistemas complejos y machine learning.

## 📌 Objetivos

- Unificar datos clínicos, mutacionales y de expresión génica (RNA-seq)
- Analizar dinámicas tumorales: supervivencia, mutaciones, coexpresión
- Desarrollar modelos predictivos para progresión o recurrencia

## 🗂️ Dataset

- Fuente: [TCGA Pancreatic Adenocarcinoma (PAAD) – cBioPortal](https://www.cbioportal.org/study/summary?id=paad_tcga)

## ⚙️ Tecnologías

- Python, Pandas, NumPy, Scikit-learn, XGBoost
- Seaborn, Plotly, NetworkX, Lifelines (Kaplan-Meier)

## 📊 Fases del proyecto

1. **Planificación y exploración**  
2. **Preprocesamiento de datos**  
3. **Análisis exploratorio**  
4. **Modelado predictivo (ML)**  
5. **Interpretación y conclusiones**

## 📁 Estructura

```
📂 data/            # Archivos CSV, mutaciones, RNA-seq
📂 notebooks/       # Jupyter Notebooks por fase
📂 src/             # Funciones reutilizables
📂 results/         # Gráficos, modelos, evaluaciones
README.md
requirements.txt
```

## 🧠 Lecciones aprendidas

- Integración multiómica y limpieza de datos biomédicos
- Interpretación clínica de modelos ML
- Ciencia reproducible y documentación paso a paso
