# 📦 E-Commerce Funnel & Retention Analysis

## 📌 Project Overview

This project analyzes user behavior from an e-commerce company's website by turning raw event logs into actionable business metrics. The goals were to:

- Construct a **conversion funnel** showing user progression from product view to purchase  
- Conduct a **cohort analysis** to evaluate monthly retention patterns post-purchase

📄 [View Full Project Spreadsheet](https://docs.google.com/spreadsheets/d/1mP457L7VC0wt6mznyZBxOQeP3lBSEBWfranspaMT7SI/edit?gid=868644233#gid=868644233)

---

## 🗂️ Dataset

The analysis uses raw user event logs available in the following spreadsheet:

📊 [View Raw Dataset – raw_user_activity](https://docs.google.com/spreadsheets/d/1yuavBZ4OYYUD1opH-dq0d6nejREDy8f0ozumT9-yEuo/edit#gid=0)

Key columns include:
- `user_id`: Unique user identifier  
- `event_type`: Type of activity (view, cart, purchase)  
- `category_code`: Product category  
- `brand`: Product brand  
- `event_time`: Timestamp of the event  

---

## 🔍 Key Questions Answered

1. What does the conversion funnel look like across product view, cart, and purchase stages?  
2. How well does the company retain users over time after their first purchase?

---

## 🧼 Data Cleaning & Preparation

Performed in Excel:
- Converted `event_time` to a readable datetime format  
- Categorized events into funnel stages  
- Assigned `cohort_month` and `event_month` for retention tracking  
- Created pivot tables to analyze retention by cohort  

---

## 📈 Visualizations

### 1. Conversion Funnel  
![Conversion Funnel](visualizations/conversion_funnel.png)  
**Insight:**  
Only 29% of users who view a product add it to their cart, and just 10% complete a purchase. There's a sharp drop at each stage — especially from cart to checkout — indicating opportunities to optimize the buying journey.

---

### 2. Cohort Analysis – Unique User Count  
![Cohort Analysis](visualizations/cohort_analysis.png)  
**Insight:**  
Retention sharply declines after the first month. Very few users return 2–4 months after their first purchase, especially from the late 2020 cohorts.

---

### 3. Cohort Analysis – Retention Rates (%)  
![Retention Rates](visualizations/retention_rates.png)  
**Insight:**  
Most cohorts retain less than 5% of their users beyond the second month. Long-term engagement remains a challenge, highlighting the need for better post-purchase follow-up and incentives.

---

## 🧠 Assumptions

- Each `user_id` represents a unique customer  
- Users begin their journey with a `view` event and progress through `cart` to `purchase`  
- A user's cohort is based on the month of their **first purchase**

---

## 🛠️ Tools Used

- Excel (Data Cleaning & Pivot Tables)  
- Tableau Public (Data Visualization)  
- GitHub (Project Versioning & Documentation)

---

🚀 Project submission for the Spreadsheet Data Analysis sprint (TripleTen BI Program).
