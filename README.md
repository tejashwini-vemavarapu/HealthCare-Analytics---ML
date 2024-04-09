# HealthCare-Analytics---ML
Predicting Diabetic patient Readmission using Machine Learning

# Problem Definition
The study aims to improve patient safety by analyzing historical patterns in diabetes management among patients admitted to US hospitals, with the goal of conserving resources and money.

Clinical data databases pose challenges due to missing values, inconsistent or partial records, and high dimensionality.

The dataset includes both category and numeric columns, some of which are inconsistent or have missing values, and prescription drug information was also included to examine its potential impact on readmission rates.

#Goal

To predict the risk of readmission for diabetic patients in US hospitals based on
various patient and hospital characteristics.

# Dataset
https://archive.ics.uci.edu/ml/datasets/diabetes+130-us+hospitals+for+years+1999-
2008

# Dataset Description

The diabetes dataset from the UCI Machine Learning Repository contains data on
over 100,000 hospital admissions of patients with diabetes to 130 hospitals in the
United States from 1999 to 2008. The goal of this analysis is to build a logistic
regression model to predict whether a patient will be readmitted within 30 days of
their initial hospitalization based on their demographic information, medical
history, and medications. There are 37 categorical and 13 numerical variables.

1. Age: age of patient in years

2. Gender: gender of patient (male or female)

3. Admission_type_id: identifier corresponding to the type of admission
(emergency,
urgent, elective, etc.)

4. Time_in_hospital: number of days between admission and discharge

5. Medical_specialty: specialty of the admitting physician

6. Num_lab_procedures: number of lab procedures performed during the stay

7. Num_procedures: number of non-lab procedures performed during the stay

8. Num_medications: number of distinct medications administered during the
stay

9. Change: whether there was a change in medication during the stay (yes or
no)

10.DiabetesMed: whether any diabetes medication was prescribed (yes or no)

11.Readmitted: whether the patient was readmitted within 30 days (yes, no, or
>30)

The dependent variable for the logistic regression model is the binary variable
"Readmitted", which can be coded as 1 for patients who were readmitted within 30
days and 0 for those who were not.

