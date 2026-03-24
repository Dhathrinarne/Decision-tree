# 🏠 Loan Approval Prediction using Decision Tree  


![Google Colab](https://img.shields.io/badge/Google%20Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-009688?style=for-the-badge)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge)

---

## **📌 Overview**  
This project focuses on building a Decision Tree Classifier to predict loan approval using a housing finance dataset. It demonstrates a complete end-to-end machine learning workflow including:

- Data preprocessing  
- Feature engineering  
- Model building  
- Model evaluation  
- Hyperparameter tuning  

The project was implemented using Python in Google Colab and showcases how decision trees can be applied to real-world financial classification problems.

---

## **🎯 Objective**  
- To predict whether a loan will be approved or not  
- To understand Decision Tree concepts like entropy, Gini index, and information gain  
- To perform data preprocessing and feature engineering  
- To improve model performance using hyperparameter tuning  

---

## **📊 Dataset**  
- **Dataset:** Housing Finance Dataset  
- **Total Records:** 1570 rows  
- **Total Features:** 22 columns
- 
- https://1drv.ms/f/c/f483042b9735aab9/IgD-H4rA0jvITLwIi8EL5YneARJZcq-SJ7cIEQkmyUe-fFg?e=6TIYTs

### **Key Features:**  
- Age  
- Income (TotInc)  
- Loan Requested (LoanReq)  
- Loan-to-Value Ratio (LTV)  
- FOIR (Fixed Obligation to Income Ratio)  
- Employer Type  
- Marital Status  
- Accommodation Type  

### **Target Variable:**  
- **Decision → (1 = Approved, 0 = Not Approved)**  

---

## **⚙️ Features**  
- Data Cleaning & Preprocessing  
- Label Encoding & Dummy Variable Creation  
- Decision Tree Model Building  
- Model Evaluation using Accuracy & Confusion Matrix  
- Hyperparameter Tuning using GridSearchCV  
- Data Visualization  

---

## **🛠️ Tools & Technologies**  
- Python  
- Google Colab  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  

---

## **📁 Dataset Details**  
The dataset contains both categorical and numerical variables:

### **Categorical Variables:**  
- Employer_Type  
- Build_Selfcon  
- Tier  

### **Numerical Variables:**  
- Age  
- Income  
- LoanReq  
- LTV  
- etc.  

Dummy variables were created for categorical columns, and boolean values were converted into numeric format for model compatibility.

---

## **🔄 Project Flow**  

### **1. Data Collection from Google Drive**  
The dataset is stored in Google Drive and accessed within Google Colab. This allows easy file management and integration with the notebook environment.

---

### **2. Data Loading using Pandas**  
The dataset is loaded into a Pandas DataFrame using functions like `read_csv()`. This converts raw data into a structured format for analysis.

---

### **3. Data Exploration**  
Initial exploration is performed to understand the dataset:  
- `head()` → View first few rows  
- `describe()` → Get statistical summary  
- `isnull()` → Identify missing values  

This step helps in understanding data distribution and detecting issues.

---

### **4. Data Preprocessing**  

#### **a. Handling Missing Values**  
Missing or null values are treated using appropriate methods such as filling with mean/median or removing rows/columns.

#### **b. Encoding Categorical Variables**  
Categorical features (like Employer Type, Marital Status) are converted into numerical format using:  
- Label Encoding  
- One-Hot Encoding  

#### **c. Feature Engineering**  
New features may be created or existing ones modified to improve model performance and capture important patterns.

#### **d. Dummy Variable Creation**  
Categorical variables are transformed into dummy/indicator variables so that machine learning models can process them.

---

### **5. Model Pipeline**  

#### **a. Train-Test Split**  
The dataset is divided into training and testing sets (e.g., 80% train, 20% test).  
- Training data → Used to train the model  
- Testing data → Used to evaluate performance  

#### **b. Decision Tree Model Building**  
A Decision Tree Classifier is trained using the training dataset.  
The model splits data based on feature values to make predictions.

---

### **6. Model Evaluation**  

#### **a. Accuracy Score**  
Measures how many predictions are correct out of total predictions.

#### **b. Confusion Matrix**  
Provides a detailed breakdown of predictions:  
- True Positives  
- True Negatives  
- False Positives  
- False Negatives  

This helps in understanding model performance beyond accuracy.

---

### **7. Hyperparameter Tuning**  

#### **GridSearchCV for Optimal Parameters**  
GridSearchCV is used to find the best combination of parameters (like tree depth, split criteria).  
This improves model performance and prevents overfitting.

---

### **✅ Summary**  
The project follows a complete machine learning workflow:  
Data → Preprocessing → Model Building → Evaluation → Optimization  

This ensures a reliable and well-performing prediction model.
---

## **▶️ How to Run**  

# Install required libraries
pip install pandas numpy matplotlib seaborn scikit-learn

## **💻 Code**  
The complete implementation is available in the notebook:  

👉 **Decisiontree.ipynb** 
https://colab.research.google.com/drive/1C4JxM-mn9V4HG_EygJRhVR4EuVYfA0Uu?usp=drive_link

---

## **📈 Result**  
- **Model Accuracy:** ~80.89%  

### **Confusion Matrix:**  

[[ 20 52]

[ 8 234]]



The model performs well in predicting loan approvals with a high number of true positives.

---

## **📊 Visualizations**  
- Decision Tree Diagram
- <img width="1340" height="577" alt="image" src="https://github.com/user-attachments/assets/67ce5b1d-adb2-4f62-85ed-740d6b4d7cd4" />

- Confusion Matrix Heatmap
- <img width="539" height="492" alt="image" src="https://github.com/user-attachments/assets/8c230cf5-0d2c-4bcc-89d0-1f93698efa47" />

Visualizations were created using Matplotlib and Seaborn for better interpretation.

---
## **Steps:**
Open the notebook in Google Colab 

Upload given dataset 

Run all cells step-by-step

## **🔍 Key Insights**
LTV, FOIR, and Income are key factors influencing loan approval
Decision Trees provide easy interpretability through rules
Limiting tree depth helps avoid overfitting
Hyperparameter tuning significantly improves model performance

## **⭐ If you like this project**
If you found this project helpful, please give it a ⭐ on GitHub and share it with others! 🚀
