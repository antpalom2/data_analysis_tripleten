# 🏙️ Manhattan Vacation Rental Market Analysis

## 📌 Project Overview

This project analyzes Airbnb listings in Manhattan to help a client determine the most attractive neighborhoods and property sizes for investment in the vacation rental market. The analysis is based on Airbnb open data and includes insights into rental popularity and revenue potential.

**Sprint 1 — Spreadsheet Data Analysis**  
Conducted as part of TripleTen’s Data Analytics program.

📄 [View Full Project Spreadsheet](https://docs.google.com/spreadsheets/d/1GqIG4HPlfzu_2T8SJvossuLtErgViuUOdrMulZeVoYI/edit?gid=442099053#gid=442099053)

---

## 🗂️ Dataset

The dataset includes property listings and calendar availability scraped from Airbnb public data.

📊 [Access the Raw Dataset](https://docs.google.com/spreadsheets/d/1qdnGCyf_eMhtXXvbPIc8wnz3WIlllL2GnlYvVBlufx8/copy)

Key fields include:
- `neighborhood`, `room_type`, `bedrooms`, `price`, and `review_count`  
- Calendar data with nightly pricing and availability  
- Cleaned using `PROPER()`, `TRIM()`, and conditional logic

---

## 🔍 Key Questions Answered

1. Which neighborhoods and property sizes are most attractive for vacation rentals?  
2. How much revenue did these listings generate?

---

## 🧼 Data Cleaning Steps

Performed in Excel:
- Standardized `neighborhood` names using `TRIM()` and `PROPER()` → stored in `neighborhood_clean`  
- Cleaned `bedrooms` column using `IF(ISBLANK(...), 0, ...)` → stored in `bedrooms_clean`  
- Created a `top_listing` column where:
  - `top_neighborhood` is `TRUE`
  - `top_bedroom` is `TRUE`  
- Revenue calculation:
  - `IF(available = "f", adjusted_price, 0)` → `revenue_earned`
  - `SUMIF()` matched revenue by `listing_id`
  - Estimated annual revenue = 30-day revenue × 12

---

## 📊 Analysis Highlights

- **Top Neighborhoods** by review count (used as a proxy for rental activity)  
- **Most Common Property Sizes:** 1-bedroom units dominate, with studios more popular in Midtown  
- **Top Listings** chosen from the most active neighborhoods with highest-earning unit types

| Listing | Estimated Annual Revenue |
|---------|---------------------------|
| ID 1    | $359,280                  |
| ID 2    | $313,200                  |
| ...     | ...                       |

---

## 📈 Visualizations

### 1. Top 10 Most Popular Neighborhoods by Number of Reviews  
![Top 10 Neighborhoods](visualizations/most_popular_neighborhoods.png)  
**Insight:**  
Lower East Side, Hells Kitchen, and Harlem are the most reviewed neighborhoods, suggesting high rental traffic.

---

### 2. Property Sizes by Neighborhood (Pivot Table)  
![Bedrooms by Neighborhood](visualizations/most_popular_by_bedroom_spaces.png)  
**Insight:**  
1-bedroom listings are most common in most areas, but Midtown favors studios — likely due to apartment layouts and short-stay guests.

---

## 🧠 Assumptions

- `review_count` is used as a proxy for demand  
- 30-day revenue × 12 is a reasonable annual estimate  
- `top_listing` is based on top neighborhoods and most frequent bedroom count

---

## 🛠️ Tools Used

- Excel (Data Cleaning & Calculations)  
- Tableau Public (Data Visualization)  
- GitHub (Project Versioning & Documentation)

---

🚀 Project submission for the Spreadsheet Data Analysis sprint (TripleTen BI Program).
