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
-(15.07.2025)
1. Seleccionar genes candidatos:
- Los más conocidos en cáncer de páncreas.
- Los genes más mutados presentes en los pacientes con cáncer.
- Los genes con mayor correlación con la supervivencia (calcular la correlación entre la expresión génica y la supervivencia para cada gen). Podría dar candidatos funcionales aunque no presenten mutación.
-Combinación de los anteriones métodos de selección de genes candidatos.
2. Dividir pacientes por expresión génica alta/baja (por percentil o mediana).
3. Graficar curva KM para cada gen, comparando los grupos.
4. Evaluar significancia estadística (log-rank test).

# Genes candidatos comunes en cáncer de páncreas según la bibliografía consultada (debo añadir la bibliografía consultada) #

Gen	-- Rol principal
KRAS -- Oncogén (mutado en ~90%)
TP53 -- Supresor tumoral
CDKN2A -- Ciclo celular
SMAD4	-- Vía TGF-β
BRCA1/2	-- Reparación de ADN
ARID1A	-- Remodelación cromatina
GATA6	-- Diferenciación pancreática
MYC	-- Proliferación celular
PTEN	-- Inhibidor de PI3K/AKT
MUC1	-- Adhesión y señalización

# Genes candidatos según su frecuencia de mutación presentes en los pacientes con cáncer de mis datos #

