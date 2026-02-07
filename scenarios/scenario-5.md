# Scenario 5 – SLA Recovery & De-Escalation

## Purpose
This scenario ensures SLA levels remain accurate by resetting or reducing escalation when an order progresses to a new status.

## Trigger
- Order status change

## Logic Overview
Recovery notifications are sent only once per recovery event to avoid duplicate messages.
  
- The scenario checks if the order status has progressed beyond the delayed stage.
- If an order moves forward in its lifecycle, the associated SLA level is reset.
- Recovery logic prevents repeated or false escalations.
- Recovery notifications are sent only once per recovery event to avoid duplicate messages.

## Output
- Corrected SLA levels
- Orders that previously triggered SLA escalations are re-evaluated.
- Clean and reliable escalation history

## Platform & Components
- Google Sheets (order and SLA data)
- Make.com (state evaluation and updates)
- Discord (SLA recovery notifications)
