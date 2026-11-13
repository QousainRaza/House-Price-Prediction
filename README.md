# 🏡 House Price Prediction

**A Machine Learning project that predicts residential house prices using property characteristics and Linear Regression.**

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-Machine%20Learning-F7931E?logo=scikitlearn)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter)

## 📌 Project Overview

House Price Prediction is a machine learning project focused on estimating residential property prices based on selected housing characteristics.

The project uses Python and Scikit-learn to perform data preprocessing, feature selection, categorical encoding, model training, and evaluation.

A **Linear Regression** model is trained to understand the relationship between property features and their sale prices. The project demonstrates a practical machine learning workflow, from raw dataset exploration to model evaluation.

## 🎯 Project Objectives

- Explore and understand housing data.
- Identify and handle missing values.
- Perform data cleaning and preprocessing.
- Select relevant features for prediction.
- Apply One-Hot Encoding to categorical variables.
- Train a Linear Regression model.
- Evaluate model performance using regression metrics.

## ✨ Key Features

- **Data Exploration:** Inspect dataset structure, columns, data types, and missing values.
- **Data Cleaning:** Handle missing values and prepare data for modeling.
- **Feature Selection:** Use 11 selected features related to property characteristics.
- **Categorical Encoding:** Transform categorical variables using OneHotEncoder.
- **Model Training:** Train a Linear Regression model using an 80/20 train-test split.
- **Model Evaluation:** Evaluate predictions using MAE, MSE, RMSE, R², and Adjusted R².

## 🛠️ Technology Stack

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Data Manipulation | Pandas, NumPy |
| Data Visualization | Seaborn |
| Machine Learning | Scikit-learn |
| Model | Linear Regression |
| Categorical Encoding | OneHotEncoder |
| Development Environment | Jupyter Notebook |

## 📊 Dataset & Selected Features

The project uses `HousePricePrediction.csv`, which contains residential property information and the target variable `SalePrice`.

The following 11 features are used for model training:

| Feature | Description |
|---|---|
| MSSubClass | Building class |
| MSZoning | Zoning classification |
| LotArea | Lot area |
| LotConfig | Lot configuration |
| BldgType | Building type |
| OverallCond | Overall house condition |
| YearBuilt | Original construction year |
| YearRemodAdd | Remodeling or addition year |
| Exterior1st | Exterior covering material |
| BsmtFinSF2 | Type 2 finished basement area |
| TotalBsmtSF | Total basement area |

`Id` is excluded because it is an identifier rather than a meaningful predictive feature.

Rows with missing `SalePrice` values are separated from the labeled training dataset and are not used for supervised model training.

## ⚙️ Machine Learning Workflow

1. **Data Loading:** Load the dataset using Pandas.
2. **Data Inspection:** Examine data types, missing values, and dataset structure.
3. **Data Cleaning:** Handle missing values in selected features.
4. **Feature Preparation:** Separate labeled training data from rows with missing target values.
5. **Feature Selection:** Separate independent variables from the target variable.
6. **Train-Test Split:** Split the labeled dataset into 80% training and 20% testing data using `random_state=42`.
7. **Categorical Encoding:** Apply OneHotEncoder to categorical features.
8. **Model Training:** Train the Linear Regression model.
9. **Model Prediction:** Generate predictions using the test dataset.
10. **Model Evaluation:** Evaluate the model using regression performance metrics.

## 📈 Model Performance

The Linear Regression model was evaluated using the test dataset.

| Evaluation Metric | Result |
|---|---:|
| Mean Absolute Error (MAE) | 32,027.90 |
| Mean Squared Error (MSE) | 2,569,602,557.67 |
| Root Mean Squared Error (RMSE) | 50,691.25 |
| R² Score | 0.6650 |
| Adjusted R² Score | 0.5938 |

### Understanding the Results

- **MAE:** The average absolute prediction error is approximately 32,028 price units.
- **RMSE:** The root mean squared prediction error is approximately 50,691 price units.
- **R² Score:** The model explains approximately 66.5% of the variation in house prices in the test dataset.
- **Adjusted R²:** The adjusted score is approximately 59.38%, accounting for the number of predictors.

These results establish a baseline for further model experimentation and improvement.

## 📂 Project Structure

```text
House-Price-Prediction/
│
├── house-price-prediction.ipynb   # Data analysis and model development
├── HousePricePrediction.csv       # Housing dataset
└── README.md                       # Project documentation
```

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd House-Price-Prediction
```

### 2. Install Required Libraries

Make sure Python is installed, then run:

```bash
pip install pandas numpy seaborn scikit-learn jupyter
```

### 3. Launch Jupyter Notebook

```bash
jupyter notebook
```

### 4. Run the Project

1. Open `house-price-prediction.ipynb`.
2. Ensure `HousePricePrediction.csv` is in the same directory.
3. Run the notebook cells sequentially to explore the data, train the model, and evaluate its performance.

## 🔮 Future Improvements

- Experiment with Random Forest and Gradient Boosting regression.
- Apply hyperparameter tuning and cross-validation.
- Explore additional features and feature engineering techniques.
- Compare multiple machine learning algorithms.
- Improve prediction accuracy through better preprocessing.
- Investigate feature importance and model interpretability.

## ⚠️ Limitations

- The current implementation uses Linear Regression as a baseline model.
- Predictions are based on 11 selected features.
- Linear Regression may not capture complex relationships in housing data.
- Model predictions are estimates, not guaranteed market valuations.

## 👨‍💻 Author

**Malik Qousain Raza**

Computer Science Undergraduate | Interested in Data Analytics, Machine Learning, and AI.

- GitHub: [QousainRaza](https://github.com/QousainRaza)
- LinkedIn: [Malik Qousian Raza](https://www.linkedin.com/in/malikqousainraza/)

---

⭐ If you find this project useful, consider giving the repository a star!
