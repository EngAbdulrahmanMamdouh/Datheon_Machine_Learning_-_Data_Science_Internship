# Datheon - Machine Learning & Data Science Internship

This repository contains my projects and tasks completed during the **Datheon Machine Learning & Data Science Internship**.

The projects demonstrate practical skills in data analysis, preprocessing, feature engineering, machine learning model development, evaluation, and visualization.

## Completed Tasks

### Task 01: Multi-Class Classification – Iris Dataset

**Project Overview**

Developed and compared supervised machine learning classification models to predict Iris flower species.

**Objectives**
- Perform Exploratory Data Analysis (EDA).
- Prepare and split the dataset.
- Apply feature scaling.
- Train and evaluate classification models.
- Compare model performance using classification metrics.

**Dataset**
- Name: Iris Dataset
- Samples: 150
- Features: 4 numerical features
- Target: Setosa, Versicolor, Virginica

**Models**
- Logistic Regression
- Decision Tree Classifier

**Model Performance**

| Model | Accuracy | Precision | Recall | F1-Score |
|---|---:|---:|---:|---:|
| Logistic Regression | 93.33% | 93.33% | 93.33% | 93.33% |
| Decision Tree | 93.33% | 93.33% | 93.33% | 93.33% |

**Notebook:** `Task 01 – Multi-Class Classification_iris.ipynb`

---

### Task 02: California Housing Price Prediction

**Project Overview**

Built regression models to predict median house values using the California Housing dataset.

**Objectives**
- Perform Exploratory Data Analysis (EDA).
- Handle missing values using imputation.
- Analyze correlations and multicollinearity.
- Engineer additional ratio and interaction features.
- Apply feature scaling and categorical encoding.
- Train and compare regression models.
- Tune regularization parameters using GridSearchCV.
- Analyze prediction errors and residual distributions.

**Dataset**
- Name: California Housing Dataset
- Samples: 20,640
- Features: 8 original input features
- Target: Median House Value

**Models**
- Linear Regression (OLS)
- Ridge Regression (L2 Regularization)
- Lasso Regression (L1 Regularization)

**Model Performance**

| Model | RMSE | MAE | R² Score |
|---|---:|---:|---:|
| Linear Regression | 69,127.04 | 49,645.49 | 0.6353 |
| Ridge Regression | 69,134.97 | 49,652.14 | 0.6353 |
| Lasso Regression | 69,128.09 | 49,646.43 | 0.6353 |

**Best Test Performance:** Linear Regression, with an R² score of approximately 0.6353.

**Notebook:** `Task_02_California_Housing_Price_Prediction.ipynb`

---

## Technologies & Tools

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
- Git & GitHub

## Repository Structure

```text
Datheon_Machine_Learning_-_Data_Science_Internship/
│
├── Task 01 – Multi-Class Classification_iris.ipynb
├── Task_02_California_Housing_Price_Prediction.ipynb
├── README.md
└── requirements.txt
```

## How to Run

1. Clone this repository.
2. Install the required libraries:

```bash
pip install -r requirements.txt
```

3. Launch Jupyter Notebook:

```bash
jupyter notebook
```

4. Open the notebook you want to explore.
5. Run the cells sequentially.

**Note:** An active internet connection may be required to download the datasets from their online sources.

## Internship Information

- **Organization:** Datheon
- **Track:** Machine Learning & Data Science
- **Duration:** 4 Weeks

## Progress

This repository will be continuously updated as additional internship tasks are completed.

---

**Developed as part of the Datheon Machine Learning & Data Science Internship.**
