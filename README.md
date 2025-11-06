# 🏡 Ames Housing Price Prediction

This project predicts housing prices using the Ames Housing dataset. We compare three models — Linear Regression, Random Forest, and XGBoost — using log-transformed sale prices for better accuracy.

## 📊 Model Comparison

| Model               | MAE (log) | RMSE (log) | R² Score | MAE (original) | RMSE (original) |
|--------------------|-----------|------------|----------|----------------|-----------------|
| Linear Regression  | 0.10      | 0.19       | 0.8002   | **15738.54**   | **26773.62**    |
| Random Forest      | 0.10      | 0.15       | 0.8845   | 17774.03       | 29330.31        |
| XGBoost            | **0.09**  | **0.14**   | **0.8879** | 16763.05       | 27004.48        |

## 🧠 Insights

- XGBoost is the best overall model based on log-transformed metrics.
- Linear Regression shows lower MAE/RMSE on the original scale due to conservative predictions.
- Log-scale metrics are more reliable for model evaluation.

## 🛠️ How to Run

```bash
pip install -r requirements.txt
