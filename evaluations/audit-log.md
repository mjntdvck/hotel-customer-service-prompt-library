# 📊 Prompt Audit Log

## P01 - Pre-arrival Welcome Email

| Prompt version | Change made | Observed effect | Lesson learned |
|---------------|------------|----------------|---------------|
| v1.0 | Basic prompt without role or structure | Output generic, inconsistent tone, required full rewrite | Need role definition and structured sections |
| v1.1 | Added role (guest experience manager) and structured sections | Improved tone and clarity, but output too long (~250 words) | Need constraints (word limit) for production-ready output |
| v1.2 | Added 180-word limit and exclusions | Consistent, send-ready output, edit time reduced to ~2–3 min | Constraints + context = reliable outputs |

---

## P02 - Concierge Upsell & Itinerary

| Prompt version | Change made | Observed effect | Lesson learned |
|---------------|------------|----------------|---------------|
| v1.0 | Generic recommendation prompt | Irrelevant and non-personalised suggestions | Need guest context and structure |
| v1.1 | Added itinerary structure and guest profile inputs | Improved relevance but tone too promotional | Need tone control |
| v1.2 | Added “not sales-heavy” constraint and word limit | More natural, luxury-standard responses, reduced edits | Tone constraints are critical in hospitality |

---

## P03 - Service Request Response

| Prompt version | Change made | Observed effect | Lesson learned |
|---------------|------------|----------------|---------------|
| v1.0 | Basic reply prompt | Generic responses, inconsistent tone | Need structured response format |
| v1.1 | Added structured sections and tone guidance | More usable but sometimes verbose | Need length constraint |
| v1.2 | Added 120-word limit and urgency logic | Fast, consistent responses, edit time ~1–2 min | Constraints + urgency handling improve reliability |

---

## P04 - Complaint Triage (JSON)

| Prompt version | Change made | Observed effect | Lesson learned |
|---------------|------------|----------------|---------------|
| v1.0 | Free-text classification prompt | Output not machine-readable, unusable for automation | Need structured output (JSON) |
| v1.1 | Added JSON output requirement | Format correct but categories inconsistent | Need constrained taxonomy |
| v1.2 | Added fixed categories and urgency rules | 90%+ accuracy, successful CRM integration | Constraints + structure enable automation |

---

## P05 - Complaint Response

| Prompt version | Change made | Observed effect | Lesson learned |
|---------------|------------|----------------|---------------|
| v1.0 | Generic response prompt | Weak tone, inconsistent structure | Need defined response components |
| v1.1 | Added apology + acknowledgement structure | Improved clarity but sometimes too long | Need constraints |
| v1.2 | Added 150-word limit and urgency handling | Consistent, professional responses, minimal editing | Structured logic improves service quality |

---

## P06 - Incident Report

| Prompt version | Change made | Observed effect | Lesson learned |
|---------------|------------|----------------|---------------|
| v1.0 | Open-ended report generation | Model hallucinated causes not in notes | Need grounding constraint |
| v1.1 | Added “use ONLY provided information” + fallback | No hallucination, accurate reports | Grounding is critical for factual tasks |

---

## P07 - Escalation Summary

| Prompt version | Change made | Observed effect | Lesson learned |
|---------------|------------|----------------|---------------|
| v1.0 | Basic summarisation prompt | Missing key decision points | Need structured format |
| v1.1 | Added sections (overview, status, risk, action) | More useful but sometimes included assumptions | Need grounding constraint |
| v1.2 | Added grounding + word limit | Clear, decision-ready summaries | Structure + grounding improves decision support |

---

## P08 - Special Request Handling

| Prompt version | Change made | Observed effect | Lesson learned |
|---------------|------------|----------------|---------------|
| v1.0 | Simple response prompt | Inconsistent handling of approvals vs rejections | Need conditional logic |
| v1.1 | Added availability-based branching | More consistent but sometimes verbose | Need constraints |
| v1.2 | Added word limit and rules | Reliable, guest-friendly responses | Conditional logic + constraints improve consistency |

---

## P09 - Review Response

| Prompt version | Change made | Observed effect | Lesson learned |
|---------------|------------|----------------|---------------|
| v1.0 | Generic review reply prompt | Poor handling of negative reviews | Need conditional logic |
| v1.1 | Added positive vs negative structure | Improved responses but too long | Need constraints |
| v1.2 | Added word limit and tone control | Consistent, publish-ready responses | Tone + structure protect brand image |

---

## P10 - Loyalty Follow-up

| Prompt version | Change made | Observed effect | Lesson learned |
|---------------|------------|----------------|---------------|
| v1.0 | Generic follow-up email | Too promotional, low engagement | Need personalisation |
| v1.1 | Added stay summary and highlights | Improved relevance but inconsistent tone | Need tone refinement |
| v1.2 | Added constraints and exclusions | Strong, relationship-focused emails | Personalisation + tone drive retention |

---
