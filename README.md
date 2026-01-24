# Sales Forecasting and Business Insights

This project combines Python forecasting models with an interactive Power BI dashboard to analyze historical sales data, predict future trends, and uncover actionable business insights. It demonstrates end-to-end analytics capability: from data cleaning and modeling to dashboard storytelling.

## Project Structure

- `data/` — Cleaned monthly sales data
- `notebooks/` — Python forecasting models and visualizations
- `powerbi/` — Power BI dashboard file
- `images/` — Forecast charts and dashboard screenshots
- `README.md` — Project overview and insights

## Forecasting Models (Python)

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

This segmentation supports inventory planning, marketing strategy, and product prioritization.

## Visualizations

- Forecast comparison chart (actual vs predicted)  
- Product-wise forecast chart (multiple products in one plot)  
- Error metric comparison table  
- Power BI dashboard visuals  


## Power BI Dashboard

The Power BI dashboard provides interactive analysis of historical sales performance across four key areas: 

### **1. Executive Overview** 
- Total sales, orders, and average order value
- Sales by region and product
- Monthly sales trends
- Filters: Region, Product, Year

### **2. Customer Insights** 
- Retail vs Wholesale comparison
- Top 10 customers by revenue
- Orders by region and customer type -
- Discount impact on sales
- Promotion usage analysis
- Filters: CustomerType, Region, Year

### **3. Salesperson & Store Performance** 
- Sales by store location
- Discounts given by salesperson
- Sales by region manager - Orders and revenue by salesperson
- Highlights: Top salesperson, top store
- Filters: Salesperson, StoreLocation, Region, Year

### **4. Delivery & Returns Analysis** 
- Late deliveries by store
- Returns by product and region
- Delivery time distribution
- Return rate and total returns
- Filters: Product, Region, StoreLocation, Year
  
This dashboard allows stakeholders to explore insights interactively and supports data-driven decision-making.  
### 🔗 Dashboard Purpose 
Power BI enables stakeholders to explore historical performance interactively. Python forecasting adds predictive power for future planning.

Together, they deliver a complete analytics solution: 

**Power BI for exploration → Python for forecasting → Insights for action**

## Tools & Libraries

- Python  
- Pandas  
- Matplotlib  
- Statsmodels  
- scikit-learn  
- Power BI

## Insights

Overall sales show a steady upward trend, and forecasts indicate continued moderate growth.

Holt‑Winters produced the most stable forecast pattern and the lowest RMSE, making it the preferred model for future planning.

Product‑wise forecasting highlights Tablets and Phones as growth categories, while Desks show a declining trend.

Chairs, Laptops, and Monitors remain stable, providing consistent revenue with low volatility.

Wholesale customers contribute higher revenue, while retail customers generate more frequent orders.

Certain regions show higher late deliveries and return rates, suggesting opportunities to improve logistics and product quality.


## Business Impact

This project demonstrates:

- Multi-model forecasting and evaluation 
- Segmented forecasting by product  
- Model selection based on RMSE  
- Integration of Python and Power BI 
- Business storytelling through dashboards and visuals  

It showcases advanced analytics skills for data analyst and business intelligence roles.

## 📬 Contact

**Jannathul Firdouz**  
Master of Analytics

🔗 LinkedIn: https://www.linkedin.com/in/jannathul-firdouz-58298b321  
💻 GitHub: https://github.com/jannathulfirdouz

