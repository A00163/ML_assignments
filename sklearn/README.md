# Logistic Regression with Imbalanced Data

This project demonstrates the use of logistic regression to handle imbalanced datasets using various techniques. The dataset is split into training and testing sets, and different methods are applied to address class imbalance.

---

## Project Structure

1. **Logistic Regression without Handling Imbalance**
   - A baseline model is trained without addressing class imbalance.
   - Results are evaluated on both training and testing sets.

2. **Logistic Regression with Oversampling**
   - Random oversampling is applied to balance the classes in the training dataset.
   - The model is trained on the oversampled data and evaluated on both training and testing sets.

3. **Logistic Regression with Undersampling**
   - Random undersampling is used to balance the classes in the training dataset.
   - The model is trained on the undersampled data and evaluated on both training and testing sets.

4. **Logistic Regression with Weighted Loss Function**
   - Class weights are calculated and incorporated into the logistic regression model to penalize the minority class less heavily.
   - The model is trained on the original dataset with weighted loss and evaluated on both training and testing sets.

---

## Requirements

The following Python libraries are required to run the code:

- `pandas`
- `scikit-learn`
- `imbalanced-learn`

pip install pandas scikit-learn imbalanced-learn
