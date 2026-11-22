# Restaurant Tips Prediction — Regression Analysis

An end-to-end Exploratory Data Analysis (EDA) and Supervised Machine Learning regression project aimed at predicting restaurant tip amounts based on billing and customer variables.

## Project Overview
Using historical tipping data collected over several months in a restaurant (244 records), this project explores the key factors driving tip values and builds regression models to estimate tips accurately.

### Dataset Features
Loaded via Seaborn's `tips` dataset, containing 244 observations[cite: 6] and 7 variables[cite: 6]:
* **`total_bill`**: Total cost of the meal in USD (numeric)[cite: 6]
* **`tip`**: Tip amount in USD — **Target Variable** (numeric)[cite: 6]
* **`sex`**: Gender of the bill payer (`Male` / `Female`)[cite: 6]
* **`smoker`**: Whether there were smokers in the party (`Yes` / `No`)[cite: 6]
* **`day`**: Day of the week (`Thur`, `Fri`, `Sat`, `Sun`)[cite: 6]
* **`time`**: Time of day (`Lunch` / `Dinner`)[cite: 6]
* **`size`**: Size of the dining party (numeric)[cite: 6]

---

## Workflow & Methodology

1. **Exploratory Data Analysis (EDA)**[cite: 6]
   * Inspected data types, summary statistics, and missing values using Pandas (`.info()`, `.describe()`)[cite: 6].
   * Analyzed correlations between `total_bill` and `tip` using scatter plots and regression lines[cite: 6].
   * Evaluated categorical distributions across gender, smoking status, day of the week, and meal time[cite: 6].

2. **Data Preprocessing & Feature Engineering**
   * Encoded categorical features (`sex`, `smoker`, `day`, `time`) for model compatibility[cite: 6].
   * Split the dataset into training and testing subsets to prevent data leakage.
   * Applied feature scaling where appropriate.

3. **Model Training & Evaluation**
   * Trained and compared regression algorithms using **Scikit-Learn** (e.g., Linear Regression, Polynomial Regression / Regularized models).
   * Evaluated model performance using standard regression metrics (**MAE**, **RMSE**, and **$R^2$ Score**).

---

## Key Insights
* **Strong Linear Correlation:** `total_bill` is the strongest predictor of `tip` amount, showing a clear positive linear relationship.
* **Party Size Impact:** Larger party sizes tend to generate higher total bills and consequently higher absolute tips, though tip percentage varies.
* **Time & Day Trends:** Dinner shifts and weekend days (Saturday and Sunday) account for the highest volume and value of transactions.

---

## Tech Stack
* **Language:** Python
* **Data Manipulation:** Pandas, NumPy[cite: 6]
* **Data Visualization:** Seaborn, Matplotlib[cite: 6]
* **Machine Learning:** Scikit-Learn[cite: 6]
* **Environment:** Jupyter Notebook / VS Code[cite: 6]

---

## How to Run Locally

1. Clone the repository:
   ```bash
   git clone [https://github.com/RanieriFilho/restaurant-tips-regression-ml.git](https://github.com/RanieriFilho/restaurant-tips-regression-ml.git)
   cd restaurant-tips-regression-ml
