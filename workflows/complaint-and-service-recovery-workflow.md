# 📂 03 — Complaint & Service Recovery Workflow

**Business function:** Guest Relations / Service Recovery  

**Trigger:** Guest complaint received (app, email, or front desk) 

**Prompts in this section:** P04, P05, P07  

---

## Section Purpose

This workflow automates the triage, response, and escalation of guest complaints.

In luxury hospitality, fast and consistent complaint handling is critical to avoid reputational damage. Manual triage and response processes are time-consuming and inconsistent.

At ~80 complaints per day, this workflow reduces handling time by **70–90%**, while improving response quality and ensuring proper escalation of high-risk issues.

---

## Chain Diagram

```
Complaint received
        │
        ▼
   P04 · Complaint triage (JSON output → system routing)
        │
        ▼
   P05 · Complaint response draft
        │
        ▼
   Response sent to guest
        │
        ▼ (if High urgency / serious issue)
   P07 · Escalation summary for management
```
---

## Human-in-the-Loop Points

| Step | Human action required |
|------|-----------------------|
| P04 output | Periodic audit and review of high-urgency cases |
| P05 output | Guest relations team reviews before sending |
| P07 output | Duty manager validates before escalation |

---

## Prompts

| File | Prompt | Status |
|------|--------|--------|
| P04-complaint-triage.md | Complaint triage and classification | ✅ Tested — v1.2 |
| P05-complaint-response.md | Complaint response draft | ✅ Tested — v1.2 |
| P07-escalation-summary.md | Escalation summary for management | ✅ Tested — v1.2 |
