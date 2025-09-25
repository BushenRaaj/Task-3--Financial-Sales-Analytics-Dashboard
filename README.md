# 📊 Financial & Sales Analytics – Power BI Dashboard

## 📌 Project Overview
This project is part of **Task 3: Dashboard Design** from the Data Analyst Internship.  
Using the **Financial_Dataset.xlsx**, I developed an **interactive and visually engaging Power BI dashboard** to help business stakeholders track and analyze key financial metrics.  

The dashboard transforms raw financial data into **actionable insights** by focusing on:  
- 💰 **Sales & Profit performance** across multiple years  
- 📦 **Product-wise profitability and contribution**  
- 🌍 **Country-level sales analysis** using map visualization  
- 🏷️ **Segment-based and discount band analysis**  
- 📈 **Trends over time** to monitor business growth  

---

## 📂 Repository Structure
- [Financial & Sales Analytics Dashboard.pbix](Financial%20&%20Sales%20Analytics%20Dashboard.pbix) → Power BI dashboard file  
- [data/Financial_Dataset.xlsx](data/Financial_Dataset.xlsx) → Raw dataset  
- [images/Preview of Financial & Sales Analytics Dashboard.png](images/Preview%20of%20Financial%20&%20Sales%20Analytics%20Dashboard.png) → Dashboard preview  
- [README.md](README.md) → Documentation  

---

## ⚙️ Steps Followed to Build the Dashboard

### 1. Data Loading
- Imported **Financial_Dataset.xlsx** into **Power BI Desktop**.  
- Verified column data types (Sales, Profit, Units Sold, Discounts, Date, etc.).  

### 2. Data Transformation
- Cleaned column names (e.g., fixed `" Sales"` → `Sales`).  
- Ensured **Date** was properly set to datetime format.  

### 3. Measures Created
Defined **DAX measures** for KPIs:
```DAX
Total Sales = SUM(Financial[Sales])
Total Profit = SUM(Financial[Profit])
Total Units Sold = SUM(Financial[Units Sold])
Profit Margin % = DIVIDE([Total Profit], [Total Sales], 0)
```

## 🖼️ Dashboard Layout

**Top Section (KPI Cards):**  
Displays **Total Sales, Profit, Profit Margin %, and Units Sold** → quick performance snapshot.  

**Middle Section (Trends & Geography):**  
- 📈 **Line Chart:** Tracks Sales & Profit over time.  
- 🌍 **Map Visualization:** Shows Sales by Country.  

**Right Section (Distribution):**  
- 🍩 **Donut Chart:** Sales distribution across Discount Bands.  

**Bottom Section (Details by Category):**  
- 📊 **Stacked Column Chart:** Sales by Segment (Government, Midmarket, etc.).  
- 📦 **Bar Chart:** Top Products by Profit.  

**Filters (Slicers):**  
Interactive filters for **Year, Country, and Segment**.  

---

## 📊 Final Dashboard Preview
*(Insert your dashboard preview image here)*

---

## 📝 Key Learnings
- Building KPIs and custom measures with **DAX**.  
- Using **cards, line charts, maps, and donut charts** for storytelling.  
- Applying **slicers/filters** to enhance interactivity.  
- Designing dashboards that enable **data-driven decision-making**.  

---

## ❓ Interview Questions Related to This Task  

### 1. What are the key elements of a dashboard?  
- **KPIs (cards):** Show overall metrics like Sales, Profit, Units Sold.  
- **Charts/Visuals:** Line charts, bar charts, maps to show comparisons.  
- **Filters/Slicers:** Enable interactive exploration.  
- **Layout & Design:** Clear, consistent, and easy to interpret.  

### 2. What is a KPI?  
A **Key Performance Indicator** is a measurable value showing how well a business is achieving objectives.  
- Example: **Total Sales, Total Profit, Profit Margin %, Units Sold**.  

### 3. What are slicers in Power BI?  
- **Interactive filters** that let users control displayed data.  
- Example: Filter by **Year, Country, or Segment**.  

### 4. Difference between Power BI and Tableau?  
- **Power BI:** Microsoft ecosystem, easier for beginners, cost-effective.  
- **Tableau:** More advanced customization, better with very large datasets, preferred for complex analytics.  

### 5. How do you make a dashboard interactive?  
- Add **slicers, filters, drill-throughs, and tooltips**.  
- Ensure visuals are interconnected for dynamic updates.  

### 6. How do you deal with large datasets in dashboards?  
- Import only required fields.  
- Use **aggregations and summary tables**.  
- Optimize DAX and relationships.  
- Use **DirectQuery mode** for huge datasets.  

### 7. What chart types do you use for trend analysis?  
- **Line Chart** → Sales/Profit over time.  
- **Area Chart** → Emphasize cumulative growth.  
- **Combo Chart** → Compare metrics like Sales vs Profit.  
