# dfPredicting Hospital Readmission for Diabetic Patients
Project Overview
This project analyzes a dataset of diabetic patient encounters to predict whether a patient is likely to be readmitted to the hospital. The analysis involves data cleaning, exploratory data analysis, feature engineering, and the application of machine learning models to predict readmission. The goal is to identify key factors that contribute to hospital readmissions and build a model that can help healthcare providers improve patient outcomes.

Dataset
The dataset contains information about diabetic patient encounters, including demographics, admission details, diagnoses, medications, and readmission status. It is sourced from the UCI Machine Learning Repository.

Key Attributes
patient_nbr: Unique identifier for a patient.
race: Patient's race.
gender: Patient's gender.
age: Patient's age group.
admission_type_id: Type of admission (e.g., emergency, urgent).
time_in_hospital: Number of days in the hospital.
num_medications: Number of medications administered.
diag_1, diag_2, diag_3: Primary, secondary, and additional diagnoses.
readmitted: Readmission status (<30, >30, NO).
Analysis and Methodology
The project follows these key steps:

Data Cleaning and Preprocessing:

Handled missing values by replacing placeholders (?) with NaN and dropping columns/rows with excessive missing data.
Removed duplicate entries to ensure data quality.
Converted categorical variables into numerical format using one-hot encoding.
Exploratory Data Analysis (EDA):

Generated descriptive statistics to understand the data distribution.
Created visualizations (histograms, bar charts) to analyze the distribution of key attributes like age, gender, and race.
Used a heatmap to visualize the correlation between different features.
Feature Engineering:

Created new features, such as total_visits (sum of outpatient, emergency, and inpatient visits) and med_change (indicating if there was a change in medication).
Recoded diagnosis codes into broader categories to simplify the analysis.
Modeling:

Split the data into training and testing sets.
Applied machine learning models to predict the readmitted status.
