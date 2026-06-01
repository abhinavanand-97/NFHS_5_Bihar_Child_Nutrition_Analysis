# 👶 NFHS-5 Bihar Child Nutrition Analysis

A beginner data analysis project exploring child nutrition and health indicators across all **38 districts of Bihar**, using data from India's National Family Health Survey — Round 5 (NFHS-5).

---

## 📌 Project Overview

Bihar is one of India's most populous states and faces significant child health challenges. This project digs into NFHS-5 district-level data to understand how child malnutrition, breastfeeding, and healthcare access vary across Bihar's districts — and how these factors are connected to each other.

---

## 📂 Dataset

- **Source:** NFHS-5 (National Family Health Survey, 2019–21)
- **File:** `NFHS-5 dataset — 706 districts, 109 columns.csv`
- **Scope:** 706 districts across India | **38 Bihar districts used** in this project
- **Total Columns:** 109 | **6 key health indicators selected**

### Indicators Analyzed
| Column | What It Means |
|---|---|
| Stunting | Children under 5 with low height-for-age (chronic malnutrition) |
| Wasting | Children under 5 with low weight-for-height (acute malnutrition) |
| Underweight | Children under 5 with low weight-for-age |
| Breastfeeding | Infants under 6 months exclusively breastfed |
| Institutional Delivery | Births that happened in a hospital/health facility |
| Child Anaemia | Children age 6–59 months with anaemia |

---

## 🛠️ What Was Done

1. **Data Filtering** — Extracted Bihar-specific rows from the national dataset
2. **Column Selection & Renaming** — Picked 6 relevant health indicators and renamed them for clarity
3. **Data Cleaning** — Removed special characters, converted to numeric, handled missing values using median imputation
4. **Exploratory Data Analysis (EDA)** — 4 visualizations covering district rankings, comparisons, correlations, and averages
5. **Correlation Analysis** — Studied how malnutrition indicators relate to breastfeeding and institutional delivery rates
6. **District-Level Insights** — Identified best and worst performing districts for each indicator

---

## 📊 Visualizations

- **Bar Chart** — Top 10 districts with highest stunting rates
- **Grouped Bar Chart** — Stunting vs Wasting vs Underweight across all 38 districts
- **Correlation Heatmap** — Relationships between all 6 health indicators
- **Average Indicator Chart** — Bihar's overall average for each health metric

---

## 🔍 Key Findings

- **Underweight & Wasting** are strongly correlated (0.73) — they tend to rise and fall together across districts
- **Exclusive Breastfeeding** shows a protective effect — higher breastfeeding rates link to lower wasting and underweight
- **Institutional Deliveries** correlate with lower stunting — hospital births give children a healthier start
- **Stunting & Wasting are negatively correlated** — they are driven by different regional factors and don't always co-occur in the same districts

---

## 🧰 Libraries Used

```
pandas
matplotlib
seaborn
```

---

## 🚀 How to Run

1. Clone this repository
2. Install dependencies:
   ```bash
   pip install pandas matplotlib seaborn
   ```
3. Place the dataset CSV in the same folder as the script
4. Update the file path in the script and run:
   ```bash
   python nfhs_5_bihar_child_nutrition_analysis.py
   ```
   Or open it directly in **Google Colab**

---

## 👤 About

This is a beginner-level EDA project — one of my first attempts at working with real government survey data. The goal was to practice data cleaning, visualization, and drawing meaningful insights from a large dataset. Feedback is welcome! 🙌
