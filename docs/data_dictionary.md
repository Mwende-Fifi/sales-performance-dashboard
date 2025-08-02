# Data Dictionary

This document defines the key fields and metrics used in the Sales Performance Dashboard. Data originates from the raw sales transactions, is cleaned, enriched with calculated metrics, and then surfaced via pivot tables and the dashboard.

## Source Sheets
- **Sheet 1**: Raw transactional data (original import).  
- **Cleaned Data**: Normalized version of the raw data with consistent field formatting.  
- **Calculated Metrics**: Enriched data with derived fields (e.g., discounts, time breakdowns) used to drive analysis.

## Core Fields

### Identifiers & Reference
- **Order ID**: Unique identifier for each sales order/transaction.  
- **Customer ID**: Unique identifier for each customer.  
- **Customer Name**: Human-readable name of the customer.  
- **Product Name**: Name of the product sold.  
- **Product Sub-Category / Category**: Hierarchical grouping of products for segmentation.

### Sales & Pricing
- **Unit Price**: Price per single unit of product before quantity.  
- **Quantity ordered**: Number of units included in the order.  
- **Total Sales (Before Discount)**: Calculated as `Unit Price * Quantity ordered`.  
- **Discount %**: Percentage discount applied to the order.  
- **Discount Amount**: Absolute value deducted from sales due to the discount.  
- **Total Sales (After Discount)**: Net sales after applying discount.  

### Customer & Order Attributes
- **Customer Segment**: Segment classification (e.g., Corporate, Home Office) used for segmentation.  
- **Order Priority**: Priority level assigned to the order (e.g., High, Critical, Not Specified).  
- **Ship Mode**: Shipping method used (e.g., Standard, Express).

### Geographic
- **Region**: Broad region (e.g., East, West) used for geographic breakdown.  
- **State or Province**: Sub-region within the broader region.  
- **City**: City associated with the order (likely shipping or customer location).

### Temporal / Time Breakdown (from Calculated Metrics)
- **Order Date**: Date when the order was placed.  
- **Ship Date**: Date when the order was shipped.  
- **Month**: Month extracted from `Order Date` (e.g., January).  
- **Year**: Year extracted from `Order Date`.  
- **Month and Year**: Combined period label (e.g., "June 2015").  
- **Week Day**: Day of week of the order (e.g., Monday).

## Derived Insights
- **Sales Trends**: Time series of sales to understand seasonality or growth.  
- **Top Products**: Products sorted by revenue or quantity sold.  
- **Regional Performance**: Comparison of revenue across regions/states/cities.  
- **Customer Segmentation Performance**: Sales aggregated by customer segment.

## Notes
- All monetary values are assumed to be in the same currency and are derived consistently from unit price, quantity, and discount logic.  
- Time-based fields are extracted from the `Order Date` to support trend analysis and filtering.

