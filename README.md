# 🧬 Modelado de la evolución del cáncer de páncreas como sistema adaptativo complejo

Este proyecto personal busca analizar la progresión del adenocarcinoma pancreático integrando datos clínicos y moleculares del consorcio TCGA. Se exploran trayectorias evolutivas mediante técnicas de ciencia de datos, teoría de sistemas complejos y machine learning.

## 📌 Objetivos

- Unificar datos clínicos, mutacionales y de expresión génica (RNA-seq)
- Analizar dinámicas tumorales: supervivencia, mutaciones, coexpresión
- Desarrollar modelos predictivos para progresión o recurrencia
Esto significa que se necesita unificar los datos clínicos, mutacionales y de de expresión génica para identificar patrones dinámicos relacionados con la progresión tumoral y la respuesta terapéutica.

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
├── data/ # Datos sin procesar y procesados
├── notebooks/ # Análisis exploratorios en Jupyter
├── src/ # Scripts de modelado y simulación
└── README.md

## 🚧 Estado actual
-(10.07.25)
Proyecto en fase inicial (recopilación y limpieza de datos).

## 🗓️ Avance semanal (14.07.2025 – 18.07.2025)
---

### 🧩 Avances

1. **Recolección y preparación de datos**
   - Descarga de clinical_data.csv, expression_data.csv, mutations_data.csv y gene_list.csv desde cBioPortal.
   - Pivotado de clinical_data.csv a formato ancho por paciente.
   - Integración final de los datasets en una tabla única con 150 pacientes.

2. **Procesamiento de mutaciones**
   - Mapeo de entrezGeneId a hugoGeneSymbol.
   - Identificación de genes más frecuentemente mutados: KRAS, TP53, SMAD4, CDKN2A…
   - Selección de subconjunto de genes candidatos para futuros análisis.

3. **Preparación para análisis de supervivencia**
   - Revisión y transformación de variables como `DAYS_TO_COLLECTION` y `SOMATIC_STATUS`.
   - Conversión a meses de supervivencia estimada.

4. **Estructura del código**
   - Modularización del pipeline principal (`paad_data_access.py`)
   - Validaciones y limpieza automática de columnas inconsistentes.

---

### 🧠 Reflexiones o decisiones

- Mantener `gene_list.csv` actualizado como referencia cruzada.
- Crear una función utilitaria para elegir subconjuntos de genes fácilmente.

---

### 🔜 Próximos pasos

- Finalizar construcción de variables de supervivencia (`tiempo + evento`).
- Empezar análisis de curvas Kaplan–Meier por gen.
- Añadir primeros gráficos a la carpeta `/results/`.


