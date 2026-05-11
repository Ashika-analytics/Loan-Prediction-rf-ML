# Loan Approval Prediction Using Machine Learning

##  Project Overview
This project predicts whether a loan application will be **approved or rejected** using Machine Learning techniques.  
Multiple models were trained and compared to identify the best-performing approach, with special focus on **minority class recall**.

---

##  Dataset
The dataset contains loan applicant details such as:
- Gender  
- Marital Status  
- Education  
- Applicant Income  
- Loan Amount  
- Credit History  
- Property Area  
- Loan Status (Target Variable)

---

##  Technologies Used
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Scikit-learn  
- XGBoost  

---

##  Machine Learning Models Used
The project follows a **step-by-step model building approach**:

1. **Logistic Regression**
   - Used as a baseline model
   - Helped understand feature impact and initial performance

2. **Random Forest Classifier**
   - Captures non-linear relationships
   - Reduces overfitting using ensemble learning
   - SMOTE was applied to handle class imbalance

3. **XGBoost Classifier**
   - Gradient boosting technique
   - Provided better performance compared to other models
   - Handled class imbalance more effectively

---

##  Model Evaluation & Key Observations
Model performance was evaluated using **recall for the minority class**, as correctly identifying minority cases was the primary objective.

- **Logistic Regression**  
  Minority class recall was very low, serving as a baseline.

- **Random Forest (with SMOTE)**  
  Despite balancing the dataset using SMOTE, **minority class recall did not show meaningful improvement**.

- **XGBoost**  
  Achieved a **minority class recall of 0.51**, which was the **best among all models**.  
  Although not very high in absolute terms, it **significantly outperformed Logistic Regression and Random Forest**, highlighting XGBoost’s ability to handle      class imbalance more effectively.

This demonstrates that **model selection and evaluation metrics are more important than accuracy alone**.

---

##  Files in this Repository
- `Loan_prediction-rf.ipynb` → Google Colab (Jupyter) notebook containing Logistic Regression, Random Forest, and XGBoost implementations  
- `README.md` → Project documentation  

---

##  How to Run the Project
1. Clone the repository  
2. Install the required libraries  
3. Open the notebook and run all cells

##  Dataset Source
The dataset used in this project is **publicly available** and has been included in this repository for reproducibility and ease of use.

---

##  Author
**Ashika**
