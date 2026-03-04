# Data Warehouse & Analytics Pipeline

A end-to-end data warehousing and analytics solution built to consolidate, transform, and surface insights from raw sales data — following **Medallion Architecture** across Bronze, Silver, and Gold layers.

---

## 🏗️ Architecture

![Data Architecture](docs/data_architecture.png)

| Layer | Purpose |
|---|---|
| **Bronze** | Raw ingestion — CSV files loaded as-is into SQL Server |
| **Silver** | Cleansing, standardization, and normalization |
| **Gold** | Business-ready star schema optimized for analytical queries |

---

## 📖 What This Project Covers

- **Data Warehouse Design** — Medallion architecture with clear layer separation
- **ETL Pipelines** — Extracting from ERP & CRM source systems, transforming, and loading
- **Data Modeling** — Fact and dimension tables in a star schema
- **Analytics & Reporting** — SQL-based dashboards covering sales trends, customer behavior, and product performance

---

## 🛠️ Tech Stack

- **Database:** SQL Server Express
- **GUI:** SQL Server Management Studio (SSMS)
- **Diagramming:** Draw.io
- **Version Control:** Git / GitHub

---

## 📂 Repository Structure

```
data-warehouse-project/
│
├── datasets/                    # Raw ERP and CRM source data (CSV)
│
├── docs/                        # Architecture diagrams and documentation
│   ├── data_architecture.drawio
│   ├── data_flow.drawio
│   ├── data_models.drawio
│   ├── etl.drawio
│   ├── data_catalog.md
│   └── naming-conventions.md
│
├── scripts/                     # SQL scripts per layer
│   ├── bronze/                  # Raw data extraction & loading
│   ├── silver/                  # Cleansing & transformation
│   └── gold/                    # Analytical models & star schema
│
├── tests/                       # Data quality checks
├── README.md
└── requirements.txt
```

---

## 🚀 Getting Started

1. Install [SQL Server Express](https://www.microsoft.com/en-us/sql-server/sql-server-downloads) and [SSMS](https://learn.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms)
2. Clone the repository and load CSVs from `/datasets`
3. Run scripts in order: `bronze/` → `silver/` → `gold/`
4. Query the Gold layer views for analytics

---

## 📊 Analytics Covered

- **Customer Behavior** — segmentation, retention, purchase patterns
- **Product Performance** — revenue by category, top/bottom performers
- **Sales Trends** — monthly/quarterly breakdowns, growth metrics

For full requirements, see [`docs/requirements.md`](docs/requirements.md).

---

## 🛡️ License

Licensed under the [MIT License](LICENSE).
