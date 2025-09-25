The dataset used in this lab is sourced from the Kaggle Dataset Repository**:  
[Students Dropout and Academic Success](https://www.kaggle.com/datasets/mahwiz/students-dropout-and-academic-success-dataset).  

It contains student records** and features, including demographic information, academic performance, and enrollment details.  
The target column shows whether a student dropped out, graduated, or remained enrolled**.  

For this lab, I focused on three specific columns:  
- `curricular_units_1st_sem_grade` → average grade from the first semester  
- `curricular_units_2nd_sem_approved` → number of approved units in the second semester  
- `curricular_units_2nd_sem_grade` → average grade in the second semester (this is the target variable)  

---

##  Files in this Repo
- `Students_Dropout_Corrected.ipynb` → Jupyter notebook with all steps (loading data, cleaning, analysis, regression, evaluation).  
- `students_regression_subset.csv` → A smaller version of the dataset used for the regression task (optional).  

---

##  Steps Followed
1. Import libraries → pandas, numpy, matplotlib, seaborn, scikit-learn  
2. Load dataset → with `sep=";"` because the file uses semicolons  
3. Explore data → checked shape, info, describe, and missing values  
4. Clean column names → converted to lowercase and replaced spaces with underscores  
5. Handle missing values → removed rows with `.dropna()`  
6. Build new DataFrame (`df_reg`) → selected 2 features and 1 target  
7. Visualize data → histograms and scatterplots to understand distributions and relationships  
8. Train regression model → Linear Regression with a train/test split  
9. Evaluate model → calculated R², MAE, and RMSE 
10. Diagnostic plots → Predicted vs Actual and Residuals vs Predicted  

---

## Results
- Both chosen features showed a positive relationship with the target.  
- The regression model performance:  
  - R²: 0.62  
  - MAE: 1.35  
  - RMSE: 1.90  
- Plots showed residuals mostly centered around zero, suggesting a reasonable model fit.  

---

## Reflection
This project helped me practice:  
- Cleaning and preparing a dataset for analysis  
- Building a smaller DataFrame with selected features  
- Training and evaluating a regression model  
- Interpreting model results with metrics and plots  
