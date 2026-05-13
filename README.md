# AdventureWorks Business Intelligence Report
### Power BI | Business Analytics | Data Modelling

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)
![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

---

## 📌 Project Background

AdventureWorks is a global manufacturing company specialising in cycling equipment and accessories. As the newly appointed Business Intelligence Analyst, I was tasked by the management team to build a reporting solution from scratch using only raw CSV data files.

The business had no existing dashboards or reporting infrastructure. My objective was to design and deliver a fully interactive Power BI report that would give leadership a clear, real-time view of business performance.

---

## 🎯 Business Objectives

The management team needed answers to four core questions:

| Business Question | Report Page |
|---|---|
| How are we performing against KPI targets (sales, revenue, profit, returns)? | Exec Dashboard |
| Which regions and territories are driving the most orders? | Map |
| Which products are trending, and how do they perform vs targets? | Product Detail |
| Who are our highest-value customers, and how are they segmented? | Customer Detail |

---

## 📂 Data Sources

All analysis was built from raw CSV files provided by the business — no pre-built database or data warehouse was available.

| File | Description |
|---|---|
| Sales Data | Transaction-level order records |
| Returns Data | Product return records |
| Products Lookup | Product names, categories, subcategories, pricing |
| Customers Lookup | Customer demographics and profile data |
| Territory Lookup | Regional and country-level territory mapping |
| Calendar Lookup | Date table for time intelligence |

---

## 🛠️ Tools & Skills Used

- **Power BI Desktop** — Report design, data modelling, visualisation
- **Power Query (M)** — Data cleaning, transformation, and shaping of raw CSV files
- **DAX** — Calculated columns, measures, KPIs, time intelligence, what-if parameters
- **Data Modelling** — Star schema design with fact and dimension tables
- **Conditional Formatting** — Dynamic colour-coded performance indicators

---

## 📊 Report Pages

### 1. Executive Dashboard
High-level KPI summary for leadership — the single-page view that answers: *"How is the business performing right now?"*

- **$24.9M** total revenue | **$10.5M** profit | **25.2K** orders | **2.2%** return rate
- Revenue trending line chart (Jan 2020 – Jan 2022) with growth trajectory
- Orders by product category — Accessories (17K), Bikes (13.9K), Clothing (7K)
- Top 10 Products table with conditional formatting flagging elevated return rates
- Month-on-month KPI cards with variance vs prior month

### 2. Map
Geographic performance view — *"Where in the world are our orders coming from?"*

- Bubble map visualising order volume across 6 countries
- Markets covered: United States, Canada, United Kingdom, France, Germany, Australia
- Continent-level filter buttons: Europe / North America / Pacific

### 3. Product Detail
Drilldown page for product-level analysis — *"How is each product tracking vs its target?"*

- KPI gauge charts: Orders, Revenue, and Profit vs monthly target
- What-if price adjustment parameter (interactive price sensitivity slider)
- Switchable metric trend chart (toggle between Revenue, Profit, Orders, Returns)
- Per-product filtering for granular investigation

### 4. Customer Detail
Customer segmentation and value analysis — *"Who are our best customers and what do they look like?"*

- **17,416** unique customers | **$1,431** average revenue per customer
- Revenue per customer trending chart
- Top 100 customers ranked by revenue with orders and revenue columns
- Orders by income level and occupation (donut charts)
- Mr. Maurice Shan identified as top customer: 6 orders, $12,408 revenue

---

## 🔍 Key Insights

- Revenue grew consistently from Jan 2020 to Jan 2022, with the steepest growth in H2 2021
- Accessories drive the highest order volume (17K) but Bikes generate the most revenue per unit
- Sport-100 Helmet (Red) has the highest return rate at 3.33% — a potential quality flag for the product team
- The majority of high-value customers are in the Professional occupation bracket with high income levels
- North America accounts for the largest share of geographic order volume

---

## 📁 Project Structure

```
adventureworks-bi-report/
│
├── data/
│   ├── AdventureWorks Sales Data 2020
│   ├── AdventureWorks Sales Data 2021
│   ├── AdventureWorks Sales Data 2022
│   ├── AdventureWorks Returns_data.csv
│   ├── AdventureWorks Products_lookup.csv
|   ├── AdventureWorks Product Categories Lookup
|   ├── AdventureWorks Product Subcategories Lookup
│   ├── AdventureWorks Customers_lookup.csv
│   ├── AdventureWorks Territory_lookup.csv
│   └── AdventureWorks Calendar_lookup.csv
├── images/
│   ├── customer_detail.png
│   ├── map.png
│   ├── product_detail.png
│   └── exec_dashboard.png
├── AdventureWorks Report.pbix     # Main Power BI report file
├──LICENSE
└── README.md
```

---

## 🚀 How to Use

1. Clone or download this repository
2. Open `AdventureWorks Report.pbix` in Power BI Desktop (free download from Microsoft)
3. If prompted, update the CSV file paths under **Transform Data → Data Source Settings**
4. Explore all 4 report pages using the tab navigation at the bottom

---

## 👤 Author

**Brendon Mbizvo**
Data Scientist | Business Analytics & BI
📧 brendonmbizvo@gmail.com
🔗 [LinkedIn](https://linkedin.com/in/brendonmbizvo) | [GitHub](https://github.com/Mbizvo)

---

*Built as part of a Business Intelligence portfolio project. Dataset based on the AdventureWorks sample database.*
