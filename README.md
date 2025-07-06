# <img width="152" height="152" alt="Image" src="https://github.com/user-attachments/assets/2d56995e-6b20-4ac1-b2ae-3f75b51c0fe4" />Business Insight 360
## Project Overview
AtliQ Hardware is growing rapidly in the recent years, and they have decided to implement the data analytics using PowerBi in their company for the first time to surpass their competitors in the market and to make data driven decisions. This project is hoped to give answers to the questions of stakeholder in terms all the aspects like finance, sales, marketing and supply chain.

This repository presents a comprehensive data analytics solution designed for **AtliQ Hardware**, a rapidly growing global hardware company. The project, developed using **Power BI**, empowers stakeholders to make informed decisions across various departments — **Sales, Finance, Marketing, Supply Chain, and Executive Management**.

Inspired by the [Codebasics Power BI Course](https://www.codebasics.io), this project integrates best practices in data modeling, dashboard development, DAX optimization, and Power BI service deployment.

> 📌 **Live Dashboard Link**: [Insert link to Power BI service report here]  
> 📁 **Course Link**: [Codebasics Power BI Course](https://www.codebasics.io)

---

## 🏢 Company Background

**AtliQ Hardware** is a multinational enterprise specializing in computers and accessories. It operates globally through:
- **Retailers**
- **Direct Sales**
- **Distributors**

Due to a costly misstep in opening a store in the U.S. without sufficient data backing, AtliQ has committed to building a **robust analytics capability**. This project is their **first Power BI implementation** to enable data-driven decision-making and stay competitive in the global market.

---

## 🎯 Project Objectives

- Deliver a 360-degree view of the business operations.
- Enable cross-functional insights across Finance, Sales, Marketing, and Supply Chain.
- Support executive leadership with KPIs and drill-down analysis.
- Implement scalable, refreshable Power BI dashboards.

---

## 🧠 Questions Asked Before Development

As part of the project kickoff, we addressed key discovery questions:

- What is the primary objective of the dashboard?
- Who are the intended users and their roles?
- What are the stakeholders' expectations and fears?
- What data is available, and what’s missing?
- What constitutes success for this project?
- Are preview sessions expected before release?
- What design inputs or brand guidelines should be followed?

---

## 🗃️ Dataset Overview

Data was imported from **MySQL** using Power BI’s native connectors. The data is stored in a **Snowflake Schema**, divided into dimension and fact tables across two schemas: `gdb041` and `gdb056`.

### 🔹 Dimension Tables

| Table | Description |
|-------|-------------|
| `dim_customer` | Customer details including platforms and sales channels |
| `dim_market` | Market geography data (Regions, Zones, Markets) |
| `dim_product` | Product divisions and categories |

### 🔸 Fact Tables

| Table | Description |
|-------|-------------|
| `fact_sales_monthly` | Monthly sales volume per customer/product/market |
| `fact_forecast_monthly` | Forecasted demand quantities |
| `gross_price` | Product-level gross prices |
| `freight_cost` | Logistics cost per market per fiscal year |
| `manufacturing_cost` | Production cost by product and year |
| `pre_invoice_deductions` | Promotional/discount deductions before invoicing |
| `post_invoice_deductions` | Return/discount deductions after invoicing |

> 🧾 **Note**: The forecasting and sales tables are denormalized to simplify analytics.

---

## 🧱 Data Modeling Approach

A well-designed **data model** was built following **best practices**:

- **Snowflake Schema** for efficiency and clarity
- Properly configured **relationships** between dimension and fact tables
- Created a **Date Table** using Power Query (M Language)
- Optimized calculated columns and measures using **DAX Studio**
<img width="1454" height="1041" alt="Image" src="https://github.com/user-attachments/assets/4799c5e6-b9a5-40b1-a31e-bda95e7be29e" />

---

## 🛠️ Tech Stack & Tools

| Tool | Purpose |
|------|---------|
| **Power BI Desktop** | Report building and visualization |
| **SQL / MySQL** | Data querying and import |
| **DAX** | Calculated measures and KPIs |
| **Power Query (M Language)** | Data transformation |
| **DAX Studio** | Performance optimization |
| **Excel** | Data validation and pre-processing |
| **Power BI Service** | Publishing, collaboration, gateway setup |
| **GitHub + LFS** | Version control and large file tracking |

---

## 📈 Power BI Concepts Applied

- Calculated columns and measures using **DAX**
- Field formatting and dynamic visual interactivity
- Conditional formatting using icons and colors
- Bookmarks and page navigation with buttons
- KPI indicators with modern visuals
- Data validation using cross-sheet references
- Dynamic titles responding to filters
- Handling division errors using `DIVIDE` function
- Using slicers for hierarchical filtering

---

## 📁 Folder Structure

Business-Insight-360/
│
├── AtliQ_Hardware_Report.pbix
├── README.md
├── /screenshots
│ ├── home_view.png
│ ├── finance_dashboard.png
│ ├── sales_dashboard.png
│ ├── marketing_dashboard.png
│ ├── supply_chain_dashboard.png
│ ├── executive_summary.png
├── /data (optional)
│ └── sample_tables.csv
├── .gitignore
└── LICENSE

yaml
Copy
Edit

---

## 💼 Departmental Dashboards

### 🏠 Home Page
- Central navigation panel using buttons
- Easy access to all department dashboards

### 💰 Finance View
- Gross Price vs Net Sales
- Gross Margin % (GM%), COGS
- YTD and YTG metrics

### 🛒 Sales View
- Sales vs Forecast Variance
- Top Customers by Volume
- Performance by Channel (Retail, Direct, Distributor)

### 📣 Marketing View
- Campaign ROI (if available)
- Pre- and Post-Invoice Deduction Analysis
- Price Elasticity Trends

### 🚚 Supply Chain View
- Freight Costs by Market
- Logistics Trends
- Forecast Accuracy

### 🧑‍💼 Executive View
- Aggregated KPIs from all departments
- High-level trends and drill-downs

> 🎥 *Short Demo Videos Available*  
> Add links or embed `.mp4` preview files for stakeholders.

---

## 🧾 Key Business Terms & Definitions

| Term | Definition |
|------|------------|
| **COGS** | Cost of Goods Sold |
| **Gross Price** | Price before any deductions |
| **Pre-/Post-Invoice Deductions** | Discounts and returns applied to sales |
| **Net Sales** | Revenue after all deductions |
| **Net Profit** | Final profit after expenses |
| **YTD / YTG** | Year-to-Date / Year-to-Go Sales |
| **Forecast Quantity** | Expected customer demand (fact table) |

---

## 🚀 Project Outcome

With the implementation of this analytics solution:

- Business leaders can make **data-driven decisions** across functions.
- Stakeholders can identify **underperforming markets or products** early.
- Historical data analysis and **forecasting accuracy** improved.
- Enables real-time collaboration using **Power BI Service** and **Power BI App**.

---

## 🌐 Power BI Service Deployment

- Reports published to **Power BI Workspace**
- Configured **Personal Gateway** for automatic refresh
- Created **Power BI App** for secure stakeholder access
- Managed user roles, access levels, and refresh schedules

---

## 🧑‍💻 Author

**Purushottam Mitra**  
📧 [pmitra620@gmail.com]  
🔗 [LinkedIn]([https://www.linkedin.com/in/pmitra620/])  
📂 [Portfolio](https://yourportfolio.com)

---

## 📝 License

This project is licensed under the **MIT License**. See the [LICENSE](./LICENSE) file for details.

---

## ⭐ Support

If you found this project useful:

- 🌟 Star the repository
- 🖖 Connect on LinkedIn
- 🍴 Fork and build your own version

---

## 🙏 Acknowledgements

- Codebasics Power BI Course
- Power BI Community Forum
- SQLBI DAX Reference
- GitHub LFS for large file handling
