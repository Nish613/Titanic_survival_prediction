# Titanic Survival Prediction

This project predicts whether a passenger survived the Titanic disaster using different machine learning classification models.

The aim of this project is to compare multiple ML models on the same dataset and evaluate which model performs better for Titanic survival prediction.

## Dataset

The dataset used is the **Titanic dataset from the Seaborn library**.

It contains passenger-related information such as:

- Passenger class
- Sex
- Age
- Number of siblings/spouses aboard
- Number of parents/children aboard
- Fare
- Embarked location
- Whether the passenger was alone

The target variable is:

- `survived`

where:

- `0` means the passenger did not survive
- `1` means the passenger survived

## Models Used

The following machine learning models were trained and compared:

1. Logistic Regression
2. K-Nearest Neighbors
3. Support Vector Machine
4. Decision Tree
5. Naive Bayes

## Data Preprocessing

The following preprocessing steps were performed:

- Loaded the Titanic dataset using Seaborn
- Checked for missing values
- Removed unnecessary columns
- Filled missing values
- Converted categorical columns into numerical form using one-hot encoding
- Split the data into training and testing sets
- Scaled numerical features where required

The numerical columns scaled were:

- `pclass`
- `age`
- `sibsp`
- `parch`
- `fare`

## Model Performance

| Model | Accuracy |
|---|---:|
| K-Nearest Neighbors | 82.68% |
| Support Vector Machine | 81.56% |
| Decision Tree | 80.45% |
| Logistic Regression | 79.33% |
| Naive Bayes | 77.09% |

## Confusion Matrices

### Logistic Regression

```text
[[90, 15],
 [22, 52]]
```

### K-Nearest Neighbors

```text
[[96,  9],
 [22, 52]]
```

### Support Vector Machine

```text
[[92, 13],
 [20, 54]]
```

### Decision Tree

```text
[[89, 16],
 [19, 55]]
```

### Naive Bayes

```text
[[79, 26],
 [15, 59]]
```

## Best Model

The best performing model was **K-Nearest Neighbors**, with an accuracy of **82.68%**.

## Libraries Used

- Python
- NumPy
- Pandas
- Seaborn
- Matplotlib
- Scikit-learn

## Conclusion

In this project, five different classification models were applied to predict Titanic passenger survival.

Among all the models tested, **K-Nearest Neighbors gave the highest accuracy of 82.68%**. Support Vector Machine and Decision Tree also performed well.

This project helped in understanding basic classification models, preprocessing, model training, prediction, confusion matrices, and accuracy comparison.
