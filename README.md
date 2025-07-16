# 🛍️ AI-Based Sales Forecasting Dashboard | Olist Brazilian E-Commerce

This project is an end-to-end **predictive and prescriptive analytics dashboard** for forecasting monthly sales using the **Olist Brazilian E-Commerce dataset**. The goal is to predict upcoming sales trends, measure forecast confidence, and deliver actionable business insights through a professional **Power BI dashboard**.

<img width="1365" height="762" alt="olistdashboard" src="https://github.com/user-attachments/assets/67c67936-2b4e-4e1a-955f-bdb7d39ecf61" />


---

## 🎯 Project Goals

- 📈 Build a predictive model using **Prophet** to forecast monthly sales
- 📊 Visualize both actual and forecasted sales with **Power BI**
- 🎯 Deliver clear business insights using **KPI cards, trend analysis, and confidence intervals**
- 🎯 Calculate **forecast accuracy** to evaluate model performance
- 🤖 Demonstrate skills in **data science + business intelligence integration**

---

## 🧮 Key Metrics & Features

| Metric                     | Description                                                         |
|----------------------------|----------------------------------------------------------------------|
| `Sum of Sales`             | Total historical sales across months (Actual)                        |
| `Sum of Predicted_Sales`   | Forecasted sales values from Prophet model                           |
| `Forecast Accuracy %`      | Accuracy of predictions compared to actual sales                     |
| `Confidence Intervals`     | 95% upper and lower bound for forecasted values                      |

---

## 🧠 Business Insights (Generated)

- Sales are projected to grow steadily over the next 6 months.
- **November** is expected to be the peak month — stock up inventory.
- Forecast accuracy can be further improved with product-level and region-specific models.

---

## ⚙️ Tech Stack & Tools

- **Python (Google Colab)**
  - `pandas`, `prophet`, `matplotlib`
- **Power BI Desktop**
  - Forecasting dashboard design and KPI visuals
- **Excel** (for intermediate export)
- **Data Source**: [Olist Public Dataset](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

---

## 🔄 Process Overview

### 1. Data Preparation (Colab / Python)
- Loaded `order_items`, `orders`, and other relevant tables
- Aggregated monthly sales using pandas
- Built forecasting model using Facebook Prophet

### 2. Forecasting
- Predicted next 12 months of sales
- Extracted upper and lower confidence intervals
- Exported `monthly_sales` and `forecast_output` to CSV

### 3. Dashboard Development (Power BI)
- Imported combined CSVs for actual and forecast
- Built:
  - 📈 Line chart for Actual vs Forecast
  - 📊 Forecast with Confidence Interval
  - 💳 KPI Cards (Actual Sales, Forecast Sales, Forecast Accuracy)
  - 🎛️ Slicers for Type (Actual/Forecast) and Date

---

## ✨ Highlights

- 🔍 **Forecast Accuracy Achieved**: `17%` error, showing realistic trends  
- 🧠 Used **Prophet’s confidence bounds** to communicate uncertainty  
- 📊 Clean, interactive Power BI dashboard suitable for stakeholders and execs  
- 📦 Ready to expand to include **product/category-level forecasts**

---

## 📁 Folder Structure

```bash
/olist-sales-forecasting/
│
├── olistdashboard.PNG              # Final dashboard snapshot
├── olist_combined_sales.csv        # Actual + Forecast sales (for Power BI)
├── olist_sales_forecast.csv        # Forecast with confidence bounds
├── README.md                       # Project documentation
└── prophet_forecasting_code.ipynb  # Notebook used to train Prophet model
