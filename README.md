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


# Methodology 
# Data Preprocessing:

1. Remove instances with missing values or incomplete data

2. Encode categorical variables using one-hot encoding or label encoding

3. Standardize numerical variables using Z-score normalization

# Feature Selection:

1. Use domain knowledge and exploratory data analysis to identify relevant features

2. Apply statistical techniques like correlation analysis, chi-square test, or feature
importance score to select important features.

# Model Training:

1. Split the dataset into training and validation sets

2. Fit a logistic regression model to the training data

3. Evaluate the model's performance on the validation set using metrics such as
accuracy, precision, recall, and F1 score.

4. Tune the model hyperparameters using techniques to improve the model's
performance.

#  Model Interpretation:

1. Interpret the model coefficients to understand the impact of each feature on the
target variable.

2. Analyze the model's predictions using tools like confusion matrix, ROC curve, and
precision-recall curve to gain insights into the model's behavior.

3. Use the model to generate predictions on new data and evaluate its performance on
an independent test set.

===============================================================================================
# Analysis:

# Data Preprocessing:

1. There are 13 numerical columsn and 37 categorical columns

2. Remove instances with missing values or incomplete data

3. 'Encounter_id', 'patient_nbr', 'weight', 'examide', 'citoglipton', 'diag_1',
'diag_2', 'diag_3' are removed.

4. Missing values are termed as ‘?’ which are replaced with NA

5. Encode categorical variables using one-hot encoding or label encoding

6. Standardize numerical variables using Z-score normalization

# Statistical Analysis:
# Multivariate Analysis Using pairplot()
# Feature Selection
1. Use domain knowledge and exploratory data analysis to identify relevant
features

2. Apply statistical techniques like correlation analysis, chi-square test, or
feature importance score to select important features.

# Feature Engineering
# Model Training
# Model Performance
# Model Interpretation:
1. Interpret the model coefficients to understand the impact of each feature on
the target variable.

2. Analyze the model's predictions using tools like confusion matrix, ROC
curve, and precision-recall curve to gain insights into the model's behavior.

3. Use the model to generate predictions on new data and evaluate its
performance on an independent test set
   
# Bias and Variance Tradeoff
1. Using Validation Set Approach

We evaluated our models during the modeling phase using a separate validation
dataset, shielding them from the test data. By utilizing the validation data to
evaluate many models, we were able to select the most accurate one to use for
making predictions about the test data. We specifically divided the data into three
parts: training (70%), testing (15%), and validation (15%).

2. Random shuffling of data
To prevent the model from being trained on only one category of labels, we
randomly sampled the data before dividing it into training and testing sets. We
utilized balanced data during the training procedure to prevent the model from
being biased towards any one category and to reduce the generalization error.

3. Hyper Parameter Tuning
By experimenting with different combinations of hyperparameters, such as
learning rate and tolerance for logistic regression and number of neurons in hidden
layers, batch size, and epochs for neural network models, we have evaluated the
performance of our models. The models' performance and error rates were
improved and reduced by the adjustment of these hyperparameters.


# Conclusion

Since the health care data provides important information, it is inappropriate to
ignore any component that might first seem unnecessary. After examining the data,
we found a number of connections that made sense and gave us a chance to do
feature engineering. We were able to minimize the amount of features while
maintaining the model's performance by combining different characteristics.

In the course of our investigation, we also discovered a few characteristics that
significantly affect readmission prediction, such as "number_inpatients." We may
concentrate on these crucial elements by recognizing them, which will increase the
model's accuracy and help us make better choices. Feature engineering reduces
noise and identifies the most important characteristics, which helps to simplify the
data and enhance the performance of the model.


