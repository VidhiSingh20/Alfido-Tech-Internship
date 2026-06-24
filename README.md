# Task-1 Iris Classification

## Objective

Build a machine learning classification model to predict Iris flower species using sepal and petal measurements.

## Dataset

Iris Classification Dataset

### Features

* sepal_length
* sepal_width
* petal_length
* petal_width

### Target

* species

## Exploratory Data Analysis (EDA)

Performed:

* Class distribution visualization
* Pairplot for class separability
* Correlation heatmap
* Feature-wise boxplots

## Models Implemented

1. K-Nearest Neighbors (KNN)
2. Logistic Regression
3. Decision Tree

## Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

## Results

| Model               | Accuracy |
| ------------------- | -------- |
| KNN                 | 93.33%   |
| Logistic Regression | 93.33%   |
| Decision Tree       | 93.33%   |

## Best Model

Logistic Regression

## Saved Model

`iris_best_model.joblib`

## Inference Example

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
