## 📊 Exploratory Data Analysis (EDA)

### Loan Approval Class Distribution
![Loan Approval Class Distribution](loan_approval_distribution.png)

**Observation**
- The dataset is imbalanced
- Around 70% of applications are rejected
- Around 30% of applications are approved
- Evaluation metrics beyond accuracy are required



### Debt-to-Income (DTI) Ratio vs Loan Approval
![DTI Ratio vs Loan Approval](dti_ratio_boxplot.png)

**Observation**
- Lower DTI ratios are associated with loan approval
- High DTI ratios strongly correlate with rejection
- Critical risk indicator in loan decisions

---

### Savings vs Loan Approval
![Savings vs Loan Approval](images/savings_boxplot.png)

**Observation**
- Savings show weak separation between classes
- High savings alone do not ensure approval
- Acts as a supporting rather than decisive feature

---

### EDA Summary
- Credit Score and DTI Ratio are the strongest predictors
- Applicant Income has moderate influence
- Savings have limited standalone impact
- Insights justify the selection of Logistic Regression as the final model
