# Datheon – Machine Learning & Data Science Internship

A collection of practical Machine Learning and Data Science projects completed as part of the Datheon internship. This repository demonstrates end-to-end workflows covering data exploration, preprocessing, feature engineering, model training, evaluation, and Natural Language Processing.

## Internship Overview

**Organization:** Datheon  
**Track:** Machine Learning & Data Science  
**Duration:** 4 Weeks  
**Technologies:** Python, Jupyter Notebook, Pandas, NumPy, Scikit-learn, XGBoost, NLTK, Matplotlib, Seaborn

## Repository Structure

```text
Datheon_Machine_Learning_-_Data_Science_Internship/
│
├── README.md
├── requirements.txt
│
├── Task 01 – Multi-Class Classification_iris.ipynb
├── Task_02_California_Housing_Price_Prediction.ipynb
├── Task_03_Customer_Churn_Prediction.ipynb
└── Task_04_Sentiment_Analysis_NLP.ipynb
```

## Completed Tasks

### Task 01: Multi-Class Classification – Iris Dataset

**Objective:** Build and compare classification models to predict Iris flower species.

**Dataset:**
- 150 samples
- 4 numerical features
- 3 target classes: Setosa, Versicolor, and Virginica
- Source: [Iris Dataset](https://raw.githubusercontent.com/mwaskom/seaborn-data/master/iris.csv)

**Workflow:**
- Data loading and exploratory data analysis.
- Data preprocessing and feature scaling.
- Stratified train-test split.
- Training Logistic Regression and Decision Tree classifiers.
- Model evaluation and comparison.

**Model Performance:**

| Model | Accuracy | Precision | Recall | F1-Score |
|---|---:|---:|---:|---:|
| Logistic Regression | 93.33% | 93.33% | 93.33% | 93.33% |
| Decision Tree | 93.33% | 93.33% | 93.33% | 93.33% |

### Task 02: California Housing Price Prediction

**Objective:** Develop regression models to predict median house values using California housing data.

**Dataset:**
- 20,640 records
- 10 original columns
- Target variable: `median_house_value`
- Source: [California Housing Dataset](https://raw.githubusercontent.com/ageron/handson-ml2/master/datasets/housing/housing.csv)

**Workflow:**
- Data exploration and visualization.
- Missing-value handling and preprocessing.
- Feature engineering and interaction features.
- Numerical scaling and categorical encoding.
- Training Linear Regression, Ridge, and Lasso models.
- Hyperparameter tuning and regression evaluation.

**Model Performance:**

| Model | RMSE | MAE | R² Score |
|---|---:|---:|---:|
| Linear Regression | 69,127.04 | 49,645.49 | 0.6353 |
| Lasso Regression | 69,128.09 | 49,646.43 | 0.6353 |
| Ridge Regression | 69,134.97 | 49,652.14 | 0.6353 |

Linear Regression achieved the best overall results, with an R² score of approximately 63.53%.

### Task 03: Customer Churn Prediction

**Objective:** Build ensemble classification models to identify customers who are likely to leave a telecommunications service.

**Dataset:**
- IBM Telco Customer Churn dataset.
- Target variable: `Churn`
- Source: [Telco Customer Churn Dataset](https://raw.githubusercontent.com/IBM/telco-customer-churn-on-icp4d/master/data/Telco-Customer-Churn.csv)

**Workflow:**
- Data cleaning and exploratory analysis.
- Conversion and handling of `TotalCharges`.
- Categorical encoding using OneHotEncoder.
- Numerical preprocessing and feature scaling.
- Class imbalance handling using class weighting.
- Training Random Forest and XGBoost classifiers.
- Cross-validation and ROC-AUC evaluation.
- Confusion matrices and feature importance analysis.

**Model Performance:**

| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Random Forest | 78.42% | 58.45% | 64.71% | 61.42% | 83.47% |
| XGBoost | 75.87% | 53.26% | 74.33% | 62.05% | 83.53% |

Both models achieved ROC-AUC scores above 80%. XGBoost achieved the highest ROC-AUC and Recall, while Random Forest achieved higher Accuracy and Precision.

### Task 04: Sentiment Analysis Using NLP

**Objective:** Build an NLP text classification system to identify positive and negative sentiment in movie reviews.

**Dataset Selection and Limitation:**

The original dataset provided through the Datheon task link contained only 10 product reviews and three sentiment labels: positive, negative, and neutral. This sample was too small for reliable model training and evaluation.

To meet the task's binary sentiment classification objective and obtain a sufficiently large dataset, the IMDb 50K Movie Reviews dataset was used instead. This dataset contains 50,000 movie reviews labeled as positive or negative.

**Dataset:**
- Original records: 50,000
- Original columns: `review`, `sentiment`
- Duplicate records identified: 418
- Missing values: 0
- Cleaned records: 49,582
- Positive reviews after cleaning: 24,884
- Negative reviews after cleaning: 24,698
- Source: [IMDb 50K Movie Reviews Dataset](https://zenodo.org/records/7928582)

**Workflow:**
- Text cleaning and preprocessing.
- Lowercasing and HTML tag removal.
- Punctuation and unwanted character removal.
- Stopword removal while preserving important negation words.
- Tokenization and lemmatization using NLTK.
- TF-IDF feature extraction with 5,000 maximum features.
- Training Multinomial Naive Bayes and Logistic Regression.
- Classification reports, confusion matrices, and ROC-AUC evaluation.
- Custom `predict_sentiment()` function for testing new reviews.

**Data Split:**

| Dataset | Samples |
|---|---:|
| Training | 39,665 |
| Testing | 9,917 |
| TF-IDF Features | 5,000 |

**Model Performance:**

| Metric | Multinomial Naive Bayes | Logistic Regression |
|---|---:|---:|
| Accuracy | 86.33% | 89.17% |
| Precision | 85.45% | 88.38% |
| Recall | 87.68% | 90.30% |
| F1-Score | 86.55% | 89.33% |
| ROC-AUC | 93.76% | 96.07% |

Logistic Regression achieved the best overall performance across all reported evaluation metrics.

The custom prediction function was also tested with four example reviews, and all four predictions matched their expected sentiment labels.

## Technologies and Libraries

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- XGBoost
- NLTK
- Jupyter Notebook

## Installation and Usage

1. Clone the repository:

```bash
git clone https://github.com/EngAbdulrahmanMamdouh/Datheon_Machine_Learning_-_Data_Science_Internship.git
```

2. Navigate to the project directory:

```bash
cd Datheon_Machine_Learning_-_Data_Science_Internship
```

3. Install the required dependencies:

```bash
pip install -r requirements.txt
```

4. Launch Jupyter Notebook:

```bash
jupyter notebook
```

5. Open the required task notebook and run the cells.

**Dataset Notes:**
- Tasks 01, 02, and 03 load their datasets from their respective online sources.
- Task 04 requires downloading the IMDb CSV dataset and placing `IMDB Dataset.csv` in the same directory as the notebook before running it.
- An active internet connection may be required to download datasets and NLTK resources.

## Skills Demonstrated

- Data Cleaning and Exploratory Data Analysis
- Data Preprocessing and Feature Engineering
- Classification and Regression
- Ensemble Learning
- Natural Language Processing
- TF-IDF Feature Extraction
- Model Evaluation and Hyperparameter Tuning
- Cross-Validation
- Data Visualization
- Git and GitHub

## Author

**Abdulrahman Mamdouh Rabea**

GitHub: [EngAbdulrahmanMamdouh](https://github.com/EngAbdulrahmanMamdouh)

## Acknowledgment

Thanks to Datheon for providing the internship tasks and the opportunity to apply Machine Learning and Data Science concepts through practical projects.

---

This repository is maintained for educational and professional portfolio purposes.
