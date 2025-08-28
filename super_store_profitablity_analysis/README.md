# 📊 Superstore Profitability Analysis  

This project analyzes transaction data from a fictional superstore to uncover key business metrics around profitability, customer behavior, and regional trends.  

By exploring category-level and regional performance, the goal is to inform data-driven recommendations that help improve operational strategy, optimize product offerings, and focus on geographic areas with high potential for profitability.  

---

## 📊 View Full Tableau Dashboard  
[🔗 Tableau Story: Superstore Profitability Analysis](https://public.tableau.com/views/superstore-profitability-analysis/SuperstoreProfitabilityAnalysis?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)  

## 📄 Download Dataset  
[🔗 Superstore Dataset (Excel)](https://practicum-content.s3.us-west-1.amazonaws.com/data-eng/remodeled/dvwt/Superstore.xls?etag=4616d537c163874941cf5fc3c9002fa8)  

---

## 📚 Skills & Techniques Applied  
This project was completed as part of the **Data Visualization with Tableau** sprint in TripleTen's Business Intelligence Analyst program.  

### 📈 Visual Analytics  
- Built bar charts and scatter plots to highlight profitability trends across products and regions  
- Designed highlight tables to visualize sub-category and state-level profit differences  
- Compared return rates and profit margins by customer and product  

### 🎯 Dashboard Design Principles  
- Emphasized clean visual communication with consistent formatting and color use  
- Structured charts around actionable insights (e.g., products to stop selling, top-performing regions)  
- Focused each visual on a specific business question to maintain clarity and narrative focus  

### 🔧 Data Structuring in Tableau  
- Used calculated fields and filters to derive metrics like return rate and profit average  
- Aggregated sub-categories and states for summary-level insights  
- Applied filters and visual grouping directly in Tableau (no external preprocessing)  

---

## 🔍 Objective  
To translate raw transaction data into actionable business insights by identifying:  
- High-performing products and sub-categories  
- Product lines and regions with consistent losses  
- Customer return trends and their effect on profits  
- Seasonal and regional profit trends across the United States  

---

## 📊 Key Visualizations & Insights  

### 1. Profits & Losses by Region and Sub-Category  
![Profits & Losses](visualizations/profits_losses.png)  
**Insight:** Copiers in the West and Chairs in the East are strong profit contributors, reflecting regional demand. In contrast, Binders in the Central region and Tables in the East consistently lose money.  

---

### 2. Top Selling Products by Profit  
![Top Products](visualizations/top_products.png)  
**Insight:** A small number of products contribute disproportionately to overall profit, underscoring the **80/20 rule (Pareto Principle)**.  

---

### 3. Bottom 10 Products by Profit  
![Bottom Products](visualizations/bottom_products.png)  
**Insight:** Several products generate **consistent losses** (e.g., over –$8,000). These should be reevaluated for vendor renegotiation, pricing adjustments, or removal.  

---

### 4. Average Profit vs. Average Return Rate  
![Avg Profit vs Return](visualizations/avg_profit_vs_return.png)  
**Insight:** Some products with low or negative profits also have **high return rates**, signaling quality issues or poor customer satisfaction.  

---

### 5. Returns by Customer  
![Returns by Customer](visualizations/returns_by_customer.png)  
**Insight:** A small group of customers show **90–100% return rates**, driving disproportionate profit erosion.  

---

### 6. Returns by Product  
![Returns by Product](visualizations/returns_by_product.png)  
**Insight:** Certain products (especially printers, phones, and furniture items) have **extremely high return rates**, suggesting vendor or quality issues.  

---

### 7. State-Level Seasonality & Profitability  
![State Seasonality](visualizations/state_seasonality.png)  
**Insight:** Profitability varies significantly by state and month. States like **Indiana (October)**, **Vermont (December)**, and **Washington (March)** show peak seasonal performance.  

---

## 🧠 Conclusion & Recommendations  

1. **Focus on High-Value Categories & Products**  
   - Double down on **Technology and Office Supplies**, especially Copiers and Canon ImageCLASS.  

2. **Address Loss-Making Categories & Products**  
   - Reevaluate **Furniture (Tables, Bookcases)** and consistently underperforming products.  

3. **Manage Returns More Effectively**  
   - Investigate chronic returners (90–100% rates).  
   - Review vendors and enforce stronger return policies.  

4. **Leverage Regional & Seasonal Insights**  
   - Capitalize on strong states (**Indiana, Vermont, Washington**) by replicating strategies in weaker markets.  
   - Align marketing with **peak months (September, December)** to maximize profitability.  

---

## 🛠 Tools Used  
- Tableau Public (Data Visualization)  
- GitHub (Project Versioning & Collaboration)  

🚀 Final project submission for the **Data Visualization with Tableau** sprint at TripleTen.  
