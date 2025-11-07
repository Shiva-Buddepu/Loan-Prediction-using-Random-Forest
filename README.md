# Loan Prediction using Random Forest

This project predicts whether a loan application will be approved using a **Random Forest Classifier**.  
The dataset includes applicant demographic, financial, and credit information used to determine the loan approval status.

---


## Dataset Entities Description

| Entity Name          | Description |
|----------------------|-------------|
| **Loan_ID**          | Unique ID assigned to each loan applicant |
| **Gender**           | Applicant gender (Male/Female) |
| **Married**          | Marital status of the applicant |
| **Dependents**       | Number of dependents |
| **Education**        | Education level (Graduate/Not Graduate) |
| **Self_Employed**    | Whether the applicant is self-employed |
| **ApplicantIncome**  | Monthly income of the main applicant |
| **CoapplicantIncome**| Monthly income of co-applicant |
| **LoanAmount**       | Loan amount requested (in thousands) |
| **Loan_Amount_Term** | Duration of loan repayment (in months) |
| **Credit_History**   | Credit score history (1 = good, 0 = bad) |
| **Property_Area**    | Applicant’s property location (Urban/Rural/Semiurban) |
| **Loan_Status**      | Loan approval status (Y = Approved, N = Not Approved) |

---

## Project Workflow

### 1. Import Libraries
Imported essential Python libraries:
- pandas  
- numpy  
- matplotlib  
- seaborn  
- scikit-learn  

### 2. Outlier Detection
Checked for outliers in:
- ApplicantIncome  
- CoapplicantIncome  
- LoanAmount  

### 3. Data Analysis
Performed:
- Summary statistics  
- Missing value detection  
- Distribution analysis  

### 4. Data Visualization
Created:
- Count plots  
- Box plots  
- Distribution plots  
- Correlation heatmap  

### 5. Preprocessing
Included:
- Handling missing values  
- Encoding categorical variables  
- Feature scaling (if required)  
- Splitting into train/test sets  

### 6. Model Building – Random Forest
Implemented the Random Forest Classifier:
```python
from sklearn.ensemble import RandomForestClassifier
model = RandomForestClassifier()
