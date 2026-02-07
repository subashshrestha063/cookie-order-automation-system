# Cookie-Order-Automation-System
An end-to-end business automation system built using **Make.com** to manage cookie orders, inventory, alerts, SLA monitoring, and daily sales insights for a fictional bakery called **ByteBake Cookies**.

This project demonstrates real-world workflow automation, system design, and operational thinking using no-code tools.

## Overview
This project is an end-to-end automation system designed to manage cookie orders,
inventory, SLA monitoring, notifications, and daily sales summaries using
Make (Integromat), Google Sheets, Discord, and Gmail.

The system simulates a real bakery workflow with production stages,
time-based SLAs, escalation handling, and reporting.

This automation system solves those problems by:
- Validating stock at order intake
- Automatically updating inventory
- Monitoring low stock and triggering alerts
- Tracking order lifecycle and SLAs
- Escalating delayed orders
- Recovering SLA breaches
- Generating daily sales summaries

The entire system is modular, scalable, and designed as a real business workflow.

##  Tools Used
- Make (Integromat)
- Google Sheets
- Discord (Notifications)
- Gmail (Customer & Internal Emails)



---
##  System Architecture

The automation is divided into **6 independent but connected scenarios**, each responsible for a specific business function.

| Scenario | Description |
|--------|------------|
| Scenario 1 | Order Intake & Stock Validation |
| Scenario 2 | Low-Stock Monitoring & Restock Alerts |
| Scenario 3 | Order Lifecycle Status & Notifications |
| Scenario 4 | SLA (Time-in-Status) Monitoring & Escalation |
| Scenario 5 | SLA Recovery and De-Esclation Automation |
| Scenario 6 | Daily Cookie Sold Summary |

Each scenario is documented individually inside the `/scenarios` folder.


---
##  Key Features

- Automated order validation
- Inventory update with stock checks
- Discord alerts for low stock
- Order status tracking (New,Baking,Packed,Out for Delivery, Delivered, Out of Stock)
- SLA monitoring and escalation
- SLA recovery workflow
- Daily sales summary:
  - Total orders
  - Total quantity sold
  - Cookie-wise sales
  - Top-selling cookie

---
## 📄 Data Design (Google Sheets)
- Orders Sheet
- Inventory Sheet
- Daily Cookie Sales Sheet
- Daily Summary Sheet

---

## 🎯 Key Learnings
- Designing multiple automations
- Handling time-based SLAs
- Preventing duplicate notifications
- Working around router limitations in Make
- Using Data Stores for aggregation

---


## 👤 Author
**Subash Shrestha**  
Automation & Workflow Design (Make)

⭐ If you find this project interesting, feel free to explore the scenarios and documentation.
