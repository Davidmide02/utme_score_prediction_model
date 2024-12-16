# Predicting Student Performance on JAMB (utme exam)


#### Overview:
This project focuses on building a machine learning model to predict students' scores on standardized tests based on various factors such as hours of study, type of school, extra tutorial participation, distance to school, and parent education level. The objective is to identify the key contributors to student performance and provide actionable insights for improving outcomes.
---

#### Dataset Description
- The dataset contains information about students, their demographic and academic background, and their performance on a standardized test. Below are the details of the dataset:
- Columns
1. hours_of_study: (Numerical) Number of hours the student spends studying daily.
2. type_of_school: (Categorical) Public or private school attended by the student.
3. extra_tutorial: (Categorical) Indicates whether the student attends extra tutorial classes (Yes/No).
4. distance_to_school: (Numerical) Distance from the student’s home to school in kilometers.
5. parent_education_level: (Categorical) Highest education level of the parents (e.g., High School, Bachelor's, Master's).
6. score: (Numerical) The student's score on the standardized test (Target variable).

---

#### Problem:
- Jamb candidates 

This a machine learning project to determine factor(s) that affects the perfomance of candidate when it comes to jamb. using the [jamb-2024 dataset](./notebook.ipynb)

#### Aim:
1. Build a predictive model to estimate students' scores based on the provided features.
2. Identify which factors significantly impact performance.
3. Provide actionable insights for policymakers, educators, and parents to enhance student success.


 


#### Project Workflow
1. Exploratory Data Analysis (EDA)
- - Analyze the distribution of scores and other features.
- - Explore relationships between the target variable (score) and other columns.
- - Check for missing values, outliers, and data imbalances.


2. Data Preprocessing
- - Handle missing values using appropriate strategies (e.g., mean/mode imputation or predictive imputation).
- - Encode categorical variables using techniques like One-Hot Encoding or Label Encoding.
- - Normalize/scale numerical columns like hours_of_study and distance_to_school to standardize the feature ranges.


3. Feature Engineering
- - Create new features, if relevant, such as study_efficiency (score per hour studied).
- - Encode missingness where necessary as a separate feature.


4. Model Selection and Training
- - Train various machine learning models, such as:
- - Linear Regression
- - Decision Trees
- - Random Forest
- - Gradient Boosting (e.g., XGBoost, LightGBM)
- - Evaluate the performance of models using appropriate metrics (e.g., RMSE, R² score).


5. Model Evaluation
- - Use cross-validation to ensure robustness.
- - Interpret the feature importance to understand which factors drive performance.


6. Insights and Recommendations
- - Analyze the model's findings and provide actionable insights for stakeholders.
---

#### Technologies Used
1. Programming Language: Python
2. Libraries:
- - - Data Analysis: Pandas, NumPy
- - - Visualization: Matplotlib, Seaborn
- - - Machine Learning: Scikit-learn, XGBoost, LightGBM

---

#### How to Run the project

1. Setup the  Environment 
- install the required dependencies
```
pip install -r requirements.txt

```
2. Run the [notebook](notebook.ipynb)



Open the Jupyter Notebook (student_performance_prediction.ipynb) to see the step-by-step implementation.
Alternatively, use the script file:
bash
Copy code
python train_model.py
3. Dataset
Place the dataset file (student_scores.csv) in the data/ directory.
Update the config.py file with the correct dataset path if needed.
4. Model Evaluation
After running the notebook or script, view the model performance metrics in the console or the notebook outputs.
Results
Best Model: [Insert the best-performing model, e.g., Random Forest]
Metrics:
RMSE: [Value]
R² Score: [Value]
Key Factors Impacting Performance:
[List top factors like hours_of_study, type_of_school, etc.]
Insights
Students attending extra tutorials showed an average improvement of X%.
Parental education level has a moderate influence on test scores.
[Insert other insights.]
Future Work
Expand the dataset with additional features like socioeconomic status, teacher quality, or extracurricular activities.
Experiment with deep learning models for potential performance improvements.
Deploy the model as an API for real-time score prediction.
Contributors
David [Your Last Name] - [Your Role]
[Other Contributors] - [Their Role]
License
This project is licensed under the MIT License.

Acknowledgments
Special thanks to [Dataset Source] for providing the data used in this project.