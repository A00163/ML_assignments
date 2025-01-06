# XGBoost Heart Disease Classifier

## **Overview**
This project implements a machine learning model using the **XGBoost Classifier** to predict the presence of heart disease. The model is trained and evaluated on the **Heart Disease dataset** from OpenML, with hyperparameter tuning to optimize performance.

---

## **Features**
- Binary classification to detect heart disease.
- Utilizes the **XGBoost** algorithm, known for its speed and accuracy.
- Includes hyperparameter tuning for:
  - Learning rate
  - Maximum tree depth
  - Number of estimators
- Performance evaluation using training and testing accuracy.

---

## **Dataset**
- **Source**: [Heart Disease Dataset on OpenML](https://www.openml.org/d/53)
- **Description**: The dataset contains 13 features related to patient health (e.g., age, cholesterol levels, etc.) and a binary target variable indicating the presence or absence of heart disease.

---

## **Requirements**
To run the project, you need the following Python libraries installed:
- **Pandas**
- **Scikit-learn**
- **XGBoost**

Install the required libraries using:
```bash
pip install pandas scikit-learn xgboost
```

---

## **How to Run**
1. Clone or download the repository.
2. Ensure all dependencies are installed.
3. Run the script:
   ```bash
   python xgboost_heart_classifier.py
   ```
4. The script will:
   - Load the dataset.
   - Train the XGBoost model with various hyperparameters.
   - Evaluate the model's performance.
   - Display the results in a tabular format.

---

## **Results**
The script outputs a table summarizing the performance of the model for different hyperparameter combinations. Key metrics include:
- Training accuracy
- Testing accuracy




این متن یک فایل **README.md** استاندارد است که می‌توانید آن را ذخیره کنید و در پروژه خود استفاده کنید.