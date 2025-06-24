
# 🚕 Zuber Ride-Sharing Analysis

This project analyzes ride-sharing activity for **Zuber**, a fictional taxi company in Chicago. The dataset contains trip, weather, and company information used to investigate business patterns, ride volume, and customer behavior under various conditions.

🗃️ **Project Focus:**  
Explore key metrics using SQL to understand trip volume by company, weather-based ride behavior, and airport routes.

---

## 📚 Skills & Techniques Applied

This project was completed as part of the **SQL Analysis Sprint** in TripleTen's Business Intelligence Analyst program.

### 🔍 SQL Techniques
- Filtering by time range with `CAST()` and `BETWEEN`
- Aggregating data with `COUNT()` and `GROUP BY`
- Using `CASE` statements for data segmentation
- Joining multiple tables via `JOIN`
- Applying conditions with `LIKE`, `IN`, `OR`
- Sorting with `ORDER BY`

---

## 🎯 Objective

To identify:
- Which taxi companies handle the most traffic
- The impact of weather on ride frequency and duration
- Passenger ride patterns from the Loop to O'Hare on rainy Saturdays

---

## 📊 Key Queries & Results

### 1. Trip Volume by Taxi Company (Nov 15–16, 2017)
```sql
SELECT
    cabs.company_name AS company_name,
    COUNT(trips.trip_id) AS trips_amount
FROM cabs
LEFT JOIN trips ON cabs.cab_id = trips.cab_id
WHERE CAST(start_ts AS date) BETWEEN '2017-11-15' AND '2017-11-16'
GROUP BY cabs.company_name
ORDER BY trips_amount DESC;
```

---

### 2. Trip Volume: Companies Containing "Yellow" or "Blue" (Nov 1–7, 2017)
```sql
SELECT
    cabs.company_name AS company_name,
    COUNT(trips.trip_id) AS trips_amount
FROM cabs
LEFT JOIN trips ON cabs.cab_id = trips.cab_id
WHERE CAST(start_ts AS date) BETWEEN '2017-11-01' AND '2017-11-07'
GROUP BY cabs.company_name
HAVING cabs.company_name LIKE '%Yellow%' OR cabs.company_name LIKE '%Blue%'
ORDER BY trips_amount DESC;
```

---

### 3. Rides by Flash Cab, Taxi Affiliation Services, and Others (Nov 1–7, 2017)
```sql
SELECT
    COUNT(trips.trip_id) AS trips_amount,
    CASE
        WHEN cabs.company_name IN ('Flash Cab', 'Taxi Affiliation Services') THEN cabs.company_name
        ELSE 'Other'
    END AS company
FROM cabs
LEFT JOIN trips ON cabs.cab_id = trips.cab_id
WHERE CAST(start_ts AS date) BETWEEN '2017-11-01' AND '2017-11-07'
GROUP BY company
ORDER BY trips_amount DESC;
```

---

### 4. Get Loop and O'Hare Neighborhood IDs
```sql
SELECT *
FROM neighborhoods
WHERE name = 'Loop' OR name LIKE '%Hare%';
```

---

### 5. Weather Conditions Grouped by Hour
```sql
SELECT
    ts,
    CASE
        WHEN description LIKE '%rain%' THEN 'Bad'
        WHEN description LIKE '%storm%' THEN 'Bad'
        ELSE 'Good'
    END AS weather_conditions
FROM weather_records;
```

---

### 6. Ride Duration from Loop to O’Hare on Rainy Saturdays
```sql
SELECT
    trips.start_ts,
    CASE
        WHEN weather_records.description LIKE '%rain%' THEN 'Bad'
        WHEN weather_records.description LIKE '%storm%' THEN 'Bad'
        ELSE 'Good'
    END AS weather_conditions,
    trips.duration_seconds
FROM trips
INNER JOIN weather_records ON weather_records.ts = trips.start_ts
WHERE pickup_location_id = 50
  AND dropoff_location_id = 63
  AND EXTRACT(ISODOW FROM weather_records.ts) = 6
ORDER BY trips.trip_id;
```

---

## 🧠 Insights & Business Implications

- **Flash Cab** and **Taxi Affiliation Services** dominate trip volumes.
- Weather conditions impact trip durations — rainy Saturdays may reduce speed and increase trip time.
- **Loop to O’Hare** is a frequent and important route for analysis.
- Additional segmentation (weather vs. clear) can inform staffing and vehicle deployment.

---

## 🛠 Tools Used

- PostgreSQL (SQL Queries & Data Retrieval)  
- TripleTen Platform (Project Execution)  
- GitHub (Version Control & Documentation)

---

🚀 *Project submission for SQL Analysis Sprint at TripleTen.*
