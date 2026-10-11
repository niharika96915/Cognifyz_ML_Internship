# Task 3: Cuisine Classification

## Overview
This project uses machine learning to predict a restaurant's primary cuisine based on restaurant features such as city, price range, average cost, aggregate rating, votes, table booking, and online delivery.

## Dataset
- Source file: `Dataset.csv`
- Original dataset: 9,551 restaurant records
- Records after cleaning: 9,542
- Records used for classification: 9,298
- Cuisine classes: 48

## Technologies Used
- Python
- Pandas and NumPy
- Scikit-learn
- Matplotlib
- Joblib
- Google Colab

## Methodology
1. Explored and cleaned the dataset.
2. Extracted the primary cuisine from the cuisine column.
3. Excluded cuisine classes with fewer than 10 examples.
4. Split the data into 80% training and 20% testing sets.
5. Applied categorical encoding and numerical scaling.
6. Trained and compared Random Forest and Logistic Regression models.
7. Evaluated performance using accuracy, precision, recall, F1-score, and a confusion matrix.

## Results
- Original Random Forest accuracy: 24.14%
- Improved Random Forest accuracy: 35.70%
- Improved Random Forest weighted F1-score: 0.247
- Logistic Regression accuracy: 3.12%

The improved Random Forest performed better in overall accuracy. However, the confusion matrix shows that predictions are biased toward common cuisine classes, and performance varies significantly across cuisines.

## Project Files
- `data/`: Dataset
- `notebooks/`: Google Colab notebook
- `outputs/`: Trained model and confusion matrix

## Conclusion
This project demonstrates a complete multiclass classification workflow, including data cleaning, preprocessing, model training, model comparison, and evaluation. The results also highlight the challenges of class imbalance and predicting cuisines with limited examples.

## Disclaimer
The model is an educational project and should not be treated as a reliable production-level cuisine prediction system.
