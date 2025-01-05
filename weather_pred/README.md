# Weather Prediction

This repository implements a linear regression model to predict the **Apparent Temperature (C)** using historical weather data. The project includes data preprocessing, exploratory data analysis, and model training using Scikit-Learn.

---

## Table of Contents

- [Introduction](#introduction)
- [Data Description](#data-description)
- [Techniques Used](#techniques-used)
- [Model Training](#model-training)
- [Evaluation Metrics](#evaluation-metrics)
- [How to Run](#how-to-run)
- [Requirements](#requirements)

---

## Introduction

This project implements a simple linear regression model to predict the **Apparent Temperature (C)** based on historical weather data. The code includes data cleaning, feature analysis, and training the model using Scikit-Learn's `LinearRegression` class.

---

## Data Description

The dataset contains historical weather data with the following features:

- **Temperature (C)**: Actual temperature at the time of recording.
- **Humidity**: Relative humidity as a percentage.
- **Wind Speed (km/h)**: Speed of the wind at the time of recording.
- **Visibility (km)**: Average visibility in kilometers.
- **Pressure (millibars)**: Atmospheric pressure.
- **Precip Type**: Type of precipitation (e.g., rain or snow).
- **Apparent Temperature (C)**: The target variable representing the "feels-like" temperature.

---

## Techniques Used

- **Data Preprocessing**:
  - Handling missing values (e.g., filling missing `Precip Type` values with the most frequent category).
  - Dropping non-numeric columns for simplicity.
- **Exploratory Data Analysis**:
  - Heatmaps to visualize feature correlations.
  - Pairplots to explore relationships between features.
- **Linear Regression**:
  - Model training using Scikit-Learn's `LinearRegression` class.
  - Predictions on unseen test data.

---

## Model Training

The model is trained using the following steps:
1. **Data Cleaning**: Missing values in the `Precip Type` column are filled with the most frequent value (`rain`). Non-numeric columns are removed.
2. **Feature and Target Splitting**:
   - Features (`X`) include all columns except the target.
   - The target variable (`y`) is the **Apparent Temperature (C)**.
3. **Model Training**: The linear regression model is trained on the cleaned training dataset.
4. **Prediction**: The trained model is used to predict the target variable for the test dataset.

---

## Evaluation Metrics

The following metrics can be used to evaluate the model's performance (not implemented in the current version):

- **Mean Absolute Error (MAE)**
- **Mean Squared Error (MSE)**
- **Root Mean Squared Error (RMSE)**

---

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/weather-prediction.git
   cd weather-prediction
   ```

2. Ensure the required datasets (`weatherHistory_Train.csv` and `weatherHistory_Test.csv`) are in the same directory as the script.

3. Run the script:
   ```bash
   python weather_pred.py
   ```

4. The predictions will be saved in a file named `weather_pred.csv`.

---

## Requirements

The following Python libraries are required to run the code:

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`

Install the dependencies using:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

---

## Outputs

- **Heatmap**: Displays the correlation between features.
- **Pairplot**: Visualizes relationships between features and the target variable.
- **`weather_pred.csv`**: Contains the predicted values for the test dataset.

---

## Future Improvements

- Add evaluation metrics to measure model performance.
- Explore advanced regression techniques (e.g., Ridge, Lasso).
- Include feature scaling to improve model accuracy.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## Author

Developed by [Your Name].  
For any questions or suggestions, feel free to contact me at [your-email@example.com].