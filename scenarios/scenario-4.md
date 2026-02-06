# Scenario 4 – SLA (Time-in-Status) Monitoring & Escalation Automation

## Purpose
This scenario monitors how long an order remains in a specific status and escalates alerts when defined SLA thresholds are breached. It helps identify delays early and ensures operational accountability.

## Trigger
- Scheduled execution (periodic SLA check)

## Logic Overview
Orders currently in active fulfillment states are evaluated against SLA thresholds.

- The scenario calculates **time-in-status** using the Last Status Update timestamp.
- SLA thresholds are defined in escalation tiers (e.g., 30 → 60 → 90 minutes).
- Each escalation level is triggered only once per status to prevent repeated alerts.
- Escalation logic progresses sequentially from Level 1 to Level 3.
- Notifications differ based on both **order status** and **SLA escalation level**.
- The **Current SLA Level** field is updated after each escalation to track progress.

## Output
- SLA breach alerts sent to internal teams
- Escalation notifications with increasing urgency
- Real-time visibility into delayed orders and bottlenecks

## Platform & Components
- Google Sheets (order status timestamps and SLA tracking)
- Make.com (time calculations, filters, and routing logic)
- Discord (SLA escalation alerts)
