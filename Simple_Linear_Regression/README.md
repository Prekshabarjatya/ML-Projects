# Simple Linear Regression

This repository contains a Simple Linear Regression model that predicts salaries based on years of experience. The model is implemented using Python and the **scikit-learn** library.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Model Training](#model-training)
- [Results](#results)
- [Future Improvements](#future-improvements)
- [Contributing](#contributing)

## Project Overview
This project demonstrates how to apply **Simple Linear Regression** to predict salaries based on experience. The model is trained on a dataset containing salary information and visualized using Matplotlib.

## Dataset
The dataset used in this project is **Salary_Data.csv**, which contains two columns:
- **Years of Experience** (Independent Variable: X)
- **Salary** (Dependent Variable: y)

The dataset is split into training and testing sets using an 80-20 split.

## Installation
To run this project, ensure you have the following dependencies installed:

```bash
pip install numpy pandas matplotlib scikit-learn
```

## Usage
Clone this repository and navigate to the project directory:

```bash
git clone https://github.com/yourusername/ml-repo.git
cd ml-repo
```

Run the script:

```bash
python simple_linear_regression.py
```

## Model Training
The model is trained using **LinearRegression** from `sklearn.linear_model`:
```python
from sklearn.linear_model import LinearRegression
regressor = LinearRegression()
regressor.fit(X_train, y_train)
```

Once trained, the model predicts salaries for test data and visualizes results using Matplotlib.

## Results
The model generates predictions for the test set and plots the results:
- **Training Set Visualization:** Scatter plot with the regression line.
- **Test Set Visualization:** Scatter plot with predictions.

### Sample Prediction:
Predict salary for 23 years of experience:
```python
print(regressor.predict([[23]]))
```

### Model Parameters:
```python
print(regressor.coef_)   # Slope (theta1)
print(regressor.intercept_)  # Intercept (theta0)
```

## Future Improvements
- Add more features for better prediction (e.g., education level, industry, location).
- Use **Polynomial Regression** for non-linear patterns.
- Optimize hyperparameters using **GridSearchCV**.
- Deploy the model using **Flask/Django API**.

## Contributing
Feel free to fork this repository, improve the model, and submit a pull request. Suggestions and contributions are welcome!

### Author
**Your Name**  
GitHub: [YourUsername](https://github.com/YourUsername)

