# Scenario 2 – Low-Stock Monitoring & Restock Alert Automation

## Purpose
This scenario continuously monitors inventory levels and alerts the team when stock falls below a defined threshold, helping prevent fulfillment delays.

## Trigger
- Scheduled execution (periodic inventory check)

## Logic Overview
Inventory records are evaluated against minimum stock thresholds.

- Items below the threshold are identified as low-stock.
- Alerts are generated only once per low-stock event to avoid notification spam.
- The scenario is designed to work independently of order intake.

### Scenario Overview
<img src="/screenshots/scenario-2/flow_scenario-2.png" width="850">

## Output
- Low-stock alerts sent to internal communication channels
- Visibility into items requiring restocking
- Supports proactive inventory management

## Tools Used
- Google Sheets (inventory data)
- Make.com (scheduled checks and conditional logic)
- Discord (internal alerts)
