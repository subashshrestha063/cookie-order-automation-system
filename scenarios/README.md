## 📊 Scenarios Summary
---

### Scenario 1 – Order Intake & Stock Validation
---
- Take new order and add to google sheets
- Validates stock 
- Updates inventory automatically
- Prevents out-of-stock fulfillment

  For Detailed Documentaion Vist - [Scenario 1 – Order Intake & Stock Validation](scenario-1.md)
  
  
### Scenario 2 – Low-Stock Monitoring & Restock Alert
---
- Monitors inventory thresholds
- Sends Discord alerts for low stock

  For Detailed Documentaion Vist - [Scenario 2 – Low-Stock Monitoring & Restock Alert Automation](scenario-2.md)
  
  
### Scenario 3 – Order Lifecycle Status & Notification Automation
---
- Tracks order status changes (New → Baking → Packed → Out for Delivery → Delivered / Cancelled)
- Sends customer & internal notifications
- Updates timestamps and last notified status

For Detailed Documentaion Vist - [Scenario 3 – Order Lifecycle Status & Notification Automation](scenario-3.md)

  
### Scenario 4 – Order SLA (Time-in-Status) Monitoring & Escalation
---
- Tracks time spent in each status
- SLA levels (0 → 1 → 2 → 3 → 4)
- Notifies teams when delays occur

For Detailed Documentaion Vist - [Scenario 4 – SLA Monitoring & Escalation](scenario-4.md)


### Scenario 5 – SLA Recovery
---
- Resets SLA level when order progresses
- Prevents repeated false escalations

For Detailed Documentaion Vist - [Scenario 5 – SLA Recovery and De-Esclation](scenario-5.md)

  
### Scenario 6 – Daily Cookie Sold Summary
---
- Aggregates daily sales data
- Calculates:
  - Total orders
  - Total quantity sold
  - Cookie of the day
  - Total revenue
- Sends daily summary to Discord and Gmail
- Writes structured summary to Google Sheets

For Detailed Documentaion Vist - [Scenario 6 – Daily Cookie Sold Summary](scenario-6.md)
