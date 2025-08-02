# Usage Guide

This document explains how to interact with the Sales Performance Dashboard and get the most value from it.

## Opening the Dashboard
1. Open `Sales_Performance_Dashboard.xlsx` (or `Week4_Faith_Mwende.xlsx`) in Microsoft Excel (2016 or later recommended for best compatibility).  
2. Navigate to the **Dashboard** sheet to view key visual summaries.

## Exploring the Dashboard
- **Filters / Slicers**: Use the interactive slicers to filter by:
  - Date range (Month, Year, or combined period)
  - Region / State / City
  - Product Category or Sub-Category
  - Customer Segment
  - Order Priority
- Adjusting these will dynamically update all related charts and summary metrics.

## Key Sections to Review
- **Total Sales Summary**: Overview of revenue, units sold, and average sale.  
- **Sales by Region**: Compare performance across different geographic regions to identify strong and weak areas.  
- **Top Products**: See which products are driving the most revenue or volume.  
- **Temporal Trends**: Analyze monthly or weekday sales patterns to spot seasonality or anomalies.

## Updating the Data
1. Replace or refresh the raw source data in the `Cleaned Data` (or source) sheet.  
2. If any transformations or new data were added:
   - Ensure the calculated fields (e.g., discounts, time extraction) are refreshed or re-applied.  
   - Refresh all pivot tables: Right-click on any pivot table and choose **Refresh**, or use the Data ribbon's refresh options.  
3. Verify that slicers and relationships reflect the updated dataset.

## Common Questions Answered
- Which region generated the highest revenue last quarter?  
- What are the top 5 products by sales volume?  
- Are certain customer segments purchasing more during specific months?  
- How do discounts affect net sales over time?

## Best Practices
- Always work on a copy of the dashboard if experimenting with structure or adding new metrics.  
- Keep a separate `raw_data.csv` or `raw_data.xlsx` file untouched as the canonical source; use the cleaned/calculated sheets for analysis.  
- Document any custom filters or assumptions you apply when sharing insights.

## Troubleshooting
- **Charts not updating**: Refresh pivot tables and ensure the slicers are connected.  
- **Missing data**: Check that new records were added to the source sheet and that date formats are consistent.  
- **Errors in calculated metrics**: Confirm that base fields (e.g., Unit Price, Quantity, Discount) are present and numeric.


