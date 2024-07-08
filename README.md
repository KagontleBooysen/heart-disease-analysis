## Heart Disease Analysis

## Overview
This project aims to analyze a dataset of medical records to identify patients at high risk of developing heart disease. The dataset contains 303 instances with 14 attributes, including demographic information (age, sex), medical history (blood pressure, cholesterol levels), and a target variable indicating the presence or absence of heart disease.

## Dataset
The dataset used in this analysis is sourced from the UCI Machine Learning Repository, specifically the Heart Disease dataset (UCI ID: 45). It includes data from multiple centers and countries, focusing on distinguishing the presence of heart disease based on various patient attributes. This the link to dataset https://archive.ics.uci.edu/dataset/45/heart+disease 

## Attributes
- age: Age of the patient in years.
- sex: Gender of the patient (1 = male, 0 = female).
- cp: Chest pain type (1 = typical angina, 2 = atypical angina, 3 = non-anginal pain, 4 = asymptomatic).
- trestbps: Resting blood pressure (in mm Hg on admission to the hospital).
- chol: Serum cholesterol level in mg/dl.
- fbs: Fasting blood sugar > 120 mg/dl (1 = true, 0 = false).
- restecg: Resting electrocardiographic results (0 = normal, 1 = having ST-T wave abnormality, 2 = showing probable or definite left ventricular hypertrophy).
- thalach: Maximum heart rate achieved.
- exang: Exercise induced angina (1 = yes, 0 = no).
- oldpeak: ST depression induced by exercise relative to rest.
- slope: The slope of the peak exercise ST segment (1 = upsloping, 2 = flat, 3 = downsloping).
- ca: Number of major vessels colored by fluoroscopy (0-3).
- thal: Thalassemia (3 = normal, 6 = fixed defect, 7 = reversable defect).
- num: Presence of heart disease (0 = absence, 1-4 = presence).

## Analysis Steps
1. Data Loading and Preprocessing:
- Loaded the dataset into a Pandas DataFrame.
- Conducted exploratory data analysis (EDA) to understand the distribution of variables, check for missing values, and handle them appropriately.
  
## Feature Engineering:
- Imputed missing values using median values for 'ca' and 'thal' columns.
- Identified and potentially removed outliers using the Interquartile Range (IQR) method.
  
## Unsupervised Learning Techniques:
- Applied K-means clustering, hierarchical clustering, and DBSCAN to cluster patients based on their medical history.
- Visualized clusters using dimensionality reduction techniques such as PCA and t-SNE.
- Used Gaussian Mixture Models (GMMs) to identify risk factors associated with heart disease.
  
## Evaluation:
- Evaluated clustering performance using metrics like silhouette score and Davies-Bouldin index.
- Compared the performance of different clustering algorithms to choose the most effective one for identifying high-risk patients.
  
## Conclusion:
- Summarized findings and insights from the analysis.
- Discussed potential next steps for further exploration or model refinement.
  
## Dependencies
- Python 3.x
- Pandas, NumPy, Matplotlib, Seaborn for data manipulation and visualization
- Scikit-learn for machine learning algorithms
