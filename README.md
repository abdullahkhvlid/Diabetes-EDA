# Diabetes Data Analysis and Visualization
Overview
This project provides an exploratory data analysis (EDA) on the Pima Indians Diabetes Dataset, aiming to understand patterns, trends, and correlations between various health-related features and the likelihood of diabetes.
The analysis includes thorough data cleaning, visualization, and statistical summaries to extract actionable insights.

The dataset used contains medical predictor variables and a binary target variable indicating whether a patient has diabetes.

Dataset Information
Source: diabetes.csv
Number of Rows: 768
Number of Columns: 9

Features:

Pregnancies: Number of times pregnant

Glucose: Plasma glucose concentration (mg/dL)

BloodPressure: Diastolic blood pressure (mm Hg)

SkinThickness: Triceps skinfold thickness (mm)

Insulin: 2-Hour serum insulin (mu U/ml)

BMI: Body mass index (weight in kg/(height in m)^2)

DiabetesPedigreeFunction: Diabetes pedigree function (likelihood based on family history)

Age: Age in years

Outcome: 0 = No diabetes, 1 = Diabetes

Workflow
1. Data Loading
Read dataset using Pandas.

Inspected dataset dimensions, column names, and data types.

2. Data Cleaning
Identified invalid values (0) in specific columns that cannot logically be zero (Glucose, BloodPressure, SkinThickness, Insulin, BMI).

Replaced these invalid values with NaN.

Filled missing values with the median of each column to reduce skewness.

3. Exploratory Data Analysis (EDA)
Pairplot Analysis to visualize relationships between features and the Outcome.

Count Plot for diabetes vs. non-diabetes cases.

Histograms for age and BMI distributions.

Box Plots to compare glucose, blood pressure, and age against diabetes outcome.

Correlation Heatmap to identify strongest relationships between variables.

Key Visualizations
Outcome Distribution
Shows the balance between diabetic and non-diabetic cases.

Age Distribution
Highlights common age ranges for patients and the spread across the dataset.

BMI Distribution
Identifies the BMI profile of patients and potential links to diabetes.

Glucose vs. Outcome
Demonstrates clear separation in glucose levels between diabetic and non-diabetic groups.

Blood Pressure vs. Outcome
Explores blood pressure variation in relation to diabetes diagnosis.

Age vs. Outcome
Shows how age correlates with higher chances of diabetes.

Correlation Matrix
Summarizes numerical relationships between all features.

Insights
Higher glucose levels are strongly associated with diabetes occurrence.

BMI and Age also show notable differences between diabetic and non-diabetic patients.

Blood Pressure does not have as strong a correlation as Glucose or BMI.

Data preprocessing significantly improves the reliability of visualizations.

Technologies Used
Python

Pandas for data manipulation

NumPy for numerical operations

Matplotlib and Seaborn for data visualization

How to Run
Clone this repository:
git clone https://github.com/your-username/diabetes-analysis.git
Install dependencies:
pip install pandas numpy matplotlib seaborn

Place the diabetes.csv file in the project directory.

Run the Jupyter Notebook or Python script to reproduce results.

Conclusion
This project provides a complete exploratory analysis pipeline for medical datasets. The methodology applied here can be adapted to other health-related datasets for pattern detection and hypothesis generation. By understanding the distribution and correlation of health metrics, we can take a data-driven approach to disease prediction and prevention.

