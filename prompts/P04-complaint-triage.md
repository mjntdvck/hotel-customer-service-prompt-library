**🏨 P04 · Complaint triage and classification (Luxury Hotel – Melbourne)**
**📌 Prompt Text (v1.2 - current)**

Copy this exactly into your AI tool. Replace all [PLACEHOLDERS] before running.

Classify the following hotel guest complaint.

Choose EXACTLY ONE category from this list:
- Room cleanliness
- Noise disturbance
- Service delay
- Staff conduct
- Facilities issue
- Billing / payment
- Other

Rate urgency as one of: Low / Medium / High

Use "High" if the complaint involves:
- safety concerns
- discrimination or misconduct
- severe dissatisfaction (e.g. threat to leave, negative review, escalation request)

Complaint text: [COMPLAINT_TEXT]

Respond in JSON only. Do not include any explanation or text outside the JSON.

{
  "category": "[chosen category]",
  "urgency": "[Low / Medium / High]",
  "summary": "[One concise sentence summarising the complaint]",
  "reason": "[Why this category and urgency were chosen]"
}

**📊 Placeholders to fill**
| Placeholder        | Source                              | Example                                                               |
| ------------------ | ----------------------------------- | --------------------------------------------------------------------- |
| `[COMPLAINT_TEXT]` | Guest email / app / front desk note | "The room was not cleaned properly and I found hair in the bathroom." |

**🏢 Intended Workflow or Task**

This prompt is Step 1 of the complaint handling workflow, enabling automated triage and routing.

Trigger: Guest submits complaint (app, email, or front desk)

Integration: JSON output is parsed by CRM / hotel system

Actor: Fully automated (with periodic audit)

Timing: Immediate (real-time processing)

Next step:

Routed to correct department

P05 (response draft) triggered

If urgency = High → escalation (P07)

Complaint received → [P04 RUNS] → JSON output → System routes issue
                                           → Department assigned
                                           → P05 triggered
                                           → If High → P07 escalation
**❗ Problem Being Solved**

Front desk or guest relations managers spend 2–4 minutes per complaint manually categorising and prioritising issues.

In a 5-star hotel handling ~80 complaints per day:

This results in 3–5 hours of triage work daily

**Key pain points:**

Inconsistent classification → wrong department routing
Delays in handling urgent issues
Lack of standardised urgency prioritisation

**⚡ Automation Potential**
**Level: Very High**

| Dimension               | Assessment                                     |
| ----------------------- | ---------------------------------------------- |
| Repetitiveness          | Extremely high - same classification task      |
| Data availability       | Always available (complaint text)              |
| Human judgment needed   | Low for most cases                             |
| Integration possibility | Direct integration with CRM / ticketing system |
| Estimated time saving   | ~90–95% (manual → near-instant)                |

**Human-in-the-loop role:**
Daily audit of “Other” category
Immediate review of High urgency cases

**Business impact:**
Faster response times
Improved service recovery
Reduced operational bottlenecks
Higher guest satisfaction

**⚠️ Risks and Limitations**
| Risk                                          | Level    | Mitigation                                   |
| --------------------------------------------- | -------- | -------------------------------------------- |
| Complaint fits multiple categories            | Medium   | Use "Other" category + human review          |
| Urgency misclassification (High → Low)        | **High** | Explicit urgency rules in prompt             |
| JSON output malformed                         | Medium   | API validation before processing             |
| Sensitive complaints mishandled automatically | High     | High urgency triggers mandatory human review |

Overall risk rating: MEDIUM–HIGH
→ Suitable for automation with governance and monitoring

**🔄 Version History**
**v1.0 - Initial draft**

Prompt:
Classify this hotel complaint and rate urgency.

Output:
Free-text response, inconsistent format, varied categories

Observed effect:
Could not integrate with system → manual intervention required

Lesson learned:
Need structured output (JSON)

**v1.1 - Added JSON output**

Change:

Enforced JSON format
Still allowed model to define its own categories

Output:
JSON format correct, but inconsistent categories (e.g. “cleaning issue”, “dirty room”)

Observed effect:
Routing errors in system

Lesson learned:
Must constrain category list

**v1.2 - Constrained categories + urgency rules ✅ Current**

Change:

Added fixed category list
Defined urgency criteria
Added summary field

Output:
Consistent, machine-readable, reliable classification

Observed effect:
~93–95% classification accuracy in test cases

Lesson learned:
Constraints + structured output = production-ready automation

**📊 A/B Test Results**

Sample: 30 hotel complaints (mixed types)

| Criteria                   | v1.0   | v1.2       |
| -------------------------- | ------ | ---------- |
| Machine-readable output    | 0%     | 100%       |
| Category consistency       | Low    | 94%        |
| Urgency accuracy           | Low    | 92%        |
| System integration success | Failed | Successful |

**🔗 Related Prompts**
Next in chain: P05 - Complaint response draft
Escalation: P07 - Escalation summary
Related:
→ P03 - Service request response
