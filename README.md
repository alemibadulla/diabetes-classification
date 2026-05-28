# diabetes-classification
Binary classification model to predict diabetes using Random Forest. Includes proper preprocessing pipeline with no data leakage. Stack: Python, Scikit-learn, Pandas.
📊 About
Binary classification model to predict whether a patient has diabetes based on medical and demographic features.
🎯 Goal
Automatically classify patients (diabetes / no diabetes) with high accuracy using a robust, production-ready pipeline.
📁 Data

Medical dataset: age, gender, BMI, hypertension, heart disease, smoking history, HbA1c level, blood glucose level

🛠️ Stack
Python Pandas Scikit-learn (RandomForestClassifier, StandardScaler, OneHotEncoder, ColumnTransformer)
🔍 What was done

Exploratory data analysis: data types, missing values, unique categorical values
Preprocessing via ColumnTransformer: StandardScaler for numeric, OneHotEncoder (drop='first') for categorical features
Stratified train/validation split (80/20) to preserve class balance
Random Forest training, evaluation via accuracy and full classification report
Test dataset scoring and predictions exported to CSV

📌 Results

No data leakage: transformations applied correctly — fit only on train, transform on val and test
Reproducible and scalable pipeline ready for deployment

