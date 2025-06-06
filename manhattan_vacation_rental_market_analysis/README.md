
# 🏙️ Manhattan Vacation Rental Market Analysis

## 📌 Project Overview

This project analyzes Airbnb listings in Manhattan to help a client determine the most attractive neighborhoods and property sizes for investment in the vacation rental market. The analysis is based on Airbnb open data and includes insights into rental popularity and revenue potential.

**Sprint 1 — Spreadsheet Data Analysis**  
Conducted as part of TripleTen’s Data Analytics program.

---

## 🗂️ Dataset

- **Listings data:** Includes property information, reviews, pricing, and more.
- **Calendar data:** Shows nightly availability and pricing.
- Source: [Inside Airbnb NYC Data](http://insideairbnb.com/get-the-data.html)

---

## 🔍 Key Questions Answered

1. **Which neighborhoods and property sizes are most attractive for vacation rentals?**
2. **How much revenue did these listings generate?**

---

## 🧼 Data Cleaning Steps

Performed in Excel:
- Standardized `neighborhood` names using `TRIM()` and `PROPER()` → stored in `neighborhood_clean`
- Cleaned `bedrooms` column using `IF(ISBLANK(...), 0, ...)` → stored in `bedrooms_clean`
- Created a new `top_listing` column where:
  - `top_neighborhood` is `TRUE`
  - `top_bedroom` is `TRUE`
- Calculated revenue from calendar data using:
  - `IF(available = "f", adjusted_price, 0)` → `revenue_earned`
  - Used `SUMIF()` to match calendar revenue to listings
  - Estimated annual revenue = 30-day revenue × 12

---

## 📊 Analysis Highlights

- **Top 10 Neighborhoods** by number of reviews (proxy for rental frequency)
- **Most Popular Property Sizes:** 1-bedrooms dominate, except Midtown (studios)
- **Top Listings** selected based on:
  - Top 10 neighborhoods
  - Most common bedroom type in each

| Listing | Estimated Annual Revenue |
|---------|---------------------------|
| ID 1    | $359,280                  |
| ID 2    | $313,200                  |
| ...     | ...                       |

---

## 📈 Visualizations

### 1. Top 10 Most Popular Neighborhoods by Number of Reviews  
![Top 10 Neighborhoods](visualizations/top_10_neighborhoods_reviews.png)  
**Insight:**  
Lower East Side, Hells Kitchen, and Harlem are the most reviewed neighborhoods, suggesting strong rental demand.

---

### 2. Property Sizes by Neighborhood (Pivot Table)  
![Bedrooms by Neighborhood](visualizations/bedrooms_by_neighborhood.png)  
**Insight:**  
1-bedroom rentals are the most common across neighborhoods, but Midtown and East Harlem show unusually high numbers of studio apartments.

---

## 💡 Future Improvements

- Automate the analysis in Python or SQL
- Incorporate occupancy rates
- Compare seasonal trends
- Normalize review counts by listing age

---

## 🧪 How to Reproduce

1. Open the Excel file:
   - Sheets: `Processed Listings`, `Calendar`, `Top Listings`
2. Follow formulas and pivot tables to trace logic
3. (Optional) Use Python to replicate calculations

---

## 📎 File Structure

```
/manhattan-vacation-rental-analysis
├── data/
│   └── airbnb_listings.xlsx
├── visualizations/
│   ├── top_10_neighborhoods_reviews.png
│   └── bedrooms_by_neighborhood.png
└── README.md
```

---

## 🎓 About

This project was completed as part of the [TripleTen](https://tripleten.com/) Data Analytics Program.  
It demonstrates applied spreadsheet analytics, data storytelling, and business insights.
