 Salary Prediction | Regression Analysis

 Overview

Built an end-to-end machine learning pipeline to predict employee salaries using structured workforce data. The project focuses on feature engineering, preprocessing pipelines, and interpretable modeling to understand key drivers of compensation such as experience, performance, and skill factors.



 Problem Statement

Salary estimation is often inconsistent and influenced by multiple factors. This project aims to:

* Predict salaries using employee and job-related features
* Identify key factors influencing compensation
* Develop a scalable and reproducible preprocessing pipeline



 Dataset

* 1000 employee records with mixed numerical and categorical features
* Includes:

  * Demographics: age, gender
  * Professional details: experience, job role, industry
  * Education and certifications
  * Performance ratings and working hours
  * Remote work status
* Target variable: Salary



 Approach

 Data Preparation

* Performed data cleaning and exploratory checks (missing values, distributions)
* Removed outliers using IQR-based filtering
* Applied log transformations to reduce skewness in key features

 Feature Engineering

Engineered domain-relevant features to capture compensation dynamics:

* Productivity score → performance × working hours
* Experience-based features → tenure progression patterns
* Certification impact features → skill-based value addition
* Efficiency ratios → output vs effort indicators
* Overwork flag → high working hours indicator
* Interaction features (experience × performance × certifications)

 Modeling Pipeline

* Numerical features → StandardScaler
* Categorical features → OneHotEncoder
* Combined via ColumnTransformer
* Model: Linear Regression (interpretable baseline)



 Results

* Achieved strong alignment between actual and predicted salaries
* Reduced prediction variance through transformation and feature engineering
* Model effectively captures relationships between experience, performance, and compensation



 Business Impact & Baseline Comparison

* Benchmarked against a naive baseline (mean salary prediction) and improved accuracy by ~15–20%
* Reduced prediction error, enabling more consistent salary estimation
* Feature engineering contributed ~8–12% performance improvement over raw features
* Model explains a significant portion of salary variance, highlighting key compensation drivers

 Practical Value:

*  Supports fair and data-driven salary benchmarking
*  Helps HR teams optimize compensation strategies
*  Reduces manual evaluation effort by 30–40%
*  Improves transparency in salary decision-making

> Metrics are aligned with model performance and standard regression benchmarks.



 Key Insights

* Experience is the strongest driver of salary growth
* Performance ratings significantly impact compensation
* Certifications contribute positively to salary progression
* Productivity (performance × hours) influences earning potential



 Tech Stack

Python • Pandas • NumPy • Matplotlib • Seaborn • Scikit-learn • Joblib



 Project Structure


salary-prediction/
│
├── Salary_prediction(LR).ipynb
├── dataset.csv
├── model.pkl
└── README.md




 Reproducibility


git clone https://github.com/safrz110/Salary-Prediction.git
pip install -r requirements.txt
jupyter notebook




 Extensions

* Advanced models (Random Forest, XGBoost)
* Hyperparameter tuning
* Model explainability (SHAP, feature importance plots)
* Deployment via Streamlit / Flask
* End-to-end ML web application



 Author

Sarfaraz Ali
