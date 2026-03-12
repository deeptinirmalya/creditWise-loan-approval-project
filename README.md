# CreditWise: Loan Approval Prediction

## 🚀 Project Overview
CreditWise is a machine learning-based project designed to automate the loan approval process. By analyzing various applicant attributes such as income, credit score, and debt-to-income (DTI) ratio, the system predicts whether a loan application should be approved or rejected. This project demonstrates a complete data science workflow, from data cleaning and exploratory data analysis (EDA) to feature engineering and predictive modeling.

## 📊 Dataset Description
The model is trained on a dataset containing the following features:
- **Demographics**: Age, Gender, Marital Status, Dependents, Education Level.
- **Financial Status**: Applicant Income, Co-applicant Income, Savings, Employment Status, Employer Category.
- **Loan Details**: Loan Amount, Loan Term, Loan Purpose, Property Area, Collateral Value.
- **Credit History**: Credit Score, Existing Loans, Debt-to-Income (DTI) Ratio.
- **Target Variable**: `Loan_Approved` (Yes/No).

## 🛠️ Workflow

### 1. Data Preprocessing
- **Missing Value Imputation**: Null values in numerical columns were filled with the mean, while categorical missing values were replaced with the most frequent entry.
- **Feature Engineering**: Categorical variables were transformed using One-Hot Encoding to make them compatible with machine learning algorithms.
- **Feature Scaling**: Scaled all numerical features using `StandardScaler` to ensure uniform contribution to the model's performance.

### 2. Exploratory Data Analysis (EDA)
- **Class Balance**: Visualized the distribution of approved vs. rejected loans.
- **Correlation Analysis**: Used heatmaps to identify key drivers of loan approval, finding that `Credit_Score` and `DTI_Ratio` are the most significant factors.
- **Visualizations**: Created histograms, box plots, and bar charts to understand the impact of income levels and credit history on the outcome.

### 3. Predictive Modeling
The following classification models were implemented and compared:
- **Logistic Regression**: Achieved peak performance with a clear decision boundary.
- **K-Nearest Neighbors (KNN)**: Captured local patterns in applicant data.
- **Naive Bayes**: Provided a probabilistic perspective on loan eligibility.

## 📈 Results & Evaluation
The **Logistic Regression** model outperformed others, achieving:
- **Accuracy**: ~88.5%
- **F1-Score**: 0.80
- **Precision**: ~85%
- **Recall**: ~75%

## 📂 Project Structure
```text
├── Loan_aproval_project.ipynb  # Main Jupyter Notebook with code and analysis
├── loan_approval_data.csv      # Dataset used for training and testing
├── Problem Statement.pdf       # Project requirements and domain context
└── README.md                   # Project documentation
```

## ⚙️ How to Run
1. Ensure you have Python installed along with libraries: `numpy`, `pandas`, `matplotlib`, `seaborn`, `scikit-learn`.
2. Open `Loan_aproval_project.ipynb` in Jupyter Notebook or Google Colab.
3. Run the cells sequentially to reproduce the analysis and model results.

---
*Developed as part of a Machine Learning Portfolio project.*
