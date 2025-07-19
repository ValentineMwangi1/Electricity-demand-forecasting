#  Electricity Demand Forecasting with SARIMA

This project focuses on analyzing and forecasting daily electricity demand using time series data. Leveraging statistical modeling (SARIMA), the project aims to uncover patterns in electricity consumption and predict future demand, enabling data-driven energy planning.

---

##  Project Objectives

- Perform Exploratory Data Analysis (EDA) on electricity demand data.
- Detect trends, seasonality, and variability in historical usage.
- Build a SARIMA (Seasonal ARIMA) model to forecast the next 90 days of demand.
- Visualize historical and predicted electricity usage with confidence intervals.
- Provide insights to support smart energy decision-making.

---

##  Dataset

The dataset used contains historical daily electricity demand data. Each record includes:
- `Date`: The observation date.
- `Electricity_Demand_MWh`: Total electricity consumed in Megawatt-hours (MWh).

The dataset was preprocessed to handle time-based indexing and converted into a stationary format for modeling.

---

##  Exploratory Data Analysis (EDA)

Key insights from EDA:
- The time series shows clear **weekly and monthly seasonality**.
- There are **periodic spikes and dips**, indicating behavioral or environmental patterns.
- Rolling averages and differencing helped reveal underlying trends and made the data more suitable for SARIMA modeling.

---

##  Time Series Modeling (SARIMA)

The SARIMA model was selected due to its ability to:
- Handle trend and seasonality.
- Generate robust predictions for structured time series data.

### Model Configuration
We used the `SARIMAX` model from `statsmodels` with the following configuration:

- **Order (p,d,q)**: (2,1,2)
- **Seasonal Order (P,D,Q,s)**: (1,1,1,7) – capturing weekly seasonality
- **Forecast Horizon**: 90 days into the future

---

##  Forecast Output

The final forecast revealed:

- A **noticeable upward trend** in electricity demand over the forecasted 90-day period.
- A smooth curve reflecting seasonal behavior, as captured by the SARIMA model.
- **Confidence intervals** to reflect uncertainty in predictions.

The forecast plot visually communicates both the historical trend and future expectations, aiding in capacity planning and demand management.

---

## 
---

## Tools & Libraries Used

- **Python 3.10+**
- **Pandas** – Data manipulation
- **Matplotlib** – Plotting
- **Statsmodels** – SARIMA time series modeling
- **Jupyter Notebook** – Analysis and development

---

## Author

Valentine Njeri 
Aspiring Data Analyst | Skilled in Python, Excel, and Power BI  


---

##  Next Steps
- Add other features (temperature, holidays) to build a multivariate forecast
- Deploy the model or dashboard to track live updates

---

> Disclaimer: This project is for educational purposes. Dataset used may be synthetic or anonymized.



