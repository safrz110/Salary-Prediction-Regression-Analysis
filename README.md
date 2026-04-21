Project Overview
This project builds a Salary Prediction model using Machine Learning techniques. The goal is to predict employee salaries based on experience, education, job role, performance, and other workplace features.
The model uses feature engineering, preprocessing pipelines, and Linear Regression to improve prediction accuracy.

 Dataset Information
The dataset contains 1000 employee records with the following features:
Employee details (age, experience, gender)
Job role & industry
Education level
Performance rating
Certifications
Working hours
Remote work status
Target variable: Salary

 Tools & Technologies
Python 
Pandas & NumPy
Seaborn & Matplotlib 
Scikit-learn 
Jupyter Notebook
Joblib
 
Exploratory Data Analysis (EDA)
Checked dataset shape, info, and missing values
Visualized salary distribution using histograms
Correlation analysis using heatmap
Outlier removal using IQR method

 Feature Engineering
New features were created to improve model performance:
Log transformations of working hours and experience
Productivity score (performance × hours)
Experience-based features
Certification impact features
Career start age analysis
Overwork flag
Efficiency ratios
Interaction features (experience × certifications × performance)

 Data Preprocessing
Separated numerical and categorical features
Applied:
StandardScaler for numerical data
OneHotEncoder for categorical data
Combined using ColumnTransformer

 Model Building
Train-test split (80/20)
Model used: Linear Regression
Built using Scikit-learn Pipeline:
Preprocessing → Model

 Model Evaluation
Performance metrics:
R² Score
Mean Absolute Error (MAE)
Root Mean Squared Error (RMSE)

 Results Visualization
Actual vs Predicted Salary Scatter Plot
Feature importance using model coefficients
 Key Insights
Experience strongly impacts salary
Performance rating significantly affects earnings
Certifications improve salary prediction accuracy
Working hours and productivity are important factors

Feature Importance Analysis
Model coefficients were analyzed to understand which features influence salary the most.

 How to Run This Project
git clone https://github.com/your-username/Salary_Prediction.git
cd Salary_Prediction
pip install -r requirements.txt

Run notebook:
jupyter notebook Salary_prediction(LR).ipynb

 Author
Sarfaraz Ali

 Support
If you like this project:
Give it a ⭐ on GitHub
Fork it for improvements

 Optional Improvements
Try advanced models (Random Forest / XGBoost)
Add hyperparameter tuning
Deploy using Streamlit or Flask
Convert into end-to-end ML web app
