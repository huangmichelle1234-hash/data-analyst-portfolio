# 🧩 Exploring Biodiversity and Conservation Across U.S. National Parks

## 🧭 Project Overview

This project explores patterns of biodiversity across four major U.S. National Parks — **Yellowstone**, **Yosemite**, **Bryce**, and **Great Smoky Mountains** — using data from the *Codecademy Biodiversity in National Parks* dataset.

The goal was to understand how species diversity and conservation status vary across parks, and to identify whether **protected species are observed less frequently** compared to non-protected species.

### 🔍 Key Questions Explored
- What categories of species are most common across parks?  
- Which parks have the highest total number of species observations?  
- What proportion of species are currently under protection in each park?  
- Which conservation statuses are most common in Yosemite National Park?  
- How do observation counts relate to conservation status — are protected species observed less frequently?  

---

## 🧹 Data Cleaning & Preparation

**Steps Taken**
- Loaded and inspected two datasets: `species_info.csv` and `observations.csv`  
- Standardized column names and stripped extra whitespace  
- Filled missing values in `conservation_status` with `"No Intervention"`  
- Dropped duplicate records and ensured unique species per park  
- Merged both datasets on `scientific_name` to create a unified DataFrame called `biodiversity`  

**Example Code:**
```python
biodiversity = pd.merge(observations, species_info, on='scientific_name', how='inner').drop_duplicates()
biodiversity['conservation_status'] = biodiversity['conservation_status'].fillna('No Intervention')
```
---
## 📊 Exploratory Data Analysis (EDA)
1️⃣ Species Composition Across Categories
Vascular plants dominate the dataset, accounting for 77% of all recorded species.

Birds and mammals follow as the next most common categories.

```python
category_counts = biodiversity.groupby('category')['scientific_name'].nunique()
percentages = (category_counts / category_counts.sum()) * 100
```

2️⃣ Observations by Park
Yellowstone accounts for 43% of total recorded observations.

It is the most biodiverse park in this dataset.

3️⃣ Species Under Protection
Only 3% of all species are listed under a conservation status.

The majority are categorized as “No Intervention.”

🌲 Focused Analysis: Yosemite National Park
In Yosemite, the most common conservation status among protected species is “Species of Concern.”

This suggests that many species in Yosemite face potential risks but are not yet officially endangered.

📈 Statistical Analysis
Hypothesis:
Protected species are observed less frequently than non-protected species.

Method:

Compared mean observation counts by conservation status.

Conducted a two-sample t-test to determine if the difference is statistically significant.

Example Code:

```python
protected = biodiversity[biodiversity['conservation_status'] != 'No Intervention']['observations']
non_protected = biodiversity[biodiversity['conservation_status'] == 'No Intervention']['observations']

t_stat, p_val = ttest_ind(protected, non_protected, equal_var=False)
Results:
```
T-statistic: Negative

P-value: < 0.05 → Statistically significant difference

Interpretation:
Protected species are observed significantly less frequently than non-protected species.
This likely reflects lower population densities or restricted habitats among protected groups.

---
## 💡 Insights & Takeaways
Insight	Key Finding
🟢 Most Observations	Yellowstone National Park — 43% of all recorded observations
🌿 Dominant Category	Vascular Plants — 77% of all species
🛡️ Protection Coverage	Only 3% of species are under protection
🌲 Yosemite Focus	Most protected species are classified as Species of Concern
📉 Observation Frequency	Protected species are observed less frequently (statistically significant)

---
## 🧠 Conclusion & Next Steps
This analysis highlights the uneven distribution of biodiversity and conservation effort across U.S. National Parks.
While most species remain unprotected, a small fraction face measurable ecological challenges that may reduce observation rates.

---
## 🚀 Future Directions
Incorporate seasonal or temporal trends in species observations

Integrate climate and land-use data to study environmental correlations with biodiversity

Track temporal changes in conservation status over time

Expand analysis to include more national parks for broader insight

🧰 Tools & Libraries
Python: Pandas, NumPy, Matplotlib, SciPy

IDE: Jupyter Notebook

Dataset: Codecademy Biodiversity in National Parks
