# Scenario 3 – Order Lifecycle Status & Notification Automation

## Purpose
This scenario manages the complete order lifecycle by tracking status changes and sending automated notifications to both customers and internal teams. It ensures visibility, consistency, and timely communication throughout the fulfillment process.

## Trigger
- Order status update in Google Sheets

## Logic Overview
Order records are continuously monitored for lifecycle status changes.

- The scenario detects when an order status changes (e.g., New → Baking → Packed → Out for Delivery → Delivered → Cancelled).
- Notifications are sent only when the current status differs from the **Last Notified Status**, preventing duplicate alerts.
- The **Last Status Update** timestamp is recorded whenever a valid status change occurs.
- Internal assignment (e.g., baker team or delivery team) is updated automatically based on the order status.
- Inventory is restocked in case of cancellation.

### Scenario Design 
<img src="/screenshots/scenario-3/flow_scenario-3.png" width="500">



## Output
- Automated customer email notifications for order status updates
- Internal Discord notifications for operational awareness
- Accurate tracking of order progression and lifecycle history

## Platform & Components
- Google Sheets (order data and lifecycle tracking)
- Make.com (status detection, routing logic, and updates)
- Discord (internal notifications)
- Gmail (customer notifications)
