# 💼 Medical Insurance Cost Analysis

## 📊 Overview
This project explores factors that influence **medical insurance charges** using a real-world dataset.  
The dataset includes information on **age, sex, BMI, number of children, smoking status, and charges**.  
The analysis investigates patterns, correlations, and trends to understand which factors most strongly impact insurance costs.

---

## 🧠 Objectives
- Analyze the **distribution of insurance charges**.  
- Examine **average insurance costs by gender**.  
- Compare costs between **parents and non-parents**.  
- Explore how **age affects insurance charges**.  
- Identify which factors have the **strongest correlation** with insurance costs.

---

## 📂 Dataset
**Source:** CSV file `insurance.csv` with the following columns:  
`age`, `sex`, `bmi`, `children`, `smoker`, `charges`  

---

## 🔎 Key Insights

### Distribution of Charges
- Insurance charges are **right-skewed**, with most individuals paying lower amounts and a few paying very high costs.  
- The mean and median provide useful benchmarks for understanding typical charges.

### Gender Differences
- **Males pay more** on average than females.  
- Visual comparison highlights gender-based disparities in insurance costs.

### Parental Status
- Individuals with children (**parents**) generally pay **higher insurance costs** than those without.  
- This trend may reflect age, lifestyle, or additional risk factors.

### Age and Insurance Costs
- Insurance costs **increase with age**, showing a roughly linear trend.  
- Older individuals tend to incur higher charges, reflecting greater health risks.

### Factor Correlations
- **Smoking status** has the **strongest correlation** with insurance charges (~0.79).  
- **Age** is moderately correlated (~0.30).  
- Other factors like BMI, sex, and number of children show smaller correlations.  

---

## 📊 Visualizations
- **Histogram** showing the distribution of insurance charges with mean, median, and range.  
- **Bar charts** comparing average insurance costs by gender and parental status.  
- **Line plot** showing average insurance costs by age.  

*(Plots can be added in a `figures/` folder for GitHub display.)*

---

## 💡 Conclusion
The analysis reveals that **smoking and age are primary drivers** of insurance costs, while other factors like sex, BMI, and number of children have smaller impacts.  
These insights can help insurers better model risk and guide pricing strategies.

---

## 🚀 Future Work
- Apply **predictive modeling** (regression or machine learning) to estimate insurance costs.  
- Investigate **interaction effects**, such as age × smoker status.  
- Incorporate additional health or lifestyle factors to improve predictive accuracy.  
- Build **interactive visual dashboards** for exploratory analysis and reporting.

---

## 🧾 Author
**Michelle Huang**  
📍 Los Angeles, CA  
🔗 [GitHub](https://github.com/huangmichelle1234-hash/data-analyst-portfolio) | 📧 huang.michelle1234@gmail.com

> *“Data-driven insights help us understand risk factors and make informed decisions in healthcare and insurance.”*
