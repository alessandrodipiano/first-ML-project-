Predicting Hospital Readmission in Diabetic Patients

A Machine Learning Study on Large-Scale Clinical Data

Abstract

Hospital readmissions represent a critical challenge for healthcare systems, reflecting both patient outcomes and economic burden. This project investigates the prediction of readmission for diabetic patients using a large real-world clinical dataset spanning multiple hospitals and years. The work focuses on constructing a rigorous end-to-end Machine Learning pipeline capable of handling noisy, heterogeneous medical data.

Problem Statement

Given patient records collected during hospital stays, the objective is to predict whether a patient will be readmitted after discharge.

The original dataset defines three outcomes:

No readmission

Readmission within 30 days

Readmission after 30 days

Due to severe class imbalance, the problem is reformulated as binary classification:

𝑦
=
{
1
	
if readmitted


0
	
otherwise
y={
1
0
	​

if readmitted
otherwise
	​

Dataset

Health Facts Database (Cerner Corporation)

Time span: 1999–2008

Institutions: ~130 U.S. hospitals

Population: Patients diagnosed with diabetes

Features: Demographics, diagnoses, procedures, medications, admission details

The dataset reflects real clinical practice and therefore exhibits:

Extensive missing values

High-cardinality categorical variables

Administrative coding systems

Measurement inconsistencies

Methodology
Exploratory Data Analysis

Distribution analysis of demographic variables

Examination of outcome imbalance

Identification of missingness patterns

Statistical association tests between features and target

Data Cleaning

Clinical datasets require substantial preprocessing. Key steps include:

Removal of variables with excessive missing data

Elimination of constant or non-informative features

Standardization of categorical values

Treatment of unknown or invalid entries

Feature Engineering

Conversion of age ranges to numerical midpoints

Mapping admission and discharge codes to meaningful categories

Aggregation of ICD-9 diagnosis codes into broader clinical groups

Reduction of high-cardinality categorical features

Missing Data Handling

Structured imputation strategy

KNN-based imputation for selected variables

Preservation of clinically meaningful patterns

Dataset Construction

A model-ready dataset is produced through:

Encoding of categorical variables

Feature selection

Target transformation

Preparation for supervised learning

Implementation

The project is implemented in Python using the scientific computing ecosystem:

NumPy — numerical operations

Pandas — data manipulation

Matplotlib / Seaborn — visualization

Scikit-learn — preprocessing and ML utilities

The notebook documents a reproducible pipeline from raw data to training-ready features.

Key Challenges

Working with real healthcare data introduces several nontrivial issues:

Extreme class imbalance

Missing and inconsistent records

Complex diagnostic coding systems

Heterogeneous feature types

Potential confounding variables

Addressing these challenges is central to the project.

