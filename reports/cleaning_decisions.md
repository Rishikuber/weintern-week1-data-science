# Data Cleaning Summary

- Raw rows: 662
- Exact duplicate rows detected and removed: 12
- Cleaned rows: 650
- Rows flagged for review: 27

## Decisions
- Preserve the raw CSV unchanged.
- Remove exact duplicate rows only.
- Normalize category and delivery status capitalization.
- Fill missing Customer ID, Payment Mode, and City with `Unknown`.
- Set non-positive Quantity and Unit Price to missing rather than inventing values.
- Recalculate Total Amount as Quantity × Unit Price.
- Mark rows with missing Quantity, Unit Price, or Order Date as `Review`.
- Exclude invalid numeric/date records and Cancelled/Returned statuses from headline sales KPIs.
