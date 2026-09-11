# OIBSIP - Task 1

## Description
This notebook analyzes the sales dataset to explore trends and generate insights.

## Files
- Veronica Obakunle task 1.ipynb
- Sales (1)_053146.csv

## Tools Used
- Python, Pandas, NumPy, Matplotlib

## Author
Veronica Obakunle


---

# OIBSIP - Task 2

---

# OIBSIP - Task 2

## Description
This project cleans a messy Titanic dataset. It standardizes inconsistent text formatting (Sex, Embarked, Fare, Age), fixes data types, handles missing values column-by-column with documented justification, removes duplicate rows, detects and caps Fare outliers using the IQR method, and produces a clean, analysis-ready dataset.

## Files
- Veronica_Obakunle_task_2.ipynb - Jupyter notebook with full cleaning pipeline
- messy_titanic_dataset-2.csv - Raw input dataset
- titanic_cleaned.csv - Cleaned output dataset

## Key Steps
- Standardized categorical values (Sex, Embarked) and stripped units/symbols from Fare and Age
- Converted invalid Age values (negative or >100) to missing
- Imputed missing values: median for Age/Fare, mode for Embarked, "Unknown" for Cabin, dropped rows missing Name
- Removed 35 duplicate rows and checked for duplicate PassengerId
- Detected 92 Fare outliers via IQR and capped them instead of dropping
- Reduced dataset from 926 rows (945 total nulls) to 887 clean rows (0 nulls)

## Tools Used
- Python, Pandas, NumPy

## Author
Veronica Obakunle



---

# OIBSIP - Task 3

## Description
This project predicts house sale prices using the Ames Housing dataset. It covers data exploration, feature preparation, and building regression models to estimate SalePrice based on property characteristics.

## Files
- Veronica_Obakunle__task_3.ipynb - Jupyter notebook with full analysis
- train.csv - Housing dataset (1460 rows, 81 features)

## Key Steps
- Explored and prepared housing features for modeling
- Trained and compared three regression models: Linear Regression, Ridge, and Lasso
- Evaluated models using MSE, RMSE, and R2 score
- Visualized top positive and negative feature coefficients driving price predictions

## Results
| Model | RMSE | R2 |
|---|---|---|
| Linear Regression | 34,643.93 | 0.8435 |
| Ridge (alpha=1.0) | 34,608.62 | 0.8438 |
| Lasso (alpha=1000) | 37,523.89 | 0.8164 |

Ridge regression performed best, slightly outperforming plain Linear Regression while regularizing the coefficients.

## Tools Used
- Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

## Author
Veronica Obakunle
