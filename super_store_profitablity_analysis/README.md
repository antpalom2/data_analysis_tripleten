# 📊 Superstore Profitability Analysis  

This project analyzes transaction data from a fictional superstore to uncover key business metrics around profitability, customer behavior, and regional trends.  

By exploring category-level and regional performance, the goal is to inform data-driven recommendations that help improve operational strategy, optimize product offerings, and focus on geographic areas with high potential for profitability.  

## 🔗 Project Links  
- [Live Tableau Story](https://public.tableau.com/views/superstore-profitability-analysis/SuperstoreProfitabilityAnalysis)  
- [Dataset: Superstore.xls](https://practicum-content.s3.us-west-1.amazonaws.com/data-eng/remodeled/dvwt/Superstore.xls)  

---

## 📚 Skills & Techniques Applied  

This project was completed as part of the **Data Visualization with Tableau** sprint in **TripleTen's Business Intelligence Analyst program**.  

### 📈 Visual Analytics  
- Built bar charts, highlight tables, and scatter plots to highlight profitability trends across products, regions, and customers.  
- Designed state-level visuals to uncover geographic and seasonal differences in profit.  
- Used return-rate analysis to expose product and customer behaviors driving losses.  

### 🎯 Dashboard Design Principles  
- Clean, consistent formatting and intuitive color encoding (blue = profit, orange/red = loss).  
- Each visualization answers a specific business question (e.g., *Which products to stop selling?*).  
- Story points build a clear narrative from profitability → losses → returns → recommendations.  

### 🔧 Data Structuring in Tableau  
- Created **calculated fields** (e.g., average return rate, profit ratio).  
- Aggregated **sub-categories, products, and states** for actionable summary insights.  
- Applied **filters** and visual grouping to highlight problem areas and success drivers.  

---

## 🔍 Objective  
Transform raw transaction data into actionable business insights by identifying:  
- High-performing products and sub-categories  
- Product lines and regions with consistent losses  
- Customer return trends and their effect on profits  
- Seasonal and regional profit trends across the U.S.  

---

## 📊 Key Visualizations & Insights  

### 1. Profits & Losses by Region and Sub-Category  
![Profits & Losses](data_analysis_tripleten/super_store_profitability_analysis/profits_losses.png.png)  
**Insight:**  
Copiers drive ~$76K profit, while Furniture categories like Tables (-$23K) drag margins. The West and East dominate profitability, while Central struggles with persistent losses.  

---

### 2. Bottom Products (Top Loss-Makers)  
![Bottom Products](data_analysis_tripleten/super_store_profitability_analysis/bottom_products.png.png)  
**Insight:**  
The **GBC DocuBind System** alone loses over -$20K. Several high-cost items (e.g., CubeX 3D printer) show both low sales and high returns → prime candidates for discontinuation.  

---

### 3. Top Products (Profit Leaders)  
![Top Products](data_analysis_tripleten/super_store_profitability_analysis/top_products.png.png)  
**Insight:**  
The **Canon ImageCLASS** product generated $38K profit — the single largest contributor. Other products like Ativa V41 ($12K) show solid returns and should be prioritized in stock & promotions.  

---

### 4. Returns by Customer  
![Returns by Customer](data_analysis_tripleten/super_store_profitability_analysis/returns_by_customer.png.png)  
**Insight:**  
A small group of customers (10 accounts) return **90–100% of their purchases**, destroying margins. These accounts should be flagged for return policy enforcement or account review.  

---

### 5. Returns by Product  
![Returns by Product](data_analysis_tripleten/super_store_profitability_analysis/returns_by_product.png.png)  
**Insight:**  
Printers, phones, and furniture items dominate the highest return rates (100%). These are likely tied to vendor quality issues → renegotiation or supplier switch may be needed.  

---

### 6. Average Profit vs. Average Return Rate  
![Avg Profit vs Return](data_analysis_tripleten/super_store_profitability_analysis/avg_profit_vs_return.png.png)  
**Insight:**  
Copiers show **high profit despite moderate returns** (worth keeping). Machines & chairs show high returns with mixed profitability → require closer monitoring.  

---

### 7. State-Level Seasonality  
![State Seasonality](data_analysis_tripleten/super_store_profitability_analysis/state_seasonality.png.png)  
**Insight:**  
Seasonality strongly affects state performance:  
- **Indiana (Oct: $643)**, **Vermont (Nov: $596)**, **Washington (Dec: $521)** show peak profit months.  
- Seasonal campaigns & stock allocation should target these cycles.  

---

## 🧠 Conclusion & Recommendations  

1. **Double Down on High-Value Products**  
   - Prioritize Copiers and Canon ImageCLASS, ensure availability, and use promotions.  

2. **Address Loss-Makers**  
   - Discontinue or renegotiate terms for underperformers like Tables (-$23K) and GBC DocuBind (-$20K).  

3. **Tackle Returns Head-On**  
   - Investigate chronic returners (customers & products at 90–100% return rates).  
   - Tighten policies and improve supplier contracts.  

4. **Leverage Regional & Seasonal Insights**  
   - Run campaigns during peak state-months (Indiana, Vermont, Washington).  
   - Replicate strong-state strategies in weaker markets.  

---

## 🛠 Tools Used  
- Tableau Public (Data Visualization)  
- GitHub (Project Versioning & Portfolio Hosting)  

🚀 Final project submission for the **Data Visualization with Tableau** sprint at **TripleTen**.  
