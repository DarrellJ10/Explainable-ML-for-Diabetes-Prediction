# Explainable Machine Learning for Diabetes Prediction  
Georgia Southern University – Fall 2025 | IT-7135: Seminar in Information Technology

---

## Project Overview
This project explores how Explainable Artificial Intelligence (XAI) can make machine learning predictions more transparent and trustworthy in healthcare.  
Using the CDC’s 2015 Behavioral Risk Factor Surveillance System (BRFSS) dataset, we train a Random Forest classifier to predict diabetes risk based on key demographic, behavioral, and health-related features.  
To interpret the model, we apply SHapley Additive exPlanations (SHAP), which explain how each feature contributes to individual and group predictions.  

---

## Objectives
- Develop a predictive model to identify individuals at risk for diabetes.  
- Apply Random Forest for reliable and interpretable prediction.  
- Use SHAP to explain model decisions at both local (individual) and global (population) levels.  
- Promote trust and clinical adoption by improving model transparency.  

---

## Dataset Description
Source: CDC Behavioral Risk Factor Surveillance System (BRFSS) 2015  
Dataset Size: ~400,000 records  

Key Features Used:
| Feature | Description |
|----------|--------------|
| GENHLTH | Self-rated general health |
| BPHIGH4 | Ever told you have high blood pressure |
| CHOLCHK | Cholesterol checked within past 5 years |
| TOLDHI2 | Told you have high cholesterol |
| SEX | Gender (1 = Male, 2 = Female) |
| EDUCA | Education level |
| INCOME2 | Income category |
| SMOKE100 | Smoked 100+ cigarettes in lifetime |
| EXERANY2 | Any physical activity/exercise in past month |
| _AGEG5YR | Age category (5-year groups) |
| _BMI5 | Body Mass Index × 100 |
| DIABETE3 | Diagnosed diabetes status (Target variable) |

---

## Project Workflow
1. Data Preprocessing  
   - Removed missing and special codes (e.g., 7, 9)  
   - Normalized BMI values  
   - Replaced missing values using mean imputation  

2. Feature Selection  
   - Selected 12 clinically relevant health, lifestyle, and demographic indicators  

3. Model Training  
   - Algorithm: Random Forest Classifier  
   - Metrics: Accuracy, Precision, Recall, F1-Score, ROC-AUC  

4. Explainability  
   - Tool: SHAP (SHapley Additive exPlanations)  
   - Visualized feature importance and local contributions  

5. Evaluation  
   - Compared predictive accuracy with interpretability insights  

---

## Technologies Used
| Category | Tools |
|-----------|-------|
| Language | Python 3.12 |
| Libraries | pandas, numpy, scikit-learn, shap, matplotlib |
| Notebook | Jupyter Notebook |
| Version Control | Git & GitHub |
| Dataset | CDC BRFSS 2015 (Kaggle) |

---

