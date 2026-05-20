#  VIT Chennai Mess Food Predictor

> Can machine learning predict whether today's mess food will be edible… or emotionally damaging?

This project was built for the Kaggle competition:

**The VIT Chennai Mess Food Predictor**

The challenge focuses on building a regression model capable of predicting food quality ratings while avoiding one of the biggest ML mistakes:

# Overfitting

A fictional team of students trained their model on only one week of data collected during a special campus event.  
Their model achieved extremely high training accuracy but completely failed in real-world conditions.

This project aims to build a more generalized and reliable prediction model using proper machine learning practices.

---

#  Objective

Predict the `quality` score of mess food samples using various chemical and numerical features provided in the dataset.

The competition evaluation metric is:

## Mean Squared Error (MSE)

Lower MSE indicates better predictions.

---

#  Machine Learning Workflow

This project follows a complete ML pipeline:

- Data preprocessing
- Exploratory Data Analysis (EDA)
- Feature selection
- Train-validation split
- Random Forest Regression
- Hyperparameter tuning using GridSearchCV
- Prediction generation
- Kaggle submission creation

---

#  Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

#  Dataset Files

- `train.csv`
- `test.csv`
- `sample_submission.csv`

Competition Link:  
https://kaggle.com/competitions/the-vit-chennai-mess-food-predictor

---

# Model Used

## Random Forest Regressor

Final tuned parameters:

```python
RandomForestRegressor(
    n_estimators=100,
    max_depth=10,
    min_samples_split=5,
    random_state=42
)
```

---

# Hyperparameter Tuning

GridSearchCV was used to optimize performance.

```python
param_grid = {
    'n_estimators': [100, 200],
    'max_depth': [None, 10],
    'min_samples_split': [2, 5],
}
```

---

# Performance

| Metric | Score |
|---|---|
| Validation RMSE | 0.7455 |
| Best Cross Validation RMSE | 0.7293 |

---

#  How to Run

## Clone Repository

```bash
git clone https://github.com/vidisha2508/Mess-Food-Quality-Predictor.git
```

## Install Requirements

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Run Notebook

Open the notebook in Kaggle or Jupyter Notebook and run all cells.

---

#  Output

Final predictions are exported as:

```txt
submission_tuned.csv
```

---

#  Future Improvements

- XGBoost / LightGBM
- Feature engineering
- Ensemble methods
- Better cross-validation
- Advanced visualization dashboards

---

#  Author

Built by Vani and Vidisha
