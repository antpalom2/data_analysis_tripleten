# 📊 Superstore Profitability Analysis

This project analyzes transaction data from a fictional superstore to uncover key business metrics around profitability, customer behavior, and regional trends.  

By exploring category-level and regional performance, the goal is to inform data-driven recommendations that help improve operational strategy, optimize product offerings, and focus on geographic areas with high potential for profitability.  

---

## 🔗 Project Links  
- [📊 View Full Tableau Story](https://public.tableau.com/views/superstore-profitability-analysis/SuperstoreProfitabilityAnalysis?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)  
- [📄 Download Dataset (Excel)](https://practicum-content.s3.us-west-1.amazonaws.com/data-eng/remodeled/dvwt/Superstore.xls?etag=4616d537c163874941cf5fc3c9002fa8)  

---

## 📚 Skills & Techniques Applied  

**This project was completed as part of the Data Visualization with Tableau sprint in TripleTen's Business Intelligence Analyst program.**

### 📈 Visual Analytics  
- Built bar charts and scatter plots to highlight profitability trends across products and regions  
- Designed geographic maps to visualize state-level differences in revenue and seasonal performance  
- Used highlight tables to compare return rates and profit margins by category  

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
![Profits & Losses](super_store_profitability_analysis/visualizations/profits_losses.png)  
**Insight:**  
Copiers in the West and chairs in the East are strong profit contributors, reflecting regional demand. In contrast, binders in the Central region and tables in the East consistently lose money. These losses highlight inefficiencies in either pricing, product quality, or local demand patterns.  

---

### 2. Top Selling Products by Profit  
![Top Products](super_store_profitability_analysis/visualizations/top_products.png)  
**Insight:**  
A small number of products contribute disproportionately to overall profit, underscoring the classic **80/20 rule (Pareto Principle)**. Strategic focus on these high-margin products — through better stock availability, promotions, or cross-selling — can maximize revenue with minimal effort.  

---

### 3. Bottom Products by Profit  
![Bottom Products](super_store_profitability_analysis/visualizations/bottom_products.png)  
**Insight:**  
Some products like the **GBC DocuBind** system and CubeX 3D printers generate large losses despite likely high costs. These products should be renegotiated with vendors, repriced, or discontinued to stop draining profitability.  

---

### 4. Average Profit vs. Average Return Rate  
![Avg Profit vs Return](super_store_profitability_analysis/visualizations/avg_profit_vs_return.png)  
**Insight:**  
Some products with low or negative profits also have **high return rates**, signaling dissatisfaction or quality issues. Products in the top-left quadrant (low profit, high returns) are liabilities and should be reviewed for redesign, discontinuation, or vendor reassessment.  

---

### 5. Returns by Customer  
![Returns by Customer](super_store_profitability_analysis/visualizations/returns_by_customer.png)  
**Insight:**  
A small group of customers return nearly **all of their purchases (90–100%)**, which significantly erodes profitability. Managing chronic returners through stricter policies or customer segmentation can reduce losses.  

---

### 6. Returns by Product  
![Returns by Product](super_store_profitability_analysis/visualizations/returns_by_product.png)  
**Insight:**  
Printers, phones, and furniture items show **extremely high return rates** (approaching 100%). This points to vendor issues, quality control problems, or mismatched customer expectations.  

---

### 7. State-Level Seasonality in Profits  
![State Seasonality](super_store_profitability_analysis/visualizations/state_seasonality.png)  
**Insight:**  
Profitability varies significantly by state and month. States like **Indiana (October), Vermont (November), and Washington (March)** show strong seasonal performance and could benefit from targeted advertising during their peak months.  

---

## 🧠 Recommendations  

1. **Focus on High-Value Categories & Products**  
   - Double down on **Technology and Office Supplies**, especially Copiers and Canon ImageCLASS.  
   - Ensure top sellers are always in stock and consider targeted promotions to maximize ROI.  

2. **Address Loss-Making Categories & Products**  
   - Reevaluate **Furniture** (Tables, Bookcases) and products like the GBC DocuBind.  
   - Either renegotiate vendor terms, adjust pricing, or discontinue consistently negative performers.  

3. **Manage Returns More Effectively**  
   - Investigate chronic returners (some customers at **90–100% return rates**).  
   - Review quality or vendor issues with high-return products.  
   - Strengthen return policies to reduce profit erosion.  

4. **Leverage Regional & Seasonal Insights**  
   - Capitalize on strong states (Indiana, Vermont, Washington) by replicating strategies in weaker markets.  
   - Align marketing and inventory with **peak months (September, December)** to maximize profitability.  

---

## 🛠 Tools Used  
- Tableau Public (Data Visualization)  
- GitHub (Project Versioning & Collaboration)  

🚀 Final project submission for the **Data Visualization with Tableau sprint** at TripleTen.  
