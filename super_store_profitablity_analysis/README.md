# 📊 Superstore Profitability Analysis

This project analyzes transaction data from a fictional superstore to uncover key business metrics around profitability, customer behavior, and regional trends.

By exploring category-level and regional performance, the goal is to inform data-driven recommendations that help improve operational strategy, optimize product offerings, and focus on geographic areas with high potential for profitability.

🔗 [View Tableau Story](https://public.tableau.com/views/superstore-profitability-analysis/SuperstoreProfitabilityAnalysis?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)  
📄 [Download Dataset (Excel)](https://practicum-content.s3.us-west-1.amazonaws.com/data-eng/remodeled/dvwt/Superstore.xls?etag=4616d537c163874941cf5fc3c9002fa8)

---

## 📚 Skills & Techniques Applied

### 📈 Visual Analytics
- Built bar charts, scatter plots, and heatmaps to highlight profitability and returns  
- Designed state-by-month views to identify **regional + seasonal trends**  
- Compared return rates to profits to identify **quality or demand issues**

### 🎯 Dashboard Design
- Clean formatting with consistent colors and scales  
- Each chart answers a **specific business question**  
- Structured for narrative flow → from profit sources → losses → returns → seasonality → recommendations  

### 🔧 Data Structuring in Tableau
- Used **calculated fields** for return rate and avg profit  
- Aggregated sub-categories and states for summary insights  
- Applied filters and grouping directly in Tableau (no external preprocessing)  

---

## 🔍 Objective
Translate raw transaction data into **actionable business insights** by identifying:
- High-performing products and sub-categories  
- Consistent loss-making products and regions  
- Customer and product return trends  
- Seasonal and state-level profit patterns  

---

## 📊 Visualizations & Insights

### 1) Profits & Losses by Region × Sub-Category
![Profits & Losses](visualizations/profits_losses.png.png)

**Insights**
- **Copiers dominate profit** (≈ **$76K**) followed by **Accessories (~$50K)** and **Chairs (~$40K)**.  
- **Consistent loss makers:** **Tables (~−$23K)**, **Bookcases (~−$3.7K)**, **Machines (~−$2K)**, **Supplies (~−$0.9K)**.  
- **Central region + Binders** is a standout problem area (**≈ −$20.6K**).  
**Action:** Prioritize Copiers & Chairs; review pricing/vendor terms for loss-makers.

---

### 2) Top 10 Products by Profit
![Top Products](visualizations/top_products.png.png)

**Insights**
- **Canon imageCLASS** far outpaces all others (**$38K+ profit**).  
- Long-tail products range **$12K–$4.9K**.  
**Action:** Keep these SKUs in stock, feature in promos, and bundle for cross-sells.

---

### 3) Bottom 10 Products by Profit
![Bottom Products](visualizations/bottom_products.png.png)

**Insights**
- **GBC DocuBind system** is worst performer (**≈ −$20.4K**).  
- Other niche tech (e.g., 3D Printers) also drag down profit.  
**Action:** Discontinue or move to **special-order only**; renegotiate vendor terms.

---

### 4) Avg Profit vs Avg Return Rate (Sub-Category)
![Avg Profit vs Return Rate](visualizations/avg_profit_vs_return.png.png)

**Insights**
- **Copiers** → strong profit + low return rate (**best quadrant**).  
- **Machines, Fasteners, Chairs** → higher returns (~28–35%) with only moderate profit.  
- **Furnishings & Bookcases** → low returns but weak profit.  
**Action:** Defend Copiers, and audit high-return sub-categories for vendor/QA issues.

---

### 5) Returns by Product (Top Return Rates)
![Returns by Product](visualizations/returns_by_product.png.png)

**Insights**
- Several SKUs (e.g., **Zebra GK420t, Okidata B401, HP Deskjet, Cisco 501G, Canon ImageCLASS**) show **100% returns**.  
- Others still extreme (**93–92% return rates**).  
**Action:** Immediate QA/vendor investigation. Remove from general stock or restrict sales.

---

### 6) Returns by Customer (Top Returners)
![Returns by Customer](visualizations/returns_by_customer.png.png)

**Insights**
- Customers like **Roland Murray & Hilary Holden** return **100% of orders**.  
- Top 10 returners average **86–100% return rates**.  
**Action:** Flag accounts for manual review, enforce stricter return policies, or conduct outreach.

---

### 7) State-Level Profitability & Seasonality
![State Seasonality](visualizations/state_seasonality.png.png)

**Insights**
- **Seasonal peaks:** Indiana (Oct ≈ $643), Vermont (Nov ≈ $596), Washington (Aug ≈ $521).  
- **Chronic losses:** Ohio, North Carolina, and New York in specific months.  
**Action:** Target ads/inventory in peak states-months, reduce exposure in weak periods.

---

## 🧠 Conclusion & Recommendations
1. **Double down on winners** → Copiers, Canon imageCLASS, Accessories.  
2. **Cut or fix losers** → Tables, Bookcases, GBC DocuBind.  
3. **Fix returns problem** → Address high-return SKUs & chronic customers.  
4. **Time campaigns** → Focus on seasonal peaks (Indiana-Oct, Vermont-Nov, Washington-Aug).  

By acting on these, the superstore can reduce waste, increase margins, and better match demand.

---

## 🛠 Tools Used
- **Tableau Public** → Visualization & Storytelling  
- **GitHub** → Version control & project portfolio  

🚀 Final project submission for the *Data Visualization with Tableau* sprint in TripleTen’s BI Analyst program.
