# Sales-Data-Analysis


## Project Description  
This Power BI project presents an interactive dashboard for analyzing sales data across multiple dimensions. It is designed to provide business users with deep insights into product performance, 
profitability, sales patterns, discounting strategies, and geographic performance. The dashboard was built to answer eight targeted business questions using intuitive, filterable visuals.

---

## Business Questions & Dashboard Features

### 1. **Top/Bottom 5 Products by Sales, Profit, Quantity Sold**
- Three sets of bar charts identify the top and bottom 5 products based on:
  - Total Sales Revenue
  - Total Profit Earned
  - Total Quantity Sold
- Helps decision-makers focus on bestsellers and poorly performing items.
- Implemented using **Top N filters** in visual level filters with dynamic sorting.

---

### 2. **Sales Trends Over Time (Daily, Monthly, Quarterly, Annually)**
- Line charts visualize how sales evolve:
  - Day-to-day (for granular trend spotting)
  - Month-to-month and quarter-to-quarter (for performance comparison)
  - Yearly summaries (to observe long-term growth or decline)
- Built using a **calendar table** with hierarchical date fields and time intelligence DAX.

---

### 3. **Relationship Between Sales and Profit**
- A scatter plot displays:
  - Each product as a data point
  - Sales on X-axis and Profit on Y-axis
  - Bubble size represents Quantity Sold
- Identifies which products are both high revenue and high profit.
- Reveals low-margin or loss-making high-sellers.

---

### 4. **Compare Sales/Profit/Quantity Between Two Periods**
- Users can select **two custom date ranges** using slicers.
- Visuals (bar/column charts or KPI cards) compare:
  - Total Sales
  - Total Profit
  - Total Quantity
- Useful for period-over-period or campaign performance analysis.
- Achieved using DAX measures with `CALCULATE` and `FILTER`.

---

### 5. **Average Discount Offered in Each Discount Category**
- Discounts are grouped into categories (e.g., 0–10%, 10–20%, etc.)
- Bar chart or table shows average discount per category.
- Assesses whether deeper discounts result in more sales or just reduce profit.
- Implemented using **calculated columns** for bins and `AVERAGE` DAX.

---

### 6. **Total Number of Orders**
- A single KPI card displays the total number of unique orders.
- Simple but essential metric for volume tracking.
- Calculated using `DISTINCTCOUNT(Sales[Order ID])`.

---

### 7. **Detailed Order View With Interactive Filters**
- A table visual includes:
  - Order ID, Date, Product, Sales, Profit, Quantity, Discount, Net Sales
- Supports filtering using slicers:
  - Product Name
  - Order Date
  - Customer ID
  - Promotion Categories
- Enables granular investigation into individual transactions.

---

### 8. **Sales by Different Cities**
- Map or bar chart visualizes total sales across cities.
- Identifies strong and weak markets geographically.
- Enhances regional performance analysis for targeting.

---

## Tools & Techniques Used
- **Power BI Desktop** for report development  
- **DAX Measures** for time intelligence, period comparison, and custom aggregations  
- **Calculated Columns** for discount categorization and date-based logic  
- **Interactive Visuals & Slicers** for user-driven exploration  
- **Top N and dynamic filters** for highlighting key data points  
- **Date Table** for proper time-based analysis and drill-down capability  

---

## Outcome  
This dashboard enables sales managers, marketing teams, and operations analysts to:
- Make data-backed decisions
- Identify high-impact products and regions
- Evaluate promotional performance
- Monitor business growth over time

---

*Created by Kanwal Zulfiqar  
*June 2025*
