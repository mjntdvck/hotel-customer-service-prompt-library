# 📂 02 - In-Stay Guest Service Workflow

**Business function:** Front Office / Guest Services  

**Trigger:** Guest request or service inquiry during stay  

**Prompts in this section:** P03, P08  

---

## Section Purpose

This workflow supports real-time guest service communication during the stay.

Luxury hotels handle a high volume of guest requests (e.g. housekeeping, late check-out, special arrangements). Manual response drafting leads to inconsistent tone and slower response times.

At ~150 requests per day, this workflow can save **7–12 hours of staff time daily**, while ensuring consistent, high-quality communication aligned with brand standards.

---

## Chain Diagram

```
Guest request received
        │
        ▼
   P03 · Service request response
        │
        ▼
   P08 · Special request / exception handling
        │
        ▼
   Request fulfilled or alternative provided
        │
        ▼
   If unresolved → Escalation (P07) 
```
---

## Human-in-the-Loop Points

| Step | Human action required |
|------|-----------------------|
| P03 output | Staff verify request details before sending |
| P08 output | Staff confirm availability and approval before response |

---

## Prompts

| File | Prompt | Status |
|------|--------|--------|
| [P03-service-request-response.md](https://github.com/mjntdvck/hotel-customer-service-prompt-library/blob/main/prompts/P03-service-request-response.md) | Service request response | ✅ Tested - v1.2 |
| [P08-special-request-handling.md](https://github.com/mjntdvck/hotel-customer-service-prompt-library/blob/main/prompts/P08-late-checkout-or-special-request.md) | Special request / late check-out handling | ✅ Tested - v1.2 |
