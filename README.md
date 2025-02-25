# HealthCare Analytics - Machine Learning

## Predicting Diabetic Patient Readmission Using Machine Learning

### Problem Definition
Hospital readmissions pose a significant burden on healthcare systems, particularly for diabetic patients. This study aims to enhance patient safety and optimize resource allocation by analyzing historical data on diabetes management in U.S. hospitals. The primary challenge lies in dealing with missing values, inconsistent records, and high-dimensional data.

### Goal
The objective is to predict the risk of readmission for diabetic patients within 30 days based on various patient and hospital characteristics.

## Dataset
The dataset used for this study is from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/diabetes+130-us+hospitals+for+years+1999-2008). It contains over 100,000 hospital admissions from 130 U.S. hospitals between 1999 and 2008. The dataset comprises 37 categorical and 13 numerical features, including patient demographics, medical history, hospital procedures, and prescribed medications.

### Key Features
- **Demographics**: Age, Gender
- **Hospitalization Details**: Admission Type, Time in Hospital, Medical Specialty
- **Procedures & Medications**: Number of Lab Procedures, Number of Medications, Medication Changes
- **Target Variable**: Readmission within 30 days (Yes/No)

## Methodology

### Data Preprocessing
1. Handle missing values by removing or imputing missing data.
2. Encode categorical variables using one-hot encoding or label encoding.
3. Standardize numerical variables using Z-score normalization.
4. Remove irrelevant or redundant features such as 'Encounter_id', 'patient_nbr', 'weight', etc.

### Feature Selection
1. Perform exploratory data analysis to identify significant features.
2. Use statistical methods such as correlation analysis and chi-square tests.
3. Rank feature importance based on predictive power.

### Model Training
1. Split the dataset into training (70%), validation (15%), and test (15%) sets.
2. Train a **Logistic Regression** model as the baseline.
3. Evaluate performance using **accuracy, precision, recall, and F1-score**.
4. Optimize the model using hyperparameter tuning.

### Model Interpretation
1. Analyze feature importance to understand the impact of each variable.
2. Use evaluation metrics such as the **confusion matrix, ROC curve, and precision-recall curve**.
3. Generate predictions on new data to assess model generalization.

## Bias and Variance Tradeoff
1. **Validation Set Approach**: We use a separate validation set to avoid overfitting.
2. **Random Data Shuffling**: Ensures balanced training and testing data.
3. **Hyperparameter Tuning**: Experimenting with different parameter settings to optimize performance.

## Results & Conclusion
- Effective feature engineering improved model performance while reducing dimensionality.
- Key factors influencing readmission include **number of inpatients, medication changes, and length of stay**.
- The final model provides a useful tool for predicting readmissions, aiding healthcare professionals in decision-making.

By leveraging machine learning, we can enhance patient outcomes and reduce hospital readmissions, leading to more efficient healthcare resource utilization.

---

## Future Work
- Experiment with advanced models like **Random Forest, XGBoost, or Neural Networks**.
- Investigate additional patient history and external factors affecting readmission rates.
- Deploy the model in a real-world hospital setting for further validation.

---

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Authors & Acknowledgments
- This project is based on publicly available healthcare data and follows ethical guidelines for medical data analysis.

## How to Contribute
Contributions are welcome! If you'd like to improve this project, please fork the repository and submit a pull request.

