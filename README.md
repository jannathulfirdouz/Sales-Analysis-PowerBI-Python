# Sales Forecasting and Model Comparison

This project analyzes monthly sales data and builds multiple forecasting models to predict future sales.  
It compares model performance using error metrics and selects the most accurate method.  
Forecasts are also segmented by product category to support business planning and inventory decisions.  
A Power BI dashboard is included to visualize key insights interactively.


## Project Structure

- `data/` — Cleaned monthly sales data  
- `notebooks/` — Python notebook with forecasting models and visualizations  
- `powerbi/` — Power BI dashboard file  
- `images/` — Forecast comparison charts  
- `README.md` — Project overview and insights

## Forecasting Models Used

| Model             | Approach                | Library      |
| ----------------- | ----------------------- | ------------ |
| Holt-Winters      | Trend-based time series | statsmodels  |
| SARIMA            | Seasonal ARIMA          | statsmodels  |
| Linear Regression | Baseline regression     | scikit-learn |


## Model Evaluation

Models were trained on 24 months of data and tested on the final 6 months.  
Performance was measured using MAE, RMSE, and MAPE.

| Model             | MAE    | RMSE   | MAPE   |
| ----------------- | ------ | ------ | ------ |
| Holt-Winters      | 18,809 | 20,739 | 12.46% |
| SARIMA            | 17,201 | 23,977 | 10.25% |
| Linear Regression | 17,084 | 21,957 | 10.45% |


Holt-Winters achieved the lowest RMSE and produced the most stable and realistic forecasts, making it the preferred model for this dataset.

## Product-wise Forecasting

To understand future demand by product category, Holt-Winters forecasts were built for each product.  
This segmented approach reveals which products are expected to grow, stabilize, or decline.

**Key Product Insights**

Tablet sales are projected to grow steadily

Desk sales show a declining trend

Chair, Laptop, and Monitor remain stable

Phone and Printer show moderate growth

This analysis supports inventory planning, marketing strategy, and product prioritization.


## Visualizations

- Forecast comparison chart (actual vs predicted)  
- Product-wise forecast chart (multiple products in one plot)  
- Error metric comparison table  
- Power BI dashboard visuals  


## Power BI Dashboard

A dedicated Power BI dashboard was created to complement the Python analysis.  
It includes:

- **Sales Overview Page**  
  - Total revenue  
  - Monthly trends  
  - Top-performing products  
  - Regional breakdown  

- **Product Performance Page**  
  - Product-wise sales trends  
  - Forecast overlays  
  - Contribution to total revenue  

- **Forecast Insights Page**  
  - Python-generated forecasts imported into Power BI  
  - Comparison of actual vs predicted values  
  - Product-level forecast visuals  

This dashboard allows stakeholders to explore insights interactively and supports data-driven decision-making.


## Tools & Libraries

- Python  
- Pandas  
- Matplotlib  
- Statsmodels  
- scikit-learn  
- Power BI  


## Business Impact

This project demonstrates:

- Forecasting accuracy across multiple models  
- Segmented forecasting by product  
- Model selection based on RMSE  
- Integration of Python forecasting with Power BI dashboards  
- Business storytelling through visuals and insights  

It’s designed to showcase advanced analytics skills for business intelligence roles.


## 📬 Contact

**Jannathul Firdouz**  
Aspiring Data Analyst | Forecasting & Dashboarding Enthusiast  
[LinkedIn Profile](#) | [GitHub Portfolio](#)
