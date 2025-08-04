Task 1: Data Cleaning & Preprocessing – SuperStore Sales

Objective
Clean and prepare the raw SuperStore Sales dataset: handle missing values, standardize formats, remove duplicates, and ensure consistent types.

What was done
- Normalized and cleaned column headers (lowercase, no spaces).
- Parsed and standardized date fields (`order_date`, `ship_date`).
- Created `shipping_days` and imputed missing values with median.
- Reconstructed missing dates when possible.
- Derived `return_flag` from raw returns data.
- Trimmed and imputed categorical/text columns using mode.
- Ensured numeric columns (`sales`, `profit`, etc.) are numeric and filled missing with median.
- Flagged shipping anomalies (`ship_before_order`, `long_delay`).
- Removed duplicate rows.
- Added `cleaned_timestamp` for audit.
- Saved cleaned output as `superstore_sales_cleaned.csv`.

Tools
- Python 3.x
- pandas

How to run
```bash
python clean_superstore.py  # or run the provided notebook cell
