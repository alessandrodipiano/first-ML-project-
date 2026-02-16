# Predicting Hospital Readmission in Diabetic Patients
Machine Learning on Large-Scale Clinical Data

## Overview

Hospital readmissions are a major indicator of healthcare quality and cost. This project applies supervised Machine Learning techniques to predict whether diabetic patients will be readmitted after discharge, using a large real-world clinical dataset collected across multiple hospitals.

Due to severe class imbalance in the original dataset, the task is formulated as a binary classification problem:

- 0 — No readmission  
- 1 — Readmission (within or after 30 days)

The project demonstrates a complete data science workflow, from raw data exploration to the construction of a model-ready dataset.

---

## Dataset

Source: Health Facts Database (Cerner Corporation)

- Time span: 1999–2008  
- Institutions: ~130 U.S. hospitals  
- Population: Patients diagnosed with diabetes  
- Data type: Electronic health records  

The dataset includes:

- Demographic information  
- Admission and discharge details  
- Diagnoses and procedures  
- Medication data  

As typical for clinical data, it contains substantial noise, missing values, and heterogeneous feature types.

---

## Methodology

### Exploratory Data Analysis

- Distribution analysis of demographic variables  
- Examination of class imbalance  
- Detection of missing values and anomalies  
- Analysis of associations between features and target  

---

### Data Cleaning

Significant preprocessing was required due to data complexity:

- Removal of variables with excessive missing values  
- Elimination of constant or non-informative features  
- Standardization of categorical values  
- Handling of unknown or invalid entries  

---

### Feature Engineering

- Conversion of age intervals to numeric midpoints  
- Mapping admission and discharge codes into meaningful categories  
- Aggregation of ICD-9 diagnosis codes into broader groups  
- Reduction of high-cardinality categorical variables  

---

### Missing Data Handling

- Structured imputation strategy  
- KNN-based imputation for selected variables  
- Preservation of clinically meaningful information  

---

### Dataset Construction

The final dataset was prepared for supervised learning through:

- Encoding of categorical variables  
- Feature selection  
- Target transformation  
- Train/test readiness  

---

## Implementation

The project is implemented in Python using the scientific computing ecosystem:

- NumPy — numerical computation  
- Pandas — data manipulation  
- Matplotlib / Seaborn — visualization  
- Scikit-learn — preprocessing and machine learning utilities  

The notebook documents a reproducible pipeline from raw data to model-ready features.

---

## Key Challenges

Working with real healthcare data introduces several challenges:

- Severe class imbalance  
- Extensive missing data  
- Complex diagnostic coding systems  
- High-cardinality categorical features  
- Heterogeneous data types  


---

### Running the Project

Clone the repository:

git clone https://github.com/alessandrodipiano/first-ML-project-

Navigate to the project directory:

cd first-ML-project-

Launch Jupyter Notebook:

jupyter notebook "Notebook 1.ipynb"

---

## Repository Structure

Notebook 1.ipynb    End-to-end analysis and preprocessing pipeline  
README.md           Project documentation  

---

## Future Work

Possible extensions include:

- Training and comparison of classification models  
- Advanced techniques for handling class imbalance  
- Hyperparameter optimization  
- Model interpretability methods (e.g., SHAP, LIME)  
- Deployment as a clinical decision-support tool  

---

## Author

Alessandro Di Piano  
Bachelor’s student in Artificial Intelligence

