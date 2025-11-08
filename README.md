# 🇨🇱 Chile GDP and Life Expectancy Analysis (2000–2016)

## 📊 Overview
This project explores the relationship between **economic growth (GDP)** and **life expectancy** in Chile from **2000 to 2016**.  
Using data analysis and visualization techniques in Python, the project investigates how changes in GDP correlate with improvements in life expectancy — and whether economic performance can be used to **predict** health outcomes.

---

## 🧠 Objectives
- Analyze **year-over-year growth** in GDP and life expectancy.  
- Identify **divergence years** where the two metrics move in opposite directions.  
- Build a **linear regression model** to determine if GDP predicts life expectancy.  
- Visualize economic and health trends over time.

---

## 📂 Dataset
**Source:** CSV file containing:  all_data.csv
`Country`, `Year`, `Life expectancy at birth (years)`, `GDP`

Data covers Chile from 2000 to 2016.

---

## ⚙️ Tools & Libraries
- **Python** (pandas, matplotlib, seaborn, scikit-learn)
- **Jupyter Notebook**
- **NumPy** for numerical calculations
- **Linear Regression** for predictive modeling

---

## 🔍 Analysis Steps
1. **Data Cleaning** – Removed nulls and standardized column names.  
2. **Growth Rate Calculation** – Computed annual percentage changes for GDP and life expectancy.  
3. **Visualization** – Created line and dual-axis plots to compare trends.  
4. **Regression Modeling** – Used `LinearRegression` to predict life expectancy from GDP.  
5. **Interpretation** – Summarized patterns, anomalies, and insights.

---

## 📈 Key Insights
- **Steady Growth:** Life expectancy rose gradually from **77.3 → 78.0 years (2000–2004)**, while GDP showed sharper fluctuations.  
- **Peak GDP Growth:** **2004** recorded the **highest GDP growth rate (31.16%)**.  
- **Divergence Years:** **2002, 2010, 2014, and 2015** — life expectancy and GDP moved in opposite directions.  
- **Strong Correlation:** Linear regression revealed a **positive relationship** between GDP and life expectancy (**R² = 0.902**).  
- **Prediction:** Based on the regression model, Chile’s **predicted life expectancy for 2024** is **~81.0 years**.  
- **Interpretation:** While long-term trends show strong alignment, short-term divergences suggest that **social and policy factors** may buffer health outcomes from immediate economic changes.

---

## 📊 Visualizations
- GDP and Life Expectancy Trends (2000–2016)
- Year-over-Year Growth Rate Comparison
- Divergence Highlight Plot
- Linear Regression Fit (GDP vs. Life Expectancy)

*(Example plots can be found in the `figures/` folder.)*

---

## 💡 Conclusion
Economic growth in Chile has closely aligned with improvements in life expectancy over the studied period.  
However, short-term fluctuations and divergence years highlight that **socioeconomic development**, not just GDP growth, contributes to national health outcomes.

---

## 🚀 Future Work
- Expand analysis to multiple Latin American countries for comparison.  
- Incorporate additional indicators like **education level**, **healthcare spending**, and **inequality metrics**.  
- Explore **time-series forecasting** models (e.g., ARIMA, Prophet) for life expectancy predictions.

---

## 🧾 Author
**Michelle Huang**  
📍 Los Angeles, CA  
🔗 [GitHub](https://github.com/huangmichelle1234-hash/data-analyst-portfolio) | 📧 huang.michelle1234@gmail.com  

---

> *“Data tells the story of progress — this project explores how a nation’s economy and its people’s well-being grow together.”*
