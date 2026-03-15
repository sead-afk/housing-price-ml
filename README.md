# Housing Price Prediction using Machine Learning

## Project Overview

This project builds a machine learning model to predict residential house prices using the Ames Housing dataset. The goal is to explore the full machine learning workflow, including data exploration, preprocessing, feature engineering, model training, and evaluation.

The dataset contains detailed information about residential homes, such as property size, location, construction quality, and other features that influence the final sale price.

The project demonstrates how machine learning techniques can be used to estimate house prices based on property characteristics.

---

## Dataset

The dataset comes from the Kaggle competition:

* House Prices: Advanced Regression Techniques

It includes:

* **79 explanatory variables**
* **1460 training observations**
* The target variable **SalePrice**

Example features include:

* Overall house quality
* Living area size
* Garage capacity
* Year built
* Basement area
* Neighborhood

---

## Project Workflow

The project follows a standard machine learning pipeline:

### 1. Data Exploration (EDA)

Exploratory Data Analysis was performed to understand the structure of the dataset and identify important relationships between features and the target variable.

Key analyses included:

* Distribution of house prices
* Missing value analysis
* Correlation analysis between numerical variables
* Identification of the most influential features

---

### 2. Data Preprocessing

Data preprocessing steps include:

* Handling missing values using **median imputation** for numerical features
* Filling missing categorical values with the **most frequent category**
* Converting categorical variables into numerical representations using **one-hot encoding**

These steps are implemented using preprocessing pipelines from **scikit-learn**.

---

### 3. Feature Engineering

Features were categorized into:

* **Numerical variables**
* **Categorical variables**

Appropriate preprocessing techniques were applied to each type using a **ColumnTransformer pipeline**.

---

### 4. Model Training

The model used in this project is a **Random Forest**, which is an ensemble method that combines multiple decision trees to improve prediction accuracy and reduce overfitting.

The model was trained using a train-validation split to evaluate performance on unseen data.

---

### 5. Model Evaluation

Model performance was evaluated using:

* **Mean Absolute Error**

MAE measures the average difference between predicted and actual house prices.

Lower MAE values indicate better model performance.

---

### 6. Prediction

The trained model was used to generate predictions for the test dataset and produce a submission file compatible with the Kaggle competition.

---

## Technologies Used

This project was implemented using the following tools and libraries:

* Python
* pandas
* NumPy
* scikit-learn
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## Project Structure

```
housing-price-ml/
│
├── data/
│   ├── test.csv
│   └── train.csv
│
├── notebooks/
│   └── housing_price_analysis.ipynb
│
├── outputs/
│   └── submissions/
│
└── README.md
```

---

## Key Learning Outcomes

This project demonstrates:

* Practical implementation of a machine learning pipeline
* Data cleaning and preprocessing techniques
* Handling missing data
* Encoding categorical variables
* Training and evaluating regression models
* Structuring a machine learning project for reproducibility

---

## Future Improvements

Potential improvements include:

* Hyperparameter tuning
* Testing additional models such as gradient boosting
* Feature engineering improvements
* Cross-validation for more robust evaluation
* Model deployment via a simple web application

---

## Author

Sead Gacanovic
