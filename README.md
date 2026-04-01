# 📚 Prompt Library — Hotel Customer Service

> **Assessment 1 | AI for Business**  
> Student: Minh Duc Do
> student ID: 22221084  
> Business Field: Hotel Customer Service  
> Organisation Type: 5-star luxury hotel in Melbourne  
> Model tested on: GPT-5/Chatgpt
> Last updated: 01/04/2026
## What This Library Does

This prompt library supports workflow automation in hotel customer service for a 5-star luxury hotel in Melbourne. It contains 10 documented, tested, and iterated prompts organised by guest journey stage and service function.

Each prompt entry includes:
- the exact prompt text
- the workflow task it supports
- the problem it solves
- its automation potential
- risks and limitations
- version history and testing notes

## Folder Structure
```text
hotel-customer-service-prompt-library/
│
├── README.md
│
├── workflows/
│   ├── workflow-overview.md
│   ├── pre-arrival-workflow.md
│   ├── guest-service-workflow.md
│   └── post-stay-workflow.md
│
├── prompts/
│   ├── P01-pre-arrival-welcome-email.md
│   ├── P02-concierge-upsell-itinerary.md
│   ├── P03-service-request-response.md
│   ├── P04-complaint-triage.md
│   ├── P05-complaint-response-draft.md
│   ├── P06-incident-report.md
│   ├── P07-escalation-summary.md
│   ├── P08-late-checkout-or-special-request.md
│   ├── P09-review-response.md
│   └── P10-loyalty-followup.md
│
└── evaluations/
    ├── audit-log.md
    ├── test-results-summary.md
    └── prompting-strategies.md
```

Library Summary Table
| ID  | Prompt Name                     | Workflow         | Automation Level | Risk Level | Status         |
| --- | ------------------------------- | ---------------- | ---------------- | ---------- | -------------- |
| P01 | Pre-arrival welcome email       | Pre-arrival      | High             | Low        | 🔄 In progress |
| P02 | Concierge upsell itinerary      | Pre-arrival      | Medium           | Medium     | 🔄 In progress |
| P03 | Service request response        | In-stay service  | High             | Low        | 🔄 In progress |
| P04 | Complaint triage                | Customer service | Very High        | Medium     | 🔄 In progress |
| P05 | Complaint response draft        | Customer service | High             | Medium     | 🔄 In progress |
| P06 | Incident report                 | Operations       | Medium           | High       | 🔄 In progress |
| P07 | Escalation summary              | Service recovery | Medium           | High       | 🔄 In progress |
| P08 | Late checkout / special request | Guest service    | Medium           | Medium     | 🔄 In progress |
| P09 | Review response                 | Post-stay        | High             | Medium     | 🔄 In progress |
| P10 | Loyalty follow-up               | Post-stay        | High             | Low        | 🔄 In progress |

Prompt Chaining Map
PRE-ARRIVAL CHAIN
P01 (Pre-arrival welcome email) → P02 (Concierge upsell itinerary)

IN-STAY SERVICE CHAIN
P03 (Service request response) → P07 (Escalation summary if needed)

CUSTOMER SERVICE CHAIN
P04 (Complaint triage) → P05 (Complaint response draft) → P07 (Escalation summary)

POST-STAY CHAIN
P09 (Review response) → P10 (Loyalty follow-up)

Prompting Strategies Used
| Strategy | Prompts | Why chosen |
|----------|---------|------------|
| RACE framework (Role–Action–Context–Evaluation) | P01, P02, P03, P05, P09, P10 | Ensures tone, task clarity, and production-ready outputs |
| Grounding constraint ("use only the provided information") | P06, P07 | Reduces hallucination in factual or sensitive service contexts |
| JSON output format | P04 | Enables machine-readable complaint routing |
| Word/format limits | All | Keeps outputs concise, brand-consistent, and ready for operational use |
| Explicit exclusions | P01, P05, P09 | Prevents inclusion of pricing, sensitive data, or inappropriate wording |

Iteration Evidence

All prompt versions are saved in this repository. Commit history is used as the version log, and each prompt file includes its own version history.
