# 📱 Mobile Price Prediction using Linear Regression

## 📌 Project Overview

### Project Title
**Mobile Price Prediction using Linear Regression**

### Objective

The objective of this project is to analyze a mobile phone dataset and build a **Linear Regression model** to predict mobile phone prices based on important hardware specifications.

The analysis focuses on identifying the features that have the strongest relationship with mobile prices and using those features to train a machine learning model.

The assignment specifically requires dataset exploration, correlation analysis, feature selection, an 80/20 train-test split, Linear Regression, and evaluation using R², MAE, and MSE.

## 📂 Dataset

**Dataset:** Mobile Price Dataset

The dataset contains mobile phone specifications and their corresponding **Price**.

Important features analyzed in this project include:

- RAM
- Internal Memory
- PPI
- Rear Camera
- Price

The dataset is loaded into a Pandas DataFrame and explored before model building.

## 🛠️ Technologies & Libraries Used

### Programming Language
- Python

### Libraries

- **Pandas** – Data loading and data analysis
- **NumPy** – Numerical operations
- **Matplotlib** – Data visualization
- **Seaborn** – Correlation heatmap and scatter plots
- **Scikit-learn** – Machine Learning and model evaluation


## 🔍 Project Workflow

The project follows the standard Machine Learning workflow:

Dataset
   ↓
Data Exploration
   ↓
Data Cleaning / Missing Value Check
   ↓
Correlation Analysis
   ↓
Feature Selection
   ↓
Train-Test Split
   ↓
Linear Regression Model
   ↓
Model Training
   ↓
Price Prediction
   ↓
Model Evaluation
   ↓
Insights & Conclusion

## 1️⃣ Data Exploration

The dataset is explored to understand its structure and quality.

The following analyses are performed:

- Dataset shape
- Column names
- Data types
- Missing values
- Statistical summary
- Numerical feature relationships

The assignment requires inspection of the dataset structure, feature distributions, missing values, and statistical summaries before model building.

## 2️⃣ Correlation Analysis

A **correlation matrix** is created to identify the relationship between numerical variables.

A correlation heatmap is generated to visually understand the strength and direction of relationships between the features and **Price**.

### Top Correlated Features

Based on the analysis in the notebook, the major features associated with Price are:

1. **RAM**
2. **PPI**
3. **Internal Memory**
4. **Rear Camera**

The notebook identifies strong positive relationships between these features and mobile price.


## 3️⃣ Data Preparation

### Feature Selection

The selected features are used as independent variables:

RAM
PPI
Internal Memory
Rear Camera

The target variable is:
Price

Therefore:
X = selected features
y = Price


## 4️⃣ Train-Test Split

The dataset is divided into:

- **80% Training Data**
- **20% Testing Data**

A `random_state` of `42` is used to make the split reproducible.

This follows the assignment requirement of using 80% of the data for training and 20% for testing.

## 5️⃣ Linear Regression Model

A Linear Regression model is created using Scikit-learn.

from sklearn.linear_model import LinearRegression

model = LinearRegression()
model.fit(X_train, y_train)

The model learns the relationship between the selected mobile specifications and their prices.

## 6️⃣ Price Prediction

After training, the model predicts prices for the testing dataset.
y_pred = model.predict(X_test)

The predicted values are then compared with the actual mobile prices.

## 7️⃣ Model Evaluation

The trained model is evaluated using the following metrics:

### R² Score

R² measures how well the model explains the variation in mobile prices.
Higher R² → better explanation of variance

### Mean Absolute Error (MAE)

MAE represents the average absolute difference between the actual and predicted prices.
MAE = Average |Actual Price - Predicted Price|

Lower MAE indicates smaller prediction errors.

### Mean Squared Error (MSE)

MSE calculates the average squared difference between actual and predicted prices.
MSE = Average (Actual Price - Predicted Price)²

Lower MSE indicates lower prediction error.

### Coefficients and Intercept

The model coefficients and intercept are also calculated to understand the mathematical relationship learned by the model.

The assignment specifically requires the slope/coefficient, intercept, R², MAE, and MSE to be reported.


## 📊 Visualizations

The project includes the following visualizations:

### Correlation Heatmap

Used to identify relationships between numerical features and Price.

### Scatter Plots

Scatter plots are created for the top correlated features against Price.

### Regression Plots

Regression plots are used to visualize the direction of the relationship between selected features and Price.

The assignment requires a correlation heatmap and scatter plots for the top correlated features.

## 💡 Key Insights

The analysis indicates that mobile hardware specifications have meaningful relationships with mobile prices.

### Main observations

- **RAM** shows a strong positive relationship with Price.
- **Internal Memory** is positively associated with Price.
- **PPI** shows a positive relationship with Price.
- **Rear Camera** also shows a positive relationship with Price.
- The selected features can therefore be used as predictors in the Linear Regression model.

The scatter and regression plots provide a visual representation of these relationships.

## 📈 Skills Demonstrated

Through this project, I practiced:

- Python Programming
- Pandas
- Data Exploration
- Data Cleaning
- Descriptive Statistics
- Correlation Analysis
- Data Visualization
- Feature Selection
- Train-Test Split
- Machine Learning
- Linear Regression
- Model Prediction
- R² Score
- MAE
- MSE
- Model Interpretation
- Data Science Reporting

These align with the assignment's evaluated skills in data exploration, visualization, data preparation, machine learning, evaluation, and reporting.

## 📁 Project Structure

Assignment_6_Linear_Regression/
│
├── Linear_Regression.ipynb
├── mobile_price.csv
├── README.md
└── requirements.txt

## ▶️ How to Run the Project

### 1. Clone the repository
git clone <your-repository-link>

### 2. Open the project

Open the project folder in **VS Code** or **Jupyter Notebook**.

### 3. Install required libraries
pip install pandas numpy matplotlib seaborn scikit-learn

### 4. Run the notebook

Open:
Linear_Regression.ipynb

Run the cells sequentially.

## 🎯 Conclusion

This project demonstrates an end-to-end **Linear Regression workflow** for mobile price prediction.

The analysis begins with dataset exploration and correlation analysis, followed by feature selection and an 80/20 train-test split. A Linear Regression model is then trained and evaluated using **R² Score, MAE, and MSE**.

The results help demonstrate how mobile hardware specifications can be used as predictors of mobile phone prices.

Further improvements could include experimenting with additional relevant features, preprocessing techniques, alternative regression algorithms, and systematic model tuning. The assignment also asks for discussion of potential improvements based on model performance.

