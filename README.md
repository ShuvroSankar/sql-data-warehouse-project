# Data Warehouse and Analytics Project

Welcome to the **Data Warehouse and Analytics Project** repository!  
This project presents a complete **data warehousing and analytics solution** — from building a PostgreSQL-based data warehouse to generating actionable business insights.  

Designed as a **portfolio project**, it demonstrates industry best practices in **data engineering**, **data modeling**, and **SQL-based analytics**.

---

## Project Requirements

### Data Engineering — Building the Data Warehouse

#### Objective
Develop a modern **data warehouse** using **PostgreSQL** to consolidate sales data and enable analytical reporting for better business decisions.

#### Specifications
- **Data Sources**: Import data from two systems — **ERP** and **CRM** — provided as CSV files.  
- **Data Quality**: Clean and standardize the data to resolve quality issues before loading.  
- **Integration**: Combine both sources into a unified, analysis-ready data model optimized for queries.  
- **Scope**: Focus on the **latest dataset** only (no historization required).  
- **Documentation**: Provide clear documentation of the data model for business and analytics users.

---

## BI: Analytics & Reporting (Data Analytics)

#### Objective
Develop **SQL-based analytics** to generate insights on:  
- **Customer Behavior**  
- **Product Performance**  
- **Sales Trends**  

These insights empower stakeholders with **key business metrics** to support **strategic decision-making**.

---

## Project Structure

```
DataWarehouse-Analytics/
│
├── /data/                # Raw CSV files (ERP, CRM)
├── /scripts/             # SQL scripts for ETL and schema creation
│   ├── create_database.sql
│   ├── staging_load.sql
│   └── analytics_queries.sql
├── /documentation/       # Data model diagrams and metadata
├── /reports/             # BI queries, dashboards, and visualizations
└── README.md             # Project overview
```

---

## Tech Stack

| Layer | Technology |
|-------|-------------|
| Database | PostgreSQL |
| ETL & Modeling | SQL |
| Data Visualization | Power BI / Tableau |
| Data Sources | CSV files (ERP & CRM) |
| Version Control | Git & GitHub |

---

## How to Run the Project

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/DataWarehouse-Analytics.git
   cd DataWarehouse-Analytics
   ```

2. **Create the database and schemas**
   ```sql
   \i scripts/create_database.sql
   ```

   This script:
   - Drops the existing `DataWarehouse` database (if it exists)
   - Creates a new `DataWarehouse` database
   - Defines the three schema layers:
     - `bronze` — raw data ingestion layer  
     - `silver` — cleaned and transformed data  
     - `gold` — aggregated and analytics-ready layer

3. **Load source data**
   - Place ERP and CRM CSV files in the `/data/` folder.
   - Run ETL SQL scripts to load and clean the data into the warehouse.

4. **Run analytics queries**
   - Execute the SQL queries in `/scripts/analytics_queries.sql` to explore business insights.

---

## Example Insights

- Top 10 customers by revenue  
- Product categories with declining sales  
- Monthly sales growth trends  
- Customer retention and churn indicators  

---

## Author

**Shuvro Sankar Sen**  
📧 [sankarshuvro1010@gmail.com]  
🔗 [https://www.linkedin.com/in/shuvro-sankar-048b5118b/]

---
