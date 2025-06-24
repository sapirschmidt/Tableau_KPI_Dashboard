# Tableau_KPI_Dashboard
I developed an interactive KPI dashboard in Tableau to monitor key performance indicators across different categories and time periods. The dashboard enables clear visualization of performance trends and supports informed decision-making by stakeholders.

# KPI Dashboard – Beverage Sales Performance (2020-2025)

Interactive **Tableau** workbook that tracks the commercial performance of a multi-brand beverage portfolio across the United States.  
The dashboard condenses revenue, profit, unit-sales and cost-of-goods metrics into one view so that executives, product managers and sales leaders can spot trends, drill into outliers and compare performance by customer, product, company and state.

---

## 🗺️  Business Questions Answered

| Theme                | Key questions built into the dashboard                                                                         |
|----------------------|----------------------------------------------------------------------------------------------------------------|
| **Growth over time** | *How have revenue, profit, units sold and COGS evolved quarter-by-quarter since 2020?*                         |
| **Customer value**   | *Which customers deliver the most (or least) revenue?*  *How concentrated is the customer base?*               |
| **Product mix**      | *Which SKUs and categories drive the lion’s share of sales?*  *Where do margins lag?*                          |
| **Geographical reach** | *Which U.S. states generate the highest revenue and profit?*                                                 |
| **Supplier / brand** | *How do partner companies (Coca-Cola, Nestlé, Pepsico, etc.) compare on sales and margin KPIs?*                |

---

## 📊  What You’ll See on the Dashboard

| Section (worksheet) | Visual | Details & Interactivity |
|---------------------|--------|-------------------------|
| **KPI Tiles**       | BANs   | Real-time totals for Revenue, Profit, Units Sold, COGS (respect current filters) |
| **Revenue By Year** | Line   | Trend of the selected metric; hover to see exact quarterly values |
| **Revenue By State**| Filled Map | Choropleth of chosen metric; click a state to filter cross-charts |
| **Revenue By Customer** | Horizontal bar | Top customers ranked by metric; bar length and labels update dynamically |
| **Revenue By Product**  | Horizontal bar | Top products or SKUs ranked by metric; scroll for full list |
| **Global Filters**  | | • Time range slider (2020 Q1 → 2025 Q4)  <br>• Metric radio buttons (Revenue / Profit / Units Sold / COGS) <br>• Company multi-select <br>• Category multi-select |

---

## 🏗️  Tech Stack

| Layer          | Technology / File | Notes |
|----------------|-------------------|-------|
| **Data**       | `Beverages_Made_dataset.xlsx` | 12,000 + transactional rows of U.S. beverage sales (2020-2025) |
| **Prep**       | Tableau Desktop 2024.1  | Minor data-type fixes & calculated fields for KPIs |
| **Viz**        | `KPI Dashboard.twb` | One workbook, five core worksheets, one dashboard tab |
| **Optional**   | Tableau Server / Tableau Public | Publish `.twb` or `.twbx` for shared, live access |

---

## 🚀  Getting Started Locally

1. **Clone** the repository  
   ```bash
   git clone https://github.com/<your-org>/beverage-kpi-dashboard.git
   cd beverage-kpi-dashboard
Open KPI Dashboard.twb in Tableau Desktop.

When prompted for a data source, point Tableau to data/Beverages_Made_dataset.xlsx (or accept the packaged extract if you saved one).

Use the left-hand filters or click any mark to explore the data interactively.

Want to publish? Save as .twbx and upload to Tableau Public or your organisation’s Tableau Server.

📂 Repo Layout
kotlin
Copy
Edit
├── data/
│   └── Beverages_Made_dataset.xlsx   # Raw transaction data
├── KPI Dashboard.twb                 # Tableau workbook
└── README.md                         # Project documentation (this file)
🤝 Contributing
Bug reports, feature requests and pull requests are welcome.
For major changes (e.g. new KPIs, alternate data sources) please open an issue first so we can discuss scope and design.
