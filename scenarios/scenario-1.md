# Scenario 1 – Order Intake & Stock Validation

## Purpose
This scenario handles incoming customer orders and validates stock availability before confirming the order.

## Trigger
- Google Form submission (customer order)

## Logic Overview
1. Receive order data from Google Forms
2. Search inventory data in Google Sheets
3. Validate available quantity against ordered quantity
4. Route logic:
   - If stock is sufficient → update inventory and mark order as **New**
   - If stock is insufficient → mark order as **Out of Stock**

### Scenario Design
<img src="/screenshots/scenario-1/flow_scenario-1.png" width="700">

## Output
- Inventory sheet updated
- Order status recorded
- Data passed to downstream scenarios

## Tools Used
- Google Forms
- Google Sheets
- Make.com Router & Filters
