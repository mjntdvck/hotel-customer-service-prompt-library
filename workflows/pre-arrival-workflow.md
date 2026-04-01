# 📂 01 - Pre-arrival Workflow

**Business function:** Guest Experience / Front Office  

**Trigger:** Booking confirmed in Property Management System (PMS)  

**Prompts in this section:** P01, P02  

---

## Section Purpose

This workflow automates pre-arrival guest communication for a 5-star luxury hotel in Melbourne. 

Pre-arrival engagement is critical in shaping first impressions and influencing guest satisfaction. However, drafting personalised emails and concierge recommendations is time-intensive.

With approximately 100–120 arrivals per week, manual communication can require **20–30 hours of staff time weekly**. This prompt chain reduces workload by up to **70–80%**, while improving consistency, personalisation, and upsell opportunities.

---
```
Booking confirmed in PMS
        │
        ▼
   P01 · Pre-arrival welcome email
        │
        ▼
   P02 · Concierge upsell & itinerary
        │
        ▼
   Guest engagement → Requests / bookings / upsell conversion
```
---

## Human-in-the-Loop Points

| Step | Human action required |
|------|-----------------------|
| P01 output | Front office reviews tone and guest details before sending |
| P02 output | Concierge verifies recommendations and availability |

---

## Prompts

| File | Prompt | Status |
|------|--------|--------|
| [P01-pre-arrival-welcome-email.md](https://github.com/mjntdvck/hotel-customer-service-prompt-library/blob/main/prompts/P01-pre-arrival-welcome-email.md) | Pre-arrival welcome email | ✅ Tested - v1.2 |
| P02-concierge-upsell-itinerary.md | Concierge upsell & itinerary | ✅ Tested - v1.2 |
