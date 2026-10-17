# House Price Prediction Using Machine Learning

## 📌 Project Overview

This project uses machine learning regression algorithms to predict median house values using the California Housing dataset. The goal is to explore housing data, train predictive models, and evaluate their performance using regression metrics.

## 🎯 Objectives

- Explore and understand the housing dataset.
- Perform exploratory data analysis (EDA).
- Train and compare machine learning regression models.
- Evaluate predictions using MAE, RMSE, and R².
- Identify the features that contribute most to the Random Forest model's predictions.

## 📊 Dataset

- **Dataset:** California Housing
- **Source:** Scikit-learn
- **Number of records:** 20,640
- **Input features:** 8
- **Target variable:** `MedHouseVal`

The target represents median house value in units of $100,000. For example, a target value of 2.0 represents $200,000 in the dataset's units.

**Important:** The dataset is historical and describes California census block groups, not current prices for individual properties.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- Jupyter Notebook

## ⚙️ Project Workflow

1. Load the California Housing dataset.
2. Inspect the dataset and check for missing values and duplicates.
3. Perform exploratory data analysis and visualisation.
4. Separate input features and the target variable.
5. Split the data into training and testing sets.
6. Train Linear Regression and Random Forest Regression models.
7. Evaluate and compare the models.
8. Visualise actual versus predicted values.
9. Examine Random Forest feature importance.
10. Make a sample prediction and save the trained model.

## 🤖 Machine Learning Models

### 1. Linear Regression
Used as a baseline model to learn a linear relationship between input features and house values.

### 2. Random Forest Regressor
Uses multiple decision trees to learn more complex relationships in the dataset.

## 📈 Model Evaluation

The models are evaluated using:

- **Mean Absolute Error (MAE):** Average absolute prediction error.
- **Root Mean Squared Error (RMSE):** Gives greater weight to larger errors.
- **R² Score:** Measures how well the model explains variation in the target.

### Results

| Model | MAE ($) | RMSE ($) | R² Score |
| --- | --- | --- | --- |
| Linear Regression | 53,320.013 | 74,558.138 | 0.576 |
| Random Forest | 32,759.935 | 50,569.357 | 0.805 |

### Results and Interpretation

The Random Forest Regressor performed better than Linear Regression on the test dataset.

- **Linear Regression:** R² score of 0.576.
- **Random Forest:** R² score of 0.805.
- Random Forest reduced the mean absolute error by approximately **38.6%** compared with Linear Regression.

The higher R² score indicates that Random Forest explained more of the variation in the test-set house values. These results apply to the California Housing dataset and should not be treated as estimates of current individual property prices.

## 📁 Project Structure

```text
house-price-prediction/
├── house_price_prediction.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```
## 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/Rohanyadav2112-DS/house-price-prediction.git
cd house-price-prediction
```

### 2. Install dependencies

```bash
python -m pip install -r requirements.txt
```

### 3. Open the notebook

Open `house_price_prediction.ipynb` in Jupyter Notebook or VS Code and run the cells in order.

The dataset loader may download the dataset the first time it is used, so an internet connection may be required.

## ⚠️ Limitations

- The dataset is based on historical census information.
- Predictions represent district-level median values, not individual property valuations.
- The dataset target has an upper limit, which can affect evaluation.
- Predictions should not be used as current real-estate market valuations.

## 👨‍💻 Author

Rohan Yadav

MSc Data Science student | Aston University | Python | SQL | Machine Learning | Data Analytics | Data Science
