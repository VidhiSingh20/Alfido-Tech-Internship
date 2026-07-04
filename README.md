<<<<<<< HEAD




Build a machine learning classification model to predict Iris flower species using sepal and petal measurements.



Iris Classification Dataset



* sepal_length
* sepal_width
* petal_length
* petal_width



* species



Performed:

* Class distribution visualization
* Pairplot for class separability
* Correlation heatmap
* Feature-wise boxplots


1. K-Nearest Neighbors (KNN)
2. Logistic Regression
3. Decision Tree



* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix



| Model               | Accuracy |
| ------------------- | -------- |
| KNN                 | 93.33%   |
| Logistic Regression | 93.33%   |
| Decision Tree       | 93.33%   |



Logistic Regression


`iris_best_model.joblib`



```python
import joblib
import pandas as pd

model = joblib.load("iris_best_model.joblib")

sample = pd.DataFrame(
    [[5.1, 3.5, 1.4, 0.2]],
    columns=[
        "sepal_length",
        "sepal_width",
        "petal_length",
        "petal_width"
    ]
)

prediction = model.predict(sample)

print(prediction[0])
```

## Conclusion

The Iris classification model was successfully developed using multiple machine learning algorithms. All models achieved an accuracy of 93.33%, and Logistic Regression was selected as the final model for deployment and inference.
=======
# Alfido Tech Internship

This repository contains the machine learning tasks completed during my internship at Alfido Tech.

## Task 1 – Iris Flower Classification

### Objective
Build a machine learning classification model to predict Iris flower species.

### Algorithms Used
- Logistic Regression
- Decision Tree
- Random Forest

### Technologies
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Task 2 – House Price Prediction

### Objective
Build a regression model to predict house prices using property features.

### Algorithms Used
- Random Forest Regressor
- Gradient Boosting Regressor

### Feature Engineering
- Sale Year
- Sale Month
- House Age
- Renovation Age
- Total Square Feet
- Log Transformation of Target Variable

### Evaluation Metrics
- RMSE
- MAE
- R² Score

### Best Model
Gradient Boosting Regressor

**Performance**
- R² Score: 0.78
- RMSE: 0.21
- MAE: 0.15

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Author

**Vidhi Singh**
>>>>>>> afb05ab (Added Task 1 and Task 2 projects)
