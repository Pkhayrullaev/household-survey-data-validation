# Household Food Consumption Survey - Data Validation Pipeline

Python (pandas) pipeline that validates a large multi-sheet household survey
and flags inconsistent records for manual review.

## What it does
- Splits survey items by unit of measurement (kg, g, litre, piece, etc.)
- Runs 9 automated checks per record: zero prices, unit-price outliers (IQR per
  product), quantity outliers, duplicates, suspiciously round values,
  fractional quantities for whole-unit items, implausible quantities, missing values
- Exports flagged records for review and splits confirmed errors by region
  for follow-up with field teams

## Tech
Python, pandas, NumPy, openpyxl

## Notes
Survey data is confidential and not included in this repository.