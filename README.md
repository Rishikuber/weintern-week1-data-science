# Data Science Internship — Week 1 Assignment

**Author:** Rishi Kuber  
**Organization:** WeIntern Pvt Ltd  
**Environment:** Python, pandas, NumPy, Matplotlib, Jupyter Notebook

## Project objective
Demonstrate e-commerce data cleaning, sales KPI analysis, customer insights, and business-focused visualizations.

## Dataset
`data/raw/ecommerce_sales_raw.csv` is a **synthetic educational dataset created for this project**. It intentionally contains missing values, duplicate rows, inconsistent capitalization, and invalid quantity/price values. It is not real business data.

## Tasks completed
- **Task 1:** Dataset inspection, missing-value report, duplicate analysis, validation, documented cleaning decisions, cleaned CSV.
- **Task 2:** Total revenue, total orders, average order value, units sold, top category, top revenue-generating product, monthly trends, city and repeat-customer insights.
- **Task 3:** Category revenue bar chart, monthly sales line chart, payment-mode pie chart, dashboard mockup.

## Folder structure
```text
data-science-week1-assignment/
├── data/
│   ├── raw/ecommerce_sales_raw.csv
│   └── cleaned/ecommerce_sales_cleaned.csv
├── notebooks/week1_analysis.ipynb
├── outputs/
│   ├── charts/
│   ├── dashboard/
│   ├── kpi_summary.csv
│   └── missing_value_report.csv
├── reports/final_report.pdf
├── screenshots/
├── README.md
└── requirements.txt
```

## Run the notebook
1. Install Python 3 and Anaconda, or use an existing Jupyter environment.
2. Open Anaconda Navigator and launch Jupyter Notebook.
3. Open `notebooks/week1_analysis.ipynb`.
4. Run cells from top to bottom. If running from the notebook folder, the notebook detects the project root automatically.

Install dependencies:
```bash
pip install -r requirements.txt
```

## KPI definition
For the report, sales KPIs exclude records with invalid quantity, unit price, or order date, and exclude `Cancelled` and `Returned` statuses. Total orders are counted as distinct Order IDs. Average Order Value = filtered revenue / distinct valid orders.

## Limitations
The dataset is synthetic; insights are illustrative and should not be presented as findings from a real company. Missing identifiers are marked `Unknown`; invalid quantities/prices are flagged instead of guessed. Total Amount is recalculated from Quantity × Unit Price.

## Submission checklist
- [ ] Run notebook from top to bottom and verify no errors.
- [ ] Review report and confirm that all observations match the latest notebook outputs.
- [ ] Add screenshots if requested by the internship.
- [ ] Push repository to GitHub and paste the repository URL into the internship submission form.
