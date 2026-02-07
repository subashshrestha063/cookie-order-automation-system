# Scenario 6 – Daily Cookie Sold Summary & Sales Insights

## Purpose
This scenario generates a daily summary of cookie sales to provide clear visibility into sales performance and demand patterns.

## Trigger
- Scheduled execution (end-of-day summary)

## Logic Overview
Order data from the day is evaluated and aggregated to produce key sales metrics.

- Quantities sold are grouped by cookie type.
- Overall order volume is calculated.
- Top-performing items are identified based on total quantity sold.
- The summary is designed to be informational and non-intrusive.

## Output
- Daily sales summary delivered to internal channels and email to manager
- Visibility into best-selling items
- Total quantity sold and total order count

## Platform & Components
- Google Sheets (order data)
- Make.com (aggregation and summary logic)
- Discord (daily summary delivery)
