
# 🏠 House Price Prediction using Linear Regression

This project demonstrates the use of **Linear Regression** to predict house prices based on features such as area, number of bedrooms, and bathrooms.

## 📊 Features

* Uses a **linear regression model** to predict house prices.
* Reads input data from a CSV file (`house_prices.csv`).
* Splits data into training and testing sets.
* Evaluates model performance using **Root Mean Squared Error (RMSE)**.

## 📁 Dataset

The dataset (`house_prices.csv`) should contain the following columns:

| area | bedrooms | bathrooms | price  |
| ---- | -------- | --------- | ------ |
| 2100 | 3        | 2         | 500000 |
| ...  | ...      | ...       | ...    |

* `area`: Size of the house in square feet
* `bedrooms`: Number of bedrooms
* `bathrooms`: Number of bathrooms
* `price`: Target variable – house price in currency units

## 🧠 Code Explanation

1. Load dataset using `pandas`.
2. Define input features (`area`, `bedrooms`, `bathrooms`) and target (`price`).
3. Split the dataset: 80% for training and 20% for testing.
4. Train a **Linear Regression** model using `scikit-learn`.
5. Predict house prices on the test set.
6. Calculate **RMSE** to evaluate model performance.

## 🛠️ How to Run

1. Ensure the following packages are installed:

   ```bash
   pip install numpy pandas scikit-learn
   ```

2. Place your CSV file as `house_prices.csv` in the project directory.

3. Run the script:

   ```bash
   python house_price_prediction.py
   ```

4. The script will print the dataset and the **Root Mean Squared Error (RMSE)** on the test set.

## 📈 Example Output

```
           area  bedrooms  bathrooms   price
0           2100         3          2  500000
1           1600         2          1  330000
...
RMSE: 24567.12
