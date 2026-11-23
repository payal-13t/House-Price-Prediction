# 🏠 House Price Prediction | Machine Learning & Regression

A machine learning project that predicts median house values using supervised regression algorithms. This project explores housing data through exploratory data analysis, feature engineering, preprocessing, model comparison, hyperparameter tuning and ensemble learning to identify an effective predictive model.

The project implements multiple regression techniques using Python and Scikit-learn, evaluates their performance using R² and RMSE, and explores ensemble methods to improve prediction performance.

---

## 📌 Project Overview

The objective of this project is to develop a regression-based machine learning solution that estimates house values based on geographical, demographic and housing-related attributes.

Using the California Housing dataset, the project follows a structured machine learning workflow:

- Data loading and exploratory data analysis
- Missing-value detection and treatment
- Statistical analysis and data visualisation
- Feature scaling and selection
- Regression model development
- Hyperparameter optimisation
- Ensemble learning
- Model evaluation and comparison
- Model serialisation

## 🎯 Key Objectives

- Understand the factors influencing median house values.
- Perform exploratory data analysis to identify patterns and relationships.
- Prepare numerical and categorical features for machine learning.
- Compare multiple regression algorithms.
- Improve model performance through hyperparameter tuning.
- Evaluate ensemble techniques, including Voting and Stacking Regressors.

## 📊 Dataset Description

The project uses the California Housing dataset.

**Dataset Statistics:**

| Attribute | Details |
|---|---|
| Total Records | 20,640 |
| Total Features | 9 input features |
| Target Variable | median_house_value |
| Problem Type | Supervised Learning |
| ML Task | Regression |

### Dataset Features

| Feature | Description |
|---|---|
| longitude | Geographic longitude |
| latitude | Geographic latitude |
| housing_median_age | Median age of houses |
| total_rooms | Total rooms in the block |
| total_bedrooms | Total bedrooms in the block |
| population | Block population |
| households | Number of households |
| median_income | Median household income |
| ocean_proximity | Proximity to the ocean |
| median_house_value | Target variable |

## ⚙️ Technologies & Libraries

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Data Manipulation | Pandas, NumPy |
| Data Visualisation | Matplotlib, Seaborn |
| Statistical Analysis | SciPy |
| Machine Learning | Scikit-learn |
| Model Persistence | Joblib |
| Development Environment | Jupyter Notebook |

## 🔍 Project Workflow

### 1. Data Loading & Understanding
- Imported the housing dataset using Pandas.
- Examined dataset dimensions, column names and data types.
- Analysed descriptive statistics.
- Identified missing values and duplicate records.

### 2. Exploratory Data Analysis (EDA)
- Analysed numerical and categorical variables.
- Examined the distribution of housing attributes.
- Explored relationships between input features and house values.
- Used statistical summaries and visualisations to understand the dataset.

### 3. Data Preprocessing & Feature Engineering
- Identified missing values in the dataset.
- Applied preprocessing techniques for numerical features.
- Used StandardScaler for feature scaling.
- Applied Recursive Feature Elimination (RFE) for feature selection.
- Selected relevant features for model development.

### 4. Model Development

Implemented and compared the following regression algorithms:

- Linear Regression
- Support Vector Regression (SVR)
- Random Forest Regressor
- Decision Tree Regressor
- K-Nearest Neighbours (KNN) Regressor

### 5. Hyperparameter Tuning

Used GridSearchCV with cross-validation to optimise model parameters.

Optimisation was performed for:
- Decision Tree Regressor
- K-Nearest Neighbours Regressor

### 6. Ensemble Learning

Implemented two ensemble techniques to evaluate whether combining multiple regression models could improve prediction performance.

**Voting Regressor**
- Combined multiple regression estimators.
- Achieved a test R² score of 78.31%.

**Stacking Regressor**
- Combined Decision Tree, Random Forest, SVR, KNN and Linear Regression as base estimators.
- Used Random Forest as the final estimator.
- Achieved a test R² score of 80.55%.

## 📈 Model Evaluation & Results

The models were evaluated using:

- **R² Score:** Measures how well the model explains the variance in house values.
- **RMSE:** Measures the magnitude of prediction errors.

### Regression Model Comparison

| Model | Train R² | Test R² |
|---|---:|---:|
| Random Forest | 90.55% | **81.00%** |
| SVR | 74.70% | 71.53% |
| Decision Tree | 100.00% | 68.80% |
| KNN Regressor | 81.01% | 67.85% |
| Linear Regression | 64.13% | 61.55% |

### Ensemble Model Results

| Model | Test R² |
|---|---:|
| Voting Regressor | 78.31% |
| Stacking Regressor | 80.55% |

**Key Finding:** Random Forest achieved the highest test R² score of approximately 81% among the individual regression models evaluated. The Stacking Regressor achieved a comparable test score of 80.55%.

These results demonstrate the importance of model comparison and evaluation rather than relying on a single algorithm.

## 📁 Repository Structure

```text
House-Price-Prediction/
│
├── House Price Prediction.ipynb
│   # Data analysis, preprocessing,
│   # model training and evaluation
│
├── house price.csv
│   # California Housing dataset
│
└── README.md
    # Project documentation
```

## 🚀 Installation & Execution

### Prerequisites

- Python 3.10 or later
- Jupyter Notebook
- pip

### Step 1: Clone the Repository

```bash
git clone https://github.com/payal-13t/House-Price-Prediction.git
```

### Step 2: Navigate to the Project Directory

```bash
cd House-Price-Prediction
```

### Step 3: Create a Virtual Environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### Step 4: Install Dependencies

```bash
pip install numpy pandas matplotlib seaborn scipy scikit-learn joblib jupyter
```

### Step 5: Launch Jupyter Notebook

```bash
jupyter notebook
```

### Step 6: Execute the Project

1. Open `House Price Prediction.ipynb`.
2. Ensure `house price.csv` is in the same directory.
3. Execute the notebook cells sequentially.
4. Review the EDA, preprocessing, model training and evaluation results.

The notebook also contains code for saving the trained Stacking Regressor using Joblib.

## 💡 Key Learnings

Through this project, I gained practical experience in:

- Applying the complete machine learning workflow to a regression problem.
- Performing exploratory data analysis on structured datasets.
- Handling missing values and preparing data for model training.
- Implementing feature scaling and feature selection.
- Comparing traditional regression algorithms with ensemble methods.
- Applying GridSearchCV for hyperparameter optimisation.
- Evaluating models using R² and RMSE.
- Saving trained machine learning models using Joblib.

## 🔮 Future Improvements

- Develop an interactive web application using Flask or Streamlit.
- Build a reusable end-to-end Scikit-learn preprocessing and prediction pipeline.
- Add automated model training and evaluation scripts.
- Implement cross-validation and additional error analysis.
- Deploy the prediction model using a cloud platform.
- Add automated testing and model monitoring.

## 👩‍💻 Author

**Payal Tiwari**

GitHub: [payal-13t](https://github.com/payal-13t)

---

⭐ If you find this project interesting, consider giving the repository a star!
