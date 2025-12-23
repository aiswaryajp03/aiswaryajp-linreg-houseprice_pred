# aiswaryajp-linreg-houseprice_pred
# House Price Prediction

This project implements a **Linear Regression** model to estimate residential property values based on key physical attributes and historical data.

## 📊 Dataset Specifications
The analysis is based on the `Real_estate.csv` dataset, which contains **500 entries** with the following features:

| Feature | Description |
| :--- | :--- |
| **Garage_Size** | Capacity or area of the attached garage. |
| **Num_Bathrooms** | Total number of bathrooms in the property. |
| **Num_Bedrooms** | Total number of bedrooms. |
| **Square_Feet** | Total interior living space (Sq. Ft.). |
| **Year_Built** | The year the property was originally constructed. |
| **Price** (Target) | The actual market value or selling price. |

## 💡 Key Insights
Correlation analysis of the features reveals:
* **Primary Drivers**: **Number of Bedrooms** (correlation: 0.56) and **Square Footage** (correlation: 0.55) are the strongest indicators of price.
* **Recency Trend**: There is a significant positive correlation (0.42) with the **Year Built**, indicating that newer homes generally command higher prices.
* **Stability**: The garage size and bathroom count have a positive, though less dominant, influence compared to total living space.

## 🔢 Linear Regression
The model represents the relationship between features and price using the general linear form:

$$Y = \beta_0 + \beta_1X_1 + \beta_2X_2 + ... + \beta_nX_n + \epsilon$$

## 🚀 Model Performance
The model shows high predictive accuracy on the test dataset:

* **R-Squared ($R^2$):** $0.9117$ (The model explains ~91% of the price variance).
* **Mean Absolute Error (MAE):** $\$27,589.29$
* **Root Mean Squared Error (RMSE):** $\$35,516.07$

## 📈 Evaluation Results
The project provides several assets to validate the model's reliability:

1.  **Actual vs. Predicted Plot**: The `Actual vs Predicted.png` chart shows a tight linear distribution, indicating that predictions closely follow actual market values.
2.  **Predictions Log**: The `predictions.csv` file provides a direct comparison between the actual prices and the model's estimates for the test set.
3.  **Implementation**: The full workflow from data cleaning to model training is documented in `houseprice_.ipynb`.

---
