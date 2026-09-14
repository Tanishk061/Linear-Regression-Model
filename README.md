# Linear-Regression-Model
Train a Linear Regression model on any dataset and report RMSE. Share GitHub or Colab link.

## About the Project

This project was completed as part of my internship task on Machine Learning.

For this task, I used the student performance dataset from my previous Exploratory Data Analysis task. I trained a Linear Regression model to predict a student's Writing Score using their Math Score and Reading Score.

The main objective was to understand the basic workflow of a regression problem, including preparing the data, splitting it into training and testing sets, training the model and evaluating its performance using RMSE.

## Dataset

The dataset contains information about student performance, including:

* Student ID
* Gender
* Race/Ethnicity
* Parental Education
* Lunch
* Test Preparation Course
* Math Score
* Reading Score
* Writing Score

The dataset contains 100 student records.

## Model Approach

### Features

The following two columns were used as input features:

* Math Score
* Reading Score

### Target

The model was trained to predict:

* Writing Score

### Train-Test Split

The dataset was divided into:

* 80% training data
* 20% testing data

A fixed random state of 42 was used so that the result can be reproduced.

## Linear Regression

I used the `LinearRegression` model from Scikit-learn.

The model learns the relationship between the input scores and the Writing Score and then uses this relationship to make predictions on the test data.

## Model Evaluation

The model was evaluated using Root Mean Squared Error (RMSE).

### Result

**RMSE: 16.10**

The RMSE represents the typical prediction error of the model in terms of Writing Score units. A lower RMSE generally indicates better prediction performance.

The model also produced an R² score of approximately **-0.27** on the test data.

## Technologies Used

* Python
* Pandas
* Scikit-learn
* CSV Dataset

## How to Run

Install the required libraries:

```bash
pip install pandas scikit-learn
```

Make sure the following files are in the same folder:

```text
student_Dataset.csv
linear_regression.py
```

Run the Python script:

```bash
python linear_regression_model.py
```

The program will train the model and display the RMSE, R² score, model coefficients and actual versus predicted values.

## Learning Outcome

Through this task, I learned the basic workflow of supervised machine learning for regression.

I learned how to select features and a target variable, split a dataset into training and testing data, train a Linear Regression model and evaluate its predictions using RMSE.

This task helped me understand how machine learning can be used to estimate a numerical outcome from existing data.
