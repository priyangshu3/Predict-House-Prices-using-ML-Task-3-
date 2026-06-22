# House Price Prediction Using Machine Learning

##  Project Overview
The primary objective of this project is to model housing valuations based on demographic, architectural, and geographic characteristics using the classic California Housing dataset.

### Technical Safeguards & Highlights:
* Hybrid Data Ingestion Framework:Employs an error-handling `try-except` structure. If a local system drops the `scikit-learn` online fetch due to SSL or network issuer restrictions (common on macOS/Python 3.13), a secure backup mirror automatically switches to an official GitHub CSV stream using `pandas`.
* Missing Value Imputation Engine:Guarantees absolute protection against model calculation drops (`ValueError: Input X contains NaN`) by processing data matrices through a `SimpleImputer` using a median strategy.
* Feature Standardization Pipeline: Applies Z-score standardization (`StandardScaler`) to eliminate variance skewness between diverse scales, such as total `Population` versus relative `AveRooms`.

## Tech Stack & Requirements
The workflow is built entirely in Python using industry-standard packages:

* Environment: Python 3.13+ / Jupyter Notebook (macOS optimized)
* Data Engineering: `pandas`, `numpy`
* Machine Learning & Preprocessing:** `scikit-learn`
* Data Visualization: `matplotlib`, `seaborn`

## Project Workflow

### Data Collection

Loaded the housing dataset containing various features of residential properties and their sale prices.

### Data Preprocessing

* Selected important numerical features.
* Handled missing values using median imputation.
* Prepared data for machine learning.
  
### Train-Test Split

* Split the dataset into training and testing sets.

### Model Evaluation

Evaluated model performance using:

* RMSE (Root Mean Squared Error)
* R² Score

### Data Visualization

Generated:

* Actual vs Predicted House Prices
* Feature Importance Analysis


## Conclusion

A machine learning model was successfully developed to predict house prices using Linear Regression. The project demonstrates the complete machine learning workflow, including data preprocessing, model training, evaluation, and prediction.

## Author

Priyangshu Bagchi

Data Science Intern
