# Data Preprocessing & Dimensionality Reduction Project

**Author**: Estifanos Zinabu  
**Organization**: ICog  

## 📌 Overview

This project focuses on **data preprocessing** and **dimensionality reduction** techniques using multiple real-world datasets. The goal is to clean, prepare, encode, scale, and reduce the dimensions of data to make it suitable for machine learning models.

---

## 📂 Datasets Used

1. **Titanic Survival Dataset**  
2. **House Prices - Advanced Regression Techniques**  
3. **Iris Species Dataset** (`sns.load_dataset('iris')`)  
4. **Diabetes Health Indicators (BRFSS2015)`**

---

## 🧪 Preprocessing Steps

Each dataset went through a pipeline of preprocessing steps:

### 1. Missing Data Handling
- **Numerical** values imputed using **mean/median**
- **Categorical** values imputed using **mode**
- Removed columns with too many missing values (>30%)

### 2. Categorical Data Encoding
- **Label Encoding** for ordinal data (e.g., Grade: A, B, C)
- **One-Hot Encoding** for nominal data (e.g., Department: CS, Math)

### 3. Feature Scaling
- Applied **StandardScaler** and **MinMaxScaler** to normalize feature ranges
- Essential for PCA and distance-based models

### 4. Outlier Detection
- Used **IQR method** and **Z-score** to identify outliers

### 5. Train-Test Split
- Stratified splitting (80% training / 20% testing)
- Maintained class balance where applicable

---

## 📉 Dimensionality Reduction (PCA)

- Applied **Principal Component Analysis (PCA)** to reduce dimensionality
- Retained **95% of variance**
- Resulted in more efficient computation with minimal information loss

| Dataset     | Original Features | PCA Components |
|-------------|-------------------|----------------|
| Titanic     | 10+               | 4              |
| House Prices| 30+               | ~10            |
| Iris        | 4                 | 2              |
| Diabetes    | 21                | ~7             |

---

## 📊 Tools & Libraries

- Python, Pandas, NumPy
- Scikit-learn (`StandardScaler`, `PCA`, `train_test_split`, etc.)
- Seaborn / Matplotlib (for visualization)

---

## 📁 Folder Structure
.
├── data/
│ └── [csv files for each dataset]
├── notebooks/
│ └── preprocessing_pipeline.ipynb
├── results/
│ └── visualizations, PCA outputs
└── README.md

---

## 🎯 Goals Achieved

✅ Cleaned messy real-world data  
✅ Encoded and scaled features appropriately  
✅ Reduced high-dimensional data with PCA  
✅ Ensured reproducibility and model-readiness  

---

## 🙏 Acknowledgments

Thanks to:
- [Kaggle](https://www.kaggle.com) for datasets
- [CDC](https://www.cdc.gov/brfss/) for BRFSS2015
- [Scikit-learn](https://scikit-learn.org) for robust ML tools

---

## 📬 Contact

For questions or collaboration:  
📧 estifanoszinabuabebe@gmail.com

---

## 📌 License

This project is licensed under the **MIT License**.

