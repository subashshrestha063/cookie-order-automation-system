# 🍪 ByteBake: End-to-End Cookie Order Automation System

![Make.com](https://img.shields.io/badge/Platform-Make.com-purple?style=flat&logo=make)
![Google Sheets](https://img.shields.io/badge/Database-Google%20Sheets-green?style=flat&logo=google-sheets)
![Discord](https://img.shields.io/badge/Notifications-Discord-5865F2?style=flat&logo=discord)
![Status](https://img.shields.io/badge/Project-Completed-success)

> A production-style business automation project built using **Make.com** to manage
orders, inventory, SLA monitoring, notifications, and daily sales reporting for a
fictional bakery called **ByteBake Cookies**.

This project focuses on **automation logic, system design, and real operational
constraints**, rather than UI or frontend development.

---

## 📖 Overview

**ByteBake Cookies** is a fictional bakery, but the operational challenges it faces
are very real:

- Orders arriving without stock validation
- Inventory running out unexpectedly
- Delays during baking and delivery stages
- No clear SLA monitoring or escalation
- Manual sales reporting at the end of the day

This project solves those problems using a **modular, no-code automation system**
that simulates how a real bakery could operate using modern automation tools.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|-----|--------|
| **Make.com** | Core automation platform orchestrating all workflows |
| **Google Sheets** | Structured data backend for orders, inventory, and reporting |
| **Discord** | Internal notifications (low stock, SLA breaches, alerts) |
| **Gmail** | Customer and internal email notifications |
| **Make Data Stores** | Temporary storage for aggregation and state tracking |

---

## ⚙️ System Architecture

The system is divided into **6 independent but connected automation scenarios**.
Each scenario handles one clear business responsibility, making the system easier
to debug, extend, and maintain.

| ID | Scenario | Description |
|----|---------|-------------|
| **Scenario 1** | Order Intake & Stock Validation | Accepts orders, validates inventory, updates stock |
| **Scenario 2** | Low-Stock Monitoring & Restock Alerts | Monitors inventory and sends alerts when stock is low |
| **Scenario 3** | Order Lifecycle Status & Notifications | Tracks order status changes and sends notifications |
| **Scenario 4** | SLA Monitoring & Escalation | Detects delayed orders and escalates issues |
| **Scenario 5** | SLA Recovery & De-escalation | Handles recovery when delayed orders are resolved |
| **Scenario 6** | Daily Sales Summary & Analytics | Generates daily sales analytics and summaries |

Each scenario is documented individually in the [`/scenarios`](scenarios/) folder.

---

## 📊 Data Design (Google Sheets)

The automation uses Google Sheets as a structured data backend.

### Core Sheets
- **Orders** – Order details, status, timestamps, SLA tracking
- **Inventory** – Cookie stock levels and restock thresholds
- **Daily Cookie Sales** – Cookie-wise sales logs
- **Daily Summary** – Aggregated daily metrics for reporting

---

## 🚀 How to Run 

This project is built on **Make.com**.

To explore or replicate the automation:

1. Open Make.com and create a new scenario.
2. Import the JSON blueprint from the [`/blueprints`](blueprints/) folder.
3. Create Google Sheets using the structure described above.
4. Reconnect your own Google, Gmail, and Discord accounts.

> ⚠️ **Note:**  
> Blueprints are provided for learning and reference.  
> Minor adjustments may be required depending on your account setup.

---

## ✨ Key Features

- Automated order intake with stock validation
- Inventory updates and low-stock alerts
- Order lifecycle tracking:
  - New → Baking → Packed → Out for Delivery → Delivered / Cancelled
- Time-based SLA monitoring and escalation
- SLA recovery workflow
- Daily sales summary including:
  - Total orders
  - Total quantity sold
  - Cookie-wise sales
  - Top-selling cookie

---

## 🧠 Learnings & Challenges

- Designing modular automations instead of one large workflow
- Working around **router limitations** in Make.com
- Preventing duplicate notifications using state tracking
- Implementing **time-based SLA logic**
- Using **Make Data Stores** for aggregation and temporary state
- Structuring Google Sheets for automation-friendly data flow

---

## 📁 Repository Structure

```text
├── README.md
├── scenarios/
│   ├── scenario-1.md
│   ├── scenario-2.md
│   ├── scenario-3.md
│   ├── scenario-4.md
│   ├── scenario-5.md
│   └── scenario-6.md
├── screenshots/
│   ├── scenario-1/
│   ├── scenario-2/
│   ├── scenario-3/
│   ├── scenario-4/
│   ├── scenario-5/
│   └── scenario-6/
└── blueprints/
    ├── scenario-1.json
    ├── scenario-2.json
    ├── scenario-3.json
    ├── scenario-4.json
    ├── scenario-5.json
    └── scenario-6.json

```
## 📝 Notes 

This project was built as a hands-on automation exercise to simulate real operational challenges.  
Implementation details are intentionally abstracted to focus on system design and logic.

---

## 👤 Author
**Subash Shrestha**  
Automation & Workflow Design (Make)

⭐ If you find this project interesting, explore the individual scenarios in the [scenarios](scenarios/).

---

