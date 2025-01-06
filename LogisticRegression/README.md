# Titanic Logistic Regression

This project uses logistic regression to predict the survival of passengers on the Titanic based on the given dataset. The implementation includes data preprocessing, model training using gradient descent, and evaluation.

---

## Project Structure

1. **Data Preprocessing**
   - Missing values in `Age` are filled with the mean.
   - Missing values in `Embarked` are filled with the most frequent value.
   - Unnecessary columns (`Cabin`, `PassengerId`, `Name`, `Ticket`) are dropped.
   - Categorical variables (`Pclass`, `Embarked`, `Sex`) are one-hot encoded.
   - An intercept column is added to the feature matrix for logistic regression.

2. **Model Implementation**
   - Logistic regression is implemented using gradient descent.
   - The sigmoid function is used for probability estimation.
   - The gradient descent algorithm optimizes weights over multiple iterations.

3. **Evaluation**
   - The model's accuracy is calculated on the training set.
   - Predictions are made on the test set, and results are saved in a CSV file for submission.

---

## Requirements

The following Python libraries are required:
- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`


pip install numpy pandas matplotlib seaborn
