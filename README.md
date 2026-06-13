# Fuel Consumption & CO₂ Emissions Prediction

A simple Machine Learning project that uses **Linear Regression** to predict vehicle **CO₂ emissions** based on engine size using the **Fuel Consumption Dataset**.

## 📌 Project Overview

This project demonstrates the basic workflow of a Machine Learning regression problem:

1. Load and explore a dataset.
2. Visualize relationships between features.
3. Split data into training and testing sets.
4. Train a Linear Regression model.
5. Evaluate model performance using common metrics.

The goal is to predict a vehicle's **CO₂ emissions** from its **engine size**.

---

## 📊 Dataset Features

The project uses the following features from the dataset:

| Feature              | Description                     |
| -------------------- | ------------------------------- |
| ENGINESIZE           | Engine size in liters           |
| CYLINDERS            | Number of cylinders             |
| FUELCONSUMPTION_COMB | Combined fuel consumption       |
| CO2EMISSIONS         | CO₂ emissions (target variable) |

---

## 🛠 Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Scikit-learn

---

## 📂 Project Structure

```text
project/
│
├── FuelConsumption.csv
├── fuel_consumption_prediction.ipynb
├── README.md
└── requirements.txt
```

---

## 📈 Data Exploration

The project performs:

* Dataset inspection using `head()` and `describe()`
* Histograms for feature distribution
* Scatter plots to visualize relationships between:

  * Fuel Consumption and CO₂ Emissions
  * Engine Size and CO₂ Emissions
  * Cylinders and CO₂ Emissions

Example visualization:

```python
plt.scatter(cdf.ENGINESIZE, cdf.CO2EMISSIONS)
plt.xlabel("Engine Size")
plt.ylabel("CO2 Emissions")
plt.show()
```

---

## 🤖 Model Training

The dataset is randomly split into:

* 80% Training Data
* 20% Testing Data

A Linear Regression model is trained using:

```python
from sklearn import linear_model

regr = linear_model.LinearRegression()

regr.fit(train_x, train_y)
```

---

## 📉 Evaluation Metrics

The model is evaluated using:

### Mean Absolute Error (MAE)

Measures the average prediction error.

### Mean Squared Error (MSE)

Measures the average squared difference between predicted and actual values.

### R² Score

Indicates how well the model explains the variance in the target variable.

```python
print("Mean absolute error:", MAE)
print("Residual sum of squares (MSE):", MSE)
print("R2-score:", R2)
```

---

## 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/fuel-consumption-prediction.git
cd fuel-consumption-prediction
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## requirements.txt

```text
numpy
pandas
matplotlib
scikit-learn
```

---

## ▶️ Running the Project

Open the Jupyter Notebook:

```bash
jupyter notebook
```

Run all cells in:

```text
fuel_consumption_prediction.ipynb
```

---

## 📌 Results

The model learns the relationship between engine size and CO₂ emissions and provides predictions for unseen vehicles. The fitted regression line can be visualized directly on the training data to understand the model's performance.

---

## 📚 Learning Objectives

This project is useful for learning:

* Data preprocessing
* Exploratory Data Analysis (EDA)
* Data visualization
* Train/Test splitting
* Linear Regression
* Model evaluation with Scikit-learn

---

## 👨‍💻 Author

**Hooman Eskandari**

Computer Science Student | Machine Learning Enthusiast

GitHub: *Add your GitHub profile link here*
