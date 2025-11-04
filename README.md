# 🚍 Public Transport Passenger Forecast 📈

<img width="1024" height="1024" alt="Gemini_Generated_Image_6vebvu6vebvu6veb" src="https://github.com/user-attachments/assets/bfa5a319-0450-422a-b505-e934f213b8c3" />


An interactive analytics and forecasting solution powered by machine learning, providing actionable insights into public transit demand patterns and future predictions. This project uses a **Random Forest Regression** approach, handling time-series travel data and delivering professional-grade automated reports.

---

## 🌟 **Overview & Motivation**

Understanding how many people use public transport—and when—is vital for city planners, transit agencies, and service operators. This real-world project analyzes passenger journeys from July 2019 to September 2024 across six major service categories. We visualize historical trends, detect hidden patterns (weekdays vs weekends, service correlations), and provide a **7-day forecast** for better staffing, investment, and strategic planning.

---

## 🛠️ **Tech Stack**
- **Python 3.8+**: Programming language
- **Jupyter Notebook** (`public_transit_forecast.ipynb`): All code, workflow, and results in a single interactive notebook
- **Pandas**: Data wrangling & CSV loader
- **Matplotlib & Seaborn**: Trend visualization and insightful plots
- **Scikit-learn**: Machine learning (Random Forest Regression, cross-validation)
- **NumPy & datetime**: Calculations and date/time handling

---

## 🔥 **Key Features**

- **End-to-End Workflow**: From raw CSV to forecast and actionable insights, everything is documented step-by-step.
- **Visual Analytics**: Professional plots for:
  - Total passengers over time
  - Service-wise usage breakdown
  - Correlation heatmaps (which services rise and fall together)
  - Weekday vs weekend demand
  - 7-day forecast with uncertainty bands
- **Machine Learning Forecast**: Random Forest model predicts the next week’s ridership with cross-validated performance metrics.
- **Automated Reporting**: Technical summary (`Technical_Report-1.txt`) with:
  - Key findings, actionable recommendations, limitations, and model confidence levels.
- **Actionable Business Insights**: Targets peak days, resource allocation, marketing, and maintenance with data-driven advice.

---

## 📊 **Major Insights**

- **Rapid Route** handles the biggest share (39%) of traffic—focus investments and service monitoring here.
- **Weekday traffic** is, on average, **142% higher** than weekends. Monday is the busiest, Sunday the slowest.
- **School Service** is highly unpredictable (106% variation), while **Light Rail** is the most stable (46% variation).
- **Services Move Together**: *Light Rail* and *Rapid Route* are tightly correlated (0.97)—schedule and contingency planning should consider this.
- **Forecast Challenge**: Successful predictions require model adaptability—Random Forest models time-dependent behaviors far better than basic averages or linear regressions.
- **7-Day Passenger Forecast**: Shows a dramatic recent drop (likely actionable or data anomaly—see report).

---

## 🚦 **How It Works**

1. **Load Data**: Read daily passenger counts from CSV (1918 days, 6 services).
2. **Clean & Explore**: Fix missing values, handle outliers, verify time coverage.
3. **Visualize Trends**: Plot time series, peak/bottom days, service-specific usage, and pattern comparisons.
4. **Calculate Correlations**: Heatmaps show how different routes interact.
5. **Model Selection**: Random Forest selected for its ability to learn complex, real-world patterns.
6. **Prediction**: Forecast next 7 days’ passengers using historical patterns and machine learning.
7. **Reporting**: Export all insights and recommendations to a readable TXT file.

---

## 📁 **Project Structure**
```
Kovai.co--public-transit-forecast/
│
├── Dataset/
│   └── Daily_Public_Transport_Passenger_Journeys_by_Service_Type_20250603.csv   # Main dataset file
│
├── Technical_report/
│   └── Technical_Report.txt                      # Technical summary and findings
│
├── forecast plots/
│   ├── 01_total_passengers_trend.png             # Total passenger trend (5-year)
│   ├── 02_individual_services.png                # Service-wise passenger trend
│   ├── 03_correlation_heatmap.png                # Service correlation heatmap
│   ├── 04_day_of_week_pattern.png                # Weekday vs weekend pattern
│   └── 05_forecast_7days.png                     # 7-day passenger forecast
│
├── 7_day_forecast.xls                            # Forecast results (Excel)
├── README.md                                     # This file (project overview & instructions)
├── public_transit_forecast.ipynb                 # Main Jupyter notebook (full workflow & code)

```
