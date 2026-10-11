# Task 1: Predict Restaurant Ratings

## Cognifyz Technologies – Machine Learning Internship

### Project Overview
This project aims to develop a machine learning model to predict the aggregate ratings of restaurants based on their available features. The project involves data preprocessing, exploratory data analysis, regression modeling, model evaluation, and feature importance analysis.

### Objective
To build and evaluate regression models that predict restaurant aggregate ratings using restaurant-related information such as votes, location, price range, cuisines, and other available attributes.

### Dataset
- **Dataset:** Restaurant Dataset
- **Total Records:** 9,551
- **Total Features:** 21
- **Target Variable:** `Aggregate rating`
- **Missing Values:** 9 missing values in the `Cuisines` column

### Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab
- Jupyter Notebook

### Project Workflow

**1. Data Loading and Exploration**
- Loaded the restaurant dataset using Pandas.
- Examined the dataset's dimensions, column names, data types, and missing values.
- Explored the distribution of aggregate restaurant ratings.

**2. Data Preprocessing**
- Handled missing values using imputation.
- Encoded categorical variables using One-Hot Encoding.
- Separated input features and the target variable.
- Removed `Restaurant ID`, `Rating color`, and `Rating text` to avoid irrelevant identifiers and target leakage.
- Split the dataset into training and testing sets using an 80:20 ratio.

**3. Model Building**
The following regression algorithms were trained and evaluated:
- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor

**4. Model Evaluation**
The models were evaluated using:
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R-squared (R²)

### Model Performance

| Model | MSE | RMSE | R² Score |
|---|---:|---:|---:|
| Random Forest | 0.0882 | 0.2969 | 0.9613 |
| Decision Tree | 0.1077 | 0.3281 | 0.9527 |
| Linear Regression | 4,128,523 | 2031.8768 | -1,813,850 |

Random Forest achieved the highest R² score among the evaluated models, with an R² of 0.9613 and an RMSE of 0.2969 on the test set.

Linear Regression performed very poorly with the current feature representation, indicating that it did not adequately model the relationships in this dataset.

### Feature Importance Analysis

Feature importance was analyzed using the Random Forest model.

The analysis showed that:
- `Votes` was by far the most influential feature in the model.
- `Longitude` and `Latitude` had substantially smaller relative importance.
- Other features, including average cost for two, price range, cuisines, and restaurant-related categorical attributes, had comparatively low importance.

Feature importance indicates a model's reliance on features for prediction and does not establish a causal relationship with restaurant ratings.

### Key Findings
- Tree-based models performed well on this dataset.
- Random Forest achieved an R² score of 0.9613.
- Decision Tree also demonstrated strong predictive performance.
- Votes was the dominant feature in Random Forest's feature importance analysis.
- Linear Regression had an extremely high prediction error and a negative R² score.

### Conclusion
The project successfully developed and evaluated machine learning models to predict restaurant aggregate ratings. Among the three models, Random Forest achieved the highest R² score and the lowest prediction error, making it the strongest performer in this evaluation.

The feature importance analysis identified Votes as the dominant predictive feature. These findings demonstrate the ability of tree-based ensemble methods to model complex relationships in the restaurant dataset.

### Project Structure
```text
Task_1_Predict_Restaurant_Ratings/
├── data/
│   └── Dataset.csv
├── notebooks/
│   └── task_1_predict_restaurant_ratings.ipynb
├── outputs/
│   ├── model_comparison.png
│   ├── actual_vs_predicted.png
│   └── feature_importance.png
└── README.md
```

### How to Run
1. Download or clone this repository.
2. Open the notebook in Google Colab or Jupyter Notebook.
3. Upload the restaurant dataset to the required location.
4. Install the required Python libraries if they are not already available.
5. Run the notebook cells sequentially to reproduce the analysis and model evaluation.

### Internship
**Organization:** Cognifyz Technologies  
**Domain:** Machine Learning  
**Task:** Predict Restaurant Ratings

