# 🧠 RetailAnalytics-DWBI

This project is a complete **Data Warehouse and Business Intelligence** (DWBI) solution, completed as part of Year 3 Semester 1 coursework for the DWBI module.

---

## 🧠 Project Overview

This project demonstrates a full end-to-end Business Intelligence (BI) workflow using a **Snowflake Schema** for a **Retail Sales** scenario. The pipeline includes:

- ⚙️ Data Warehouse design and implementation (via SSMS)
- 📊 OLAP Cube creation (via Visual Studio/SSAS)
- 📝 SSRS Reports
- 📈 Power BI Dashboards
- 📁 Excel-based OLAP operations

---

## 🗂️ Folder Structure

| Folder                        | Description                                                       |
|------------------------------|-------------------------------------------------------------------|
| `Assig1_DWBI_CUBE/`          | SSAS cube files including dimensions, measures, and deployment scripts |
| `DW_BusinessIntelligenceAssignment/` | SQL and SSMS scripts for schema creation and data population       |
| `Reports/`                   | Project overview, planning documents, and report summaries        |
| `powerBI/`                   | Power BI dashboards with slicers, drill-downs, and insights       |
| `ExcelDemo/`                 | Excel PivotTables demonstrating OLAP operations                   |

---

## 🧱 Data Warehouse Schema

The data warehouse is modeled using a **Snowflake Schema** with the following structure:

### 🔸 Fact Table
- `Factcustomer_orders`

### 🔹 Dimension Tables
- `Dimbrands`
- `Dimproduct_inventory`
- `Dimlocations`
- `Dimcustomers` (with SCD implementation)

---

## ➕ Slowly Changing Dimension (SCD)

The `Dimcustomers` table implements **Type 2 SCD** to track historical changes in:

- `address`
- `city`
- `state`
- `zipcode`
- `country`

With additional metadata fields:

- `StartDate`
- `EndDate`
- `IsCurrent`

This allows for accurate **time-based analysis** on customer location changes.

---

## 🔍 Key Features

- 💽 ETL process implemented using T-SQL + SSMS
- 📦 OLAP cube with key measures:
  - `order_qty`
  - `order_total`
  - `processing_time`
- 🧪 Excel-based OLAP operations (slice, dice, drill-down, roll-up)
- 📈 Power BI Dashboards:
  - Matrix visualizations
  - Slicers & drill-through
  - Hierarchical drill-downs
- 📝 SSRS Reports for operational and strategic business analysis

---

## 🚀 Tools & Technologies

- Microsoft SQL Server Management Studio (SSMS)
- SQL Server Analysis Services (SSAS)
- SQL Server Reporting Services (SSRS)
- Microsoft Power BI
- Microsoft Excel

---

## 📌 Author Notes

This project was completed as part of my university coursework on **Data Warehousing & Business Intelligence**. It showcases skills in:

- Dimensional Modeling  
- ETL & SCD Implementation  
- OLAP Cube Development  
- Dashboard & Report Building

---

Feel free to explore each folder and its components. Contributions, feedback, and suggestions are welcome!

