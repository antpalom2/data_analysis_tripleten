# 📦 E-Commerce Funnel & Retention Analysis

## 📌 Project Overview

This project analyzes user behavior from an e-commerce company's website by turning raw event logs into actionable business metrics. The goals were to:

- Construct a **conversion funnel** showing user progression from product view to purchase  
- Conduct a **cohort analysis** to evaluate monthly retention patterns post-purchase

📄 [View Full Project Spreadsheet](https://docs.google.com/spreadsheets/d/1mP457L7VC0wt6mznyZBxOQeP3lBSEBWfranspaMT7SI/edit?gid=868644233#gid=868644233)

---

## 📚 Skills & Techniques Applied

Throughout this project, I applied the following skills as part of the Spreadsheet Data Analysis sprint:

### 🧼 Data Cleaning & Preparation
- Identified and resolved inconsistencies using tools like **Text to Columns**, **Remove Duplicates**, and **Find & Replace**
- Applied **data validation rules** to control column input values
- Used **datetime, text, and lookup functions** (`TEXT`, `MONTH`, `YEAR`, `VLOOKUP`) to clean and transform raw event logs

### 📊 Analysis & Modeling
- Created **pivot tables** to aggregate user activity by funnel stage and cohort month
- Grouped users into **monthly acquisition cohorts** using timestamp logic
- Measured **conversion rates** and **user retention trends** using calculated fields

### 📈 Visualization & Communication
- Built **funnel and retention charts** (bar, line, and matrix formats) to support business storytelling
- Formatted and documented spreadsheets for clear stakeholder presentation
- Ensured clean chart layouts, labeled axes, and logical spreadsheet organization

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

## 📁 File Structure

The project spreadsheet includes the following sheets:

- **raw_user_activity**  
  Contains all user activity logs:
  - `user_id`, `event_type`, `category_code`, `brand`, `event_time`  
  - Used to construct the funnel and cohort analyses

- **conversion_funnel**  
  Aggregated view of user progression through:
  - Product View → Cart → Purchase  
  - Includes conversion rates by event type and brand

- **cohort_retention**  
  User retention matrix:
  - Assigns users to `cohort_month` based on first purchase  
  - Tracks retention across future months using pivot tables

- **pivot_tables**  
  Supporting tables for visualizations:
  - Conversion rate breakdowns  
  - Retention summaries  
  - Event counts by stage and brand

---

## 🛠️ Tools Used

- Excel (Data Cleaning & Pivot Tables)  
- GitHub (Project Versioning & Documentation)

---

🚀 Project submission for the Spreadsheet Data Analysis sprint (TripleTen BI Program).
