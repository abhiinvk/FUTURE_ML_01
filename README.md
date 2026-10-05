# Sales Forecasting Using Machine Learning

## Future Interns — Machine Learning Internship

### Task 1: Sales and Demand Forecasting

This project develops a machine learning-based sales forecasting
system using historical sales data.

The objective is to analyze historical sales patterns, create
time-based features, train regression models, evaluate their
performance, and forecast future monthly sales.

---

## Project Objective

The main objectives of this project are:

- Analyze historical sales data.
- Identify sales trends and seasonal patterns.
- Create time-based and historical sales features.
- Train machine learning regression models.
- Compare model performance.
- Forecast future sales.
- Generate business insights from the predictions.

---

## Dataset

The project uses the Superstore sales dataset containing historical
transaction-level sales information.

Important columns used include:

- `Order Date` — Date of the customer order.
- `Sales` — Sales amount.

The transaction-level data was aggregated into monthly sales for
forecasting.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook
- VS Code

---

## Project Workflow

### 1. Data Loading

The historical Superstore dataset was loaded using Pandas.

### 2. Data Cleaning

- Converted `Order Date` into datetime format.
- Sorted records chronologically.
- Checked for missing values.
- Checked for duplicate records.

### 3. Monthly Sales Aggregation

Transaction-level sales were aggregated into monthly sales totals.

### 4. Exploratory Data Analysis

The following patterns were analyzed:

- Monthly sales trends
- Monthly seasonality
- Historical sales variations

### 5. Feature Engineering

The following features were created:

- Year
- Month
- Quarter
- Trend
- Lag 1
- Lag 2
- Lag 3
- Three-month rolling average

### 6. Model Training

Two machine learning regression models were evaluated:

- Random Forest Regressor
- Gradient Boosting Regressor

### 7. Model Evaluation

Models were evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

---

## Model Performance

| Model | MAE | RMSE | R² |
|---|---:|---:|---:|
| Random Forest | 14129.55 | 18033.05 | 0.4779 |
| **Gradient Boosting** | **13971.19** | **16489.98** | **0.5635** |

Gradient Boosting was selected as the final model because it achieved
lower MAE and RMSE and a higher R² score than Random Forest.

---

## Feature Importance

The most important features for the final Gradient Boosting model were:

1. Month
2. Trend
3. Lag 2
4. Lag 1
5. Lag 3
6. Rolling Mean 3
7. Quarter
8. Year

The `Month` feature had the highest model importance, indicating that
monthly patterns played a major role in the model's predictions.

---

## Future Sales Forecast

The final Gradient Boosting model was used to generate a six-month
future sales forecast.

The forecast can be used to support:

- Inventory planning
- Purchasing decisions
- Demand planning
- Resource allocation
- Staffing decisions
- Financial planning

---

## Business Insights

The forecasting system demonstrates how historical sales data can be
used to support data-driven business decisions.

The model identifies monthly patterns and uses previous sales values
to estimate future demand.

Businesses can use these forecasts to prepare inventory for periods
of expected higher demand and reduce the risk of overstocking during
lower-demand periods.

---

## Project Structure

```text
Sales-Forecasting/
│
├── Sample - Superstore.csv
├── sales_forecasting.ipynb
└── README.md