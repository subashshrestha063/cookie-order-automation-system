# Scenario 1 – Order Intake & Stock Validation

## Purpose
This scenario handles incoming customer orders and validates stock availability before confirming the order.

## Trigger
- Google Form submission (customer order)
  
- Check Out Google form -> <a href ="https://docs.google.com/forms/d/e/1FAIpQLScenub56d-j8SAo0cDMgr9QiCL40jPqC15KA1zTOJMCX5YNNg/viewform?usp=header">Order ByteBake Cookies</a>

## Logic Overview
1. Receive order data from Google Forms
2. Search inventory data in Google Sheets
3. Validate available quantity against ordered quantity
4. Route logic:
   - If stock is sufficient → update inventory and mark order as **New**
   - If stock is insufficient → mark order as **Out of Stock**

### Scenario Design
<img src="/screenshots/scenario-1/flow_scenario-1.png" width="850">

## Output
- Inventory sheet updated
- Order status recorded
- Data passed to downstream scenarios

### Discord Notification-Stock Available
<img src="/screenshots/scenario-1/order_stock_available_discord.png" width="600">


### Discord Notification-Stock Unavailable
![Discord Stock Unavailable Alert](/screenshots/scenario-1/order_stock_unavailable_discord.png)

## Tools Used
- Google Forms
- Google Sheets
- Make.com Router & Filters


