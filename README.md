# Machine Learning Notebooks: Housing & Cereals Datasets

This repository contains two Jupyter notebooks that demonstrate **supervised machine learning workflows** using regression and classification techniques. Each notebook walks through dataset exploration, model training, and evaluation using standard metrics.

---

## 📂 Contents
- `housing_regression_westroxbury.ipynb`  
  Regression analysis on a housing dataset.  
- `cereals_classification_logreg_metrics.ipynb`  
  Classification and regression metrics demonstration using a cereals dataset.  

---

## 📊 Datasets
- **WestRoxbury.csv** (used in Chapter 2 notebook)  
  - Real estate dataset containing housing features and sale prices from West Roxbury, MA.  
  - Target variable: **Price** (continuous).  

- **Cereals.csv** (used in Chapter 5 notebook)  
  - Dataset describing nutritional attributes of different cereal brands.  
  - Targets:  
    - Classification: predicting categories (e.g., manufacturer or rating thresholds).  
    - Regression: predicting cereal ratings (continuous).  

---

## 🧑‍💻 Methods Used

### 1. `housing_regression_westroxbury.ipynb`
- **Data preprocessing**: Pandas-based inspection, handling columns/rows.  
- **Train/Test Split**: Dataset partitioned using `sklearn.model_selection.train_test_split`.  
- **Modeling approach**: Prepares data for regression analysis (Linear Regression).  
- **Metrics**: No explicit metrics calculated here, but the notebook sets the stage for regression evaluation (RMSE, MAE, R²).  

---

### 2. `cereals_classification_logreg_metrics.ipynb`
- **Data preprocessing**:  
  - Handled using `pandas`.  
  - Feature scaling with `StandardScaler`.  
- **Modeling**:  
  - **Logistic Regression** → Classification task.  
  - **Linear Regression** → Regression task.  
- **Evaluation methods**:  
  - **Classification**: Confusion Matrix, ROC curve, ROC AUC.  
  - **Regression**:  
    - **MSE (Mean Squared Error)**  
    - **RMSE (Root Mean Squared Error)**  
    - **MAE (Mean Absolute Error)**  

---

## ⚙️ Environment Setup
Clone the repository and install dependencies:

```bash
git clone https://github.com/YOUR-USERNAME/ml-housing-cereals.git
cd ml-housing-cereals

python -m venv .venv
source .venv/bin/activate   # On Windows: .venv\Scripts\activate
pip install -r requirements.txt
