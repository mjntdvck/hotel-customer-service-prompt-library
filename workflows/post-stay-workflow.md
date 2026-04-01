# 📂 04 - Post-Stay Workflow

**Business function:** Guest Relations / Marketing / CRM  

**Trigger:** Guest check-out or review submission  

**Prompts in this section:** P09, P10  

---

## Section Purpose

This workflow supports post-stay engagement, reputation management, and guest retention.

Online reviews and follow-up communication significantly influence brand perception and repeat bookings. However, manual handling leads to inconsistent tone and missed opportunities for engagement.

With ~40–60 reviews and 100+ departures per week, this workflow reduces communication workload by **70–80%**, while improving brand consistency and customer loyalty.

---

## Chain Diagram

```
Guest check-out
        │
        ▼
   P09 · Review response (if review submitted)
        │
        ▼
   P10 · Loyalty follow-up email
        │
        ▼
   Guest retention → Repeat booking → CRM tracking
```
---

## Human-in-the-Loop Points

| Step | Human action required |
|------|-----------------------|
| P09 output | Staff review before publishing |
| P10 output | CRM team verifies personalisation |

---

## Prompts

| File | Prompt | Status |
|------|--------|--------|
| [P09-review-response.md](https://github.com/mjntdvck/hotel-customer-service-prompt-library/blob/main/prompts/P09-review-response.md) | Guest review response | ✅ Tested - v1.2 |
| [P10-loyalty-followup.md](https://github.com/mjntdvck/hotel-customer-service-prompt-library/blob/main/prompts/P10-loyalty-followup.md) | Loyalty follow-up email | ✅ Tested - v1.2 |
