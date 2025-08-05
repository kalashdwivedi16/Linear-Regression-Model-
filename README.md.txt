# Sales Forecasting using Linear Regression

This project demonstrates a simple yet effective approach to forecast monthly sales revenue using Linear Regression. It uses synthetic data with various influencing factors to model and predict revenue trends.

## Project Structure

- **Input Variables**:
  - `Marketing_Spend`: Monthly marketing budget.
  - `Promotion_Flag`: Binary flag indicating promotional activity.
  - `Season`: Categorical variable for seasonal impact.
  - `Product_Category`: Product types A, B, or C.
  - `Channel`: Sales channel – Online, Retail, or Distributor.

- **Target Variable**:
  - `Revenue`: Simulated sales revenue generated from a combination of above factors with added noise.

## Methodology

1. **Data Generation**:
   - 12 months of synthetic data generated using `numpy` and `pandas`.
   - Revenue is calculated using a linear formula with added Gaussian noise.

2. **Preprocessing**:
   - Dropped `Month` column.
   - Categorical features encoded using `pd.get_dummies()` (one-hot encoding).

3. **Modeling**:
   - Linear Regression model from `sklearn.linear_model`.
   - Fitted on encoded features and revenue.

4. **Evaluation**:
   - Predicted on training data.
   - Metrics such as RMSE and R² Score (not shown but implied in imports).

5. **Visualization**:
   - (If included): Use of `matplotlib` and `seaborn` for potential visualizations.

## Requirements

```bash
pip install pandas numpy matplotlib seaborn scikit-learn