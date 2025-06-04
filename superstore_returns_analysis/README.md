# Superstore Returns Dashboard Analysis

This project was built as part of a junior analyst case study focused on return behavior at a fictional retail superstore. The goal was to identify what’s driving customer returns and recommend strategic solutions to minimize them — without compromising customer experience.

---

## 🔍 Objective

To help company leadership understand:
- What categories, customer types, or time periods are return-prone?
- Are there geographic patterns in return rates?
- How do returns affect profitability?
- What corrective actions are most promising?

This Tableau dashboard and multi-page story provides a breakdown of trends, customer behaviors, and KPIs to support executive decisions.

---

## 🗂️ Data Overview

The analysis was based on:
- **Order history** (2018–2021) with categories, sales, profit  
- **Return indicators** to flag returned transactions  
- **Customer names and locations** to evaluate frequency and clustering  
- **Derived KPIs** including average return rate, profit, and correlation metrics  

---

## 📊 Dashboard Overview

![Final Dashboard](visualizations/dashboard.png)

This executive view summarizes return rates over time, by state, category, and customer — as well as profitability trends and correlations.

---

## 📘 Key Visualizations & Insights

### 1. Monthly Return Rates
![Monthly Return Rates](visualizations/monthly_return_rates.png)  
**Insight:** Return rates spike in September and December, aligning with the fall and holiday shopping seasons — likely tied to increased volume and expectation mismatches.

---

### 2. State Return Rates
![State Return Rates](visualizations/state_return_rates.png)  
**Insight:** Western and Northeastern states show higher return rates, suggesting geographic variations in customer satisfaction or shipping experiences.

---

### 3. Return Rate by Category
![Return Rate by Category](visualizations/average_return_rate_per_category.png)  
**Insight:** Technology leads in return rates, followed closely by Office Supplies and Furniture. This may reflect complexity, compatibility, or expectation gaps.

---

### 4. Return Rate vs. Profit Over Time
![Return vs Profit](visualizations/rates_vs_profit.png)  
**Insight:** Profit grew sharply in 2021 despite steady return rates, pointing to improved efficiency or pricing strategies.

---

### 5. Sales vs. Returns Correlation
![Sales vs Returns](visualizations/correlation_between_sales_&_returns.png)  
**Insight:** A positive correlation exists — high-sales items often produce more returns. However, categories like Phones perform well with low return rates despite high volume.

---

### 6. High-Return Customers
![High Return Customers](visualizations/customers_with_returns.png)  
**Insight:** Some customers have near-100% return rates. These cases could reflect chronic dissatisfaction, fraud, or unclear policies — and warrant targeted engagement.

---

## ✅ Strategic Recommendations

- **Improve product detail and onboarding** for high-return categories like Technology.  
- **Target high-return regions** with localized return policies or proactive outreach.  
- **Flag high-return customers** for review, feedback collection, or loyalty alternatives.  
- **Optimize seasonal messaging** to reduce regret-based returns during high-volume periods.

---

## 💡 Business Questions Answered

- **Why focus on return rate instead of total returns?**  
  Total returns help identify which items are returned the most, but **return rate** is a better metric for comparing trends over time, by location, and across categories — because it accounts for differences in sales volume.

- **What might explain high return rates?**  
  Technology products during the holiday season show higher return rates, possibly due to increased volume and higher expectations. Regional patterns suggest potential fulfillment or delivery issues in certain states.

- **What can we do about high-return customers and regions?**  
  We recommend sending targeted surveys to both **customers with extremely high return rates** and customers in **high-return states**. These insights can inform future shipping, manufacturing, and marketing strategies.

---

## 🧾 Conclusions

We suggest a **deeper investigation** into:

- Why higher sales often correlate with higher return rates  
- Whether **holiday purchases** (especially in Technology) create more post-purchase dissatisfaction  
- If **specific regions are receiving more defective or mishandled items**  
- Engaging high-return customers and testing **region-specific improvements**

These recommendations aim to balance return rate reduction with continued customer satisfaction and sales performance.

---

## 🛠 Tools Used

- Tableau  
- Excel  
- GitHub

---

> 📘 Final submission for Business Intelligence Capstone: “Storytelling with Data”
