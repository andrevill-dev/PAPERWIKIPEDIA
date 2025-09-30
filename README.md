# 📊 Data Processing and Analysis Project

This repository contains the complete workflow for processing, exploring, and analyzing a dataset.  
The steps are implemented through **Jupyter Notebooks**, following a logical order from raw data preprocessing to dimensionality reduction and clustering.

> ⚠️ Note: The **original dataset cannot be published on GitHub** due to privacy and usage restrictions.  
> Instead, processed versions are included in `.pkl` format so the analyses can be reproduced.

---

## 🚀 Project Workflow

### 0. Data Preprocessing
**Notebook:** `0_Procesamiento Data.ipynb`  
- Initial data cleaning.  
- Normalization of fields and handling of missing values.  
- Preparing a structured dataset for further analysis.

---

### 1. Static Data Exploration
**Notebook:** `1_ExploracionDataESTATICA.ipynb`  
- Exploratory Data Analysis (EDA).  
- Descriptive statistics, data distributions, and basic correlations.

---

### 2. Temporal Analysis
**Notebook:** `2_EDICIONES_AN_TEMPORAL.ipynb`  
- Time-based analysis of the dataset.  
- Identification of trends, peaks, and temporal patterns.

---

### 3. Category Analysis
**Notebook:** `3_EDICIONES X CATEGORIA.ipynb`  
- Grouping and analyzing data by main categories.  
- Identifying similarities and differences across groups.

---

### 4. Editor Analysis by Category
**Notebook:** `4_EDITORES X CATEGORIA.ipynb`  
- Breaking down the dataset by editors and categories.  
- Detecting behavioral differences between editors.

---

### 5. Autoencoder – Dimensionality Reduction (Editions)
**Notebook:** `5_EDICIONES Autoencoder for Dimensionality Reduction.ipynb`  
- Applying an autoencoder model to reduce dimensionality.  
- Generating embeddings for editions to simplify later clustering.

---

### 6. Autoencoder – Dimensionality Reduction (Editors)
**Notebook:** `6_EDITORES Autoencoder for Dimensionality Reduction.ipynb`  
- Autoencoder applied specifically to editors’ data.  
- Optimizing representations for improved clustering performance.

---

### 7. Clustering with HDBSCAN
**Notebook:** `7_HDBSCAN CLUSTERING.ipynb`  
- Using the **HDBSCAN** algorithm on reduced embeddings.  
- Discovering dense clusters and grouping patterns.  
- Evaluating the quality and consistency of clusters.

---

## 📂 Processed Data

The `.pkl` files contain the processed datasets, ready for reuse in the notebooks:

- `language_activities.pkl` → Processed activities.  
- `language_editions.pkl` → Processed editions.  
- `language_editors.pkl` → Processed editors.  

These replace the original dataset, which cannot be shared publicly.

---

## 🛠️ Requirements

- Python 3.10+  
- Jupyter Notebook  
- Main libraries:
  - pandas  
  - numpy  
  - matplotlib / seaborn  
  - scikit-learn  
  - tensorflow / keras (for autoencoders)  
  - hdbscan  


