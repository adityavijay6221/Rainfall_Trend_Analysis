# 🌧️ Rainfall Analysis & Agricultural Impact | AWS S3, Snowflake, Power BI

## 📌 Project Overview
This project implements an end-to-end **data analytics pipeline** to analyze rainfall patterns and their relationship with agricultural variables such as crop yield, area cultivated, humidity, and seasonality.

The workflow includes:
- Data ingestion using **Amazon S3**
- Data warehousing and transformation using **Snowflake SQL**
- Interactive visualization using **Power BI**

---

## 🎯 Problem Statement
Rainfall is a critical factor influencing agricultural productivity and crop planning.  
However, rainfall patterns vary significantly across **locations, seasons, and years**, making it difficult to draw actionable insights without centralized analysis.

**This project aims to:**
- Analyze rainfall distribution across regions and seasons
- Identify rainfall-intensive locations
- Understand seasonal rainfall consistency
- Enable data-driven agricultural planning using BI dashboards

---

## 🗂️ Data Architecture & Flow
1. CSV data uploaded to **Amazon S3**
2. Data loaded from S3 into **Snowflake**
3. Data transformation and aggregation using **Snowflake SQL**
4. Snowflake connected to **Power BI**
5. Interactive rainfall analytics dashboard created

---

## 📊 Dataset Overview
**Source:** `data_season.csv`

**Key Fields Analyzed**
- Year  
- Location  
- Rainfall  
- Season (Kharif, Rabi, Zaid)  
- Temperature  
- Humidity  
- Area cultivated  
- Crop type  
- Yield  
- Soil type  
- Irrigation method  

---

## 🔍 Data Analysis Steps

### 1. Data Ingestion
- CSV file stored in **Amazon S3**
- External stage created in Snowflake
- Data loaded into Snowflake tables

### 2. Data Transformation (Snowflake SQL)
- Standardized column formats
- Removed inconsistencies in categorical fields
- Aggregated rainfall by:
  - Location
  - Season
  - Year
- Prepared analytical tables for BI consumption

### 3. Data Visualization (Power BI)
- Connected Power BI directly to Snowflake
- Built interactive visuals with filters for:
  - Location
  - Season
  - Year
- Created KPIs and comparative charts for rainfall analysis

---

## 📈 Key Insights from the Analysis

### 🌍 Location-Wise Rainfall
- **Bangalore** records the **highest average rainfall** among all locations in the dataset.
- Other high-rainfall regions include **Raichur, Kasaragodu, Mangalore, and Chikmangaluru**.
- Coastal and southern regions consistently receive higher rainfall than inland regions.

### 🌾 Seasonal Rainfall Patterns
- Rainfall levels are **relatively consistent across seasons**:
  - **Rabi** season shows the highest average rainfall
  - **Kharif** closely follows
  - **Zaid** records slightly lower rainfall
- Seasonal variation exists but is less significant than regional variation.

### 📅 Year-Wise Stability
- Rainfall values remain **stable across years** for most locations.
- No extreme year-over-year volatility observed in average rainfall trends.

### 🌡️ Climatic Correlation
- High rainfall regions also show **moderate temperatures and humidity levels**, indicating favorable agricultural conditions.
- Yield variation appears more dependent on **area cultivated and crop type** than rainfall alone.

---

## 💼 Business & Analytical Value
- Supports **agricultural planning** by identifying high-rainfall regions
- Helps policymakers assess **regional climate consistency**
- Enables **seasonal crop selection strategies**
- Demonstrates scalable cloud-based BI architecture using AWS + Snowflake

---

## 🛠️ Tools & Technologies
- **Amazon S3** – Data storage  
- **Snowflake** – Data warehousing & SQL transformation  
- **Power BI** – Dashboarding & visualization  

---


