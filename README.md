# 📊 Exploring the Key Potential of Power BI – Analyzing the Sales Data (RFM Segmentation)

---

## 🚀 Project Overview
This project demonstrates how **Microsoft Power BI** can turn raw business data into actionable insights using **data modeling, DAX calculations, and interactive dashboards**.  
The analysis is based on **automotive sales data (2020–2022)** and focuses on exploring **sales performance, customer segmentation, product returns, and regional trends** through **RFM segmentation**.

---

## 🎯 Objectives
- Transform raw CSV data into a clean and analytical data model using **Power Query**  
- Build an **interactive Power BI dashboard** for executive-level reporting  
- Implement **DAX measures** to calculate KPIs like Revenue, Profit, Return Rate, and Growth %  
- Apply **RFM (Recency, Frequency, Monetary) segmentation** to classify customers  
- Explore **Power BI’s AI & UX features** such as Bookmarks, Drill-through, and Smart Narrative  
- Provide **data-driven recommendations** for improving business performance  

---

## 🧠 Dataset Information

| File Name | Description |
|------------|--------------|
| `Sales Data 2020.csv` | Sales transactions for 2020 |
| `Sales Data 2021.csv` | Sales transactions for 2021 |
| `Sales Data 2022.csv` | Sales transactions for 2022 |
| `Returns Data.csv` | Product return details |
| `Customer Lookup.csv` | Customer demographics |
| `Product Lookup.csv` | Product master data |
| `Territory Lookup.csv` | Regional data |
| `Calendar Lookup.csv` | Calendar table for time intelligence |

**Data Source:** [Kaggle – Global Bike Sales Dataset](https://www.kaggle.com/) *(or insert your dataset link)*

---

## ⚙️ Tools & Technologies
- **Power BI Desktop** – Data modeling, visualization & analysis  
- **Power Query Editor** – Data cleaning & transformation  
- **DAX (Data Analysis Expressions)** – Custom KPIs and measures  
- **Excel / CSV Files** – Data source  
- **Microsoft Power Platform** – Integration-ready BI environment  

---

## 🧩 Key Power BI Features Used
- **Data Modeling:** Star & Snowflake Schemas with Fact and Dimension Tables  
- **Dynamic Data Loading:** Folder connection for auto-refresh on new yearly files  
- **DAX Measures:** Total Revenue, Gross Profit, Return Rate, Time Intelligence (MoM %, YoY %)  
- **Bookmarks & Drill-Through:** Interactive navigation and deep-dive analytics  
- **AI Visuals:** Smart Narrative, Key Influencers, Decomposition Tree, Forecasting  
- **RFM Segmentation:** Customer grouping based on Recency, Frequency, and Monetary scores  

---

## 📈 Dashboard Insights
- **Total Net Sales:** €24.1M  
- **Profit Margin:** 42%  
- **Return Rate:** 2.2%  
- **Top Regions:** Europe & North America  
- **Top Categories:** Accessories & Bikes  
- **High Return Product:** Tires & Tubes (needs quality check)  
- **Customer Segments:** “Champions” and “Loyal Customers” are most profitable  

---

## 🧮 Sample DAX Measures

```DAX
-- Total Revenue
Total Revenue =
SUMX('Sales Data', 'Sales Data'[OrderQuantity] * RELATED('Product Lookup'[ProductPrice]))

-- Gross Profit
Gross Profit =
[Total Revenue] - [Total Cost]

-- Return Rate
Return Rate =
DIVIDE([Total Returned Quantity], [Total Order Quantity])

-- Revenue Growth %
Revenue % Change =
DIVIDE([Total Revenue] - [PM Revenue], [PM Revenue])
```

---

## 💡 Key Learnings
- Importance of **data modeling and relationships** for consistent analysis  
- Effective use of **DAX** to calculate advanced KPIs  
- Leveraging **Power BI AI visuals** to gain automated insights  
- Building **dynamic, user-friendly dashboards** with bookmarks & filters  

---

## 📎 Future Enhancements
- Integrate **real-time SAP or SQL data connections**  
- Add **Power BI Service reports** for automatic refresh and sharing  
- Use **AutoML models** for predictive sales forecasting  
- Extend RFM model using **Python or Power BI’s AI integration**

---

## 📘 Author

**👤 Saurab Barua**  
🎓 Master’s in Informatics & Business – FH Südwestfalen  
🔗 [LinkedIn Profile](https://www.linkedin.com/in/s-baru)  
📧 [saurab.barua@example.com](mailto:barua.saurab@fh-swf.de)

---

