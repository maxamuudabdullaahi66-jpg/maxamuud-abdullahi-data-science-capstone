# 📊 Customer Churn Prediction — Data Science Capstone

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![Scikit--learn](https://img.shields.io/badge/Scikit--learn-Machine%20Learning-F7931E?logo=scikit-learn)
![Plotly](https://img.shields.io/badge/Plotly-Visualization-3F4F75?logo=plotly)
![Dash](https://img.shields.io/badge/Dash-Dashboard-008DE4)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter)

## 👤 Author

**Maxamuud Abdullahi**

## 🚀 Project Overview

This project demonstrates an end-to-end **Data Science and Machine Learning workflow** for customer churn prediction.

It includes data cleaning, exploratory data analysis, SQL analysis, feature engineering, machine learning, model evaluation, visualizations, an interactive dashboard, and a final report.

> **Dataset note:** This repository uses a **synthetic educational dataset** created specifically for this capstone. It does not represent real customers, a real company, or official statistics about Somalia.

## 🎯 Objectives

- Prepare and clean customer-level data.
- Explore patterns associated with churn.
- Answer business questions using SQL.
- Engineer machine-learning features.
- Compare classification algorithms.
- Evaluate models using accuracy, precision, recall, and F1-score.
- Build an interactive dashboard.
- Produce a reproducible portfolio project.

## 🗂️ Project Structure

```text
├── data/
├── notebooks/
│   ├── 01_data_collection.ipynb
│   ├── 02_data_wrangling.ipynb
│   ├── 03_eda_visualization.ipynb
│   ├── 04_sql_analysis.ipynb
│   ├── 05_feature_engineering.ipynb
│   └── 06_machine_learning.ipynb
├── src/
│   ├── data_cleaning.py
│   ├── train_model.py
│   └── churn_analysis.sql
├── dashboard/
│   └── app.py
├── models/
├── reports/
├── images/
│   └── figures/
├── README.md
└── requirements.txt
```

## 📦 Dataset

The project contains **1,200 synthetic customer records** covering demographics, region, contract type, service usage, payment behavior, tenure, spending, satisfaction, support calls, complaints, and churn.

## 🔎 Exploratory Data Analysis

### Churn Distribution
![Churn Distribution](images/figures/01_churn_distribution.png)

### Churn by Contract Type
![Churn by Contract](images/figures/02_churn_by_contract.png)

### Churn by Region
![Churn by Region](images/figures/03_churn_by_region.png)

### Churn by Satisfaction
![Churn by Satisfaction](images/figures/04_churn_by_satisfaction.png)

### Churn by Tenure
![Churn by Tenure](images/figures/05_churn_by_tenure.png)

### Churn by Payment Method
![Churn by Payment](images/figures/06_churn_by_payment.png)

## 🤖 Machine Learning

Three classification algorithms were tested:

- Logistic Regression
- Decision Tree
- Random Forest

The workflow uses a stratified train/test split, preprocessing pipelines, one-hot encoding, scaling, class balancing, and multiple evaluation metrics.

## 📈 Model Results

Results from the held-out test set of the synthetic dataset:

| Model | Accuracy | Precision | Recall | F1 |
|---|---:|---:|---:|---:|
| Logistic Regression | 0.650 | 0.122 | 0.455 | 0.192 |
| Decision Tree | 0.558 | 0.118 | 0.591 | 0.197 |
| Random Forest | 0.904 | 0.000 | 0.000 | 0.000 |

For this demonstration, the **Decision Tree** is used in the included deployment pipeline because it has the highest F1-score among the tested models.

These results are **not general claims about real-world performance**, because the underlying dataset is synthetic.

### Confusion Matrix

![Confusion Matrix](images/figures/07_confusion_matrix.png)

## 🗄️ SQL Analysis

Reusable SQL queries are available in:

```text
src/churn_analysis.sql
```

They cover customer counts, churn rates by contract, spending and satisfaction comparisons, and customers with repeated support interactions.

## 📊 Interactive Dashboard

The project includes a Plotly Dash dashboard showing:

- Customer count
- Observed synthetic churn rate
- Churn rate by contract type
- Churn rate by region

Run:

```bash
python dashboard/app.py
```

## 🛠️ Technologies

**Python · Pandas · NumPy · Matplotlib · Scikit-learn · SQL · Plotly · Dash · Jupyter · Joblib · GitHub**

## ▶️ Run Locally

```bash
git clone https://github.com/YOUR_USERNAME/maxamuud-abdullahi-data-science-capstone.git
cd maxamuud-abdullahi-data-science-capstone
pip install -r requirements.txt
python src/data_cleaning.py
python src/train_model.py
python dashboard/app.py
```

## 📄 Final Report

The complete report is located at:

```text
reports/Maxamuud_Abdullahi_Customer_Churn_Capstone_Report.pdf
```

## ⚠️ Limitations

- The dataset is synthetic.
- It does not represent actual Somali customer behavior.
- The models have not been externally validated.
- The analysis does not establish causal relationships.
- Real deployment would require privacy, security, fairness, monitoring, and data-quality controls.

## 🔮 Future Improvements

- Replace the synthetic dataset with a real, appropriately licensed dataset.
- Add cross-validation and hyperparameter tuning.
- Add SHAP/model explainability.
- Add automated data validation.
- Add dashboard filters.
- Add model monitoring.
- Deploy the dashboard to a cloud service.
- Add GitHub Actions tests.

## 👨‍💻 Author

**Maxamuud Abdullahi**

Data Science | Python | SQL | Machine Learning | Data Visualization

⭐ **Portfolio project:** A reproducible Data Science workflow from data preparation to machine learning, visualization, dashboarding, and reporting.
