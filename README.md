# Decision Tree Classifier for Salary Prediction

This project demonstrates a simple implementation of a Decision Tree Classifier to predict whether an employee's salary is more than 100k based on the company they work for, their job role, and their degree.

## Dataset

The dataset used in this project contains the following columns:
- `company`: The company where the employee works (e.g., Google, ABC Pharma, Facebook).
- `job`: The job role of the employee (e.g., Sales Executive, Business Manager, Computer Programmer).
- `degree`: The highest degree held by the employee (e.g., Bachelors, Masters).
- `salary_more_than_100k`: Target variable indicating if the salary is more than 100k (1 for Yes, 0 for No).

**Sample data:**

| company    | job                | degree    | salary_more_than_100k |
|------------|--------------------|-----------|-----------------------|
| Google     | Sales Executive     | Bachelors | 0                     |
| Facebook   | Business Manager    | Masters   | 1                     |
| ABC Pharma | Computer Programmer | Bachelors | 0                     |

## Model

We use the `DecisionTreeClassifier` from the `scikit-learn` library to build the model. The categorical features (`company`, `job`, and `degree`) are label encoded before fitting the model. After training, the model achieves a score of **1.0** on the training data.

## Steps in the code:
1. Data Preprocessing: Label encoding of categorical variables.
2. Model Training: Using Decision Tree Classifier to fit the data.
3. Model Evaluation: Calculating the accuracy of the model.

## Requirements

- pandas
- scikit-learn

## How to run

1. Load the dataset into a pandas DataFrame.
2. Encode the categorical variables (`company`, `job`, `degree`).
3. Train the Decision Tree Classifier using the preprocessed data.
4. Evaluate the model on the training data.

## Conclusion

This project successfully demonstrates how to use a Decision Tree Classifier for predicting employee salaries based on categorical features.
