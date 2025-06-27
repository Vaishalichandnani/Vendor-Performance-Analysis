# Vendor Performance Analysis

## Objective

To analyze vendor-wise sales, profitability, and inventory performance for a retail business, and help management take data-driven actions related to vendor selection, purchasing, promotions, and inventory clearance.

---

## Tools Used

- **Python**: Data ingestion, cleaning, transformation, and statistical analysis
- **SQLite**: Lightweight relational database for structured raw data storage
- **Pandas, NumPy, SQLAlchemy, SciPy**: Data manipulation, aggregation, and hypothesis testing
- **Jupyter Notebook**: For step-by-step exploratory data analysis
- **Power BI**: Interactive dashboard for visualizing vendor performance
- **Excel**: Cleaned file exported for Power BI use

---

## Project Structure

'''text
Vendor-Performance-Analysis/
│
├── data/
│   ├── vendor_sales_summary.csv             # Cleaned CSV used in Python
│   └── vendor_sales_summary_clean.xlsx      # Excel version used in Power BI
│
├── scripts/
│   ├── ingestion_db.py                      # Loads raw CSVs into SQLite
│   └── get_vendor_summary.py                # Generates final summary dataset
│
├── notebooks/
│   ├── Exploratory Data Analysis.ipynb      # Initial profiling, outlier checks
│   └── Vendor Performance Analysis.ipynb    # Final feature engineering & insights
│
├── dashboard/
│   └── vendor_performance.pbix              # Power BI interactive dashboard
│
├── report/
│   └── Vendor Performance Report.pdf        # PDF report with written insights
│
├── requirements.txt                         # Python dependencies
└── README.md                                # Project documentation
'''

---

## Key KPIs Computed

- **Total Purchase Cost**
- **Total Sales Revenue**
- **Gross Profit** and **Profit Margin %**
- **Unsold Inventory Capital**
- **Stock Turnover**
- **Sales-to-Purchase Ratio**
- **Vendor & Brand-level Rankings**

---

## Key Insights

- **Top 10 vendors** make up ~66% of purchases — potential over-dependency.
- **$2.7M in unsold inventory** — ties up working capital.
- **High-margin, low-volume brands** — should be prioritized for promotion.
- **Bulk purchase discounts** — significantly reduce unit costs.
- **Statistical validation** confirms meaningful margin differences across vendor segments.

All insights are backed by data and visualized in Power BI for stakeholder use.

---

## Dashboard Preview

> The dashboard includes:
- KPI cards for quick performance view
- Top and Bottom vendors & brands
- Sales vs Profit Margin scatterplot
- Unsold capital & inventory inefficiencies
- Filters for vendor, brand, and category

Open the '.pbix' file in Power BI Desktop:  
'dashboard/vendor_performance.pbix'

---

## How to Run

1. Place your raw CSVs into the '/data/' folder.
2. Run 'scripts/ingestion_db.py' to load them into a local SQLite database.
3. Run 'scripts/get_vendor_summary.py' to generate the cleaned summary dataset.
4. Use 'vendor_sales_summary_clean.xlsx' as input for the Power BI dashboard.
5. Explore the notebooks or the final PDF report for analysis insights.

---

## Deliverables

- Cleaned CSV and Excel datasets
- Python scripts (ingestion, summary creation)
- Exploratory & final analysis notebooks
- Interactive Power BI dashboard
- Business report PDF
- Complete documentation (this README)

---
