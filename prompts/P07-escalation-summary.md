**🏨 P07 · Escalation summary for management (Luxury Hotel – Melbourne)**

**📌 Prompt Text (v1.2 - current)**

Copy this exactly into your AI tool. Replace all [PLACEHOLDERS] before running.

You are a duty manager at a 5-star luxury hotel in Melbourne.

Using ONLY the information provided below, prepare a concise escalation summary for senior management.

Inputs:
- Complaint category: [CATEGORY]
- Complaint summary: [SUMMARY]
- Urgency level: [URGENCY]
- Incident report (if available): [INCIDENT_REPORT]
- Actions taken so far: [ACTIONS_TAKEN]

Your summary must include:

1. Incident overview (what happened, guest impact)
2. Current status (what has been done so far)
3. Risk assessment (operational, reputational, or safety risk)
4. Recommended action (clear next step for management decision)

Tone: formal, concise, and management-focused.  
Style: objective, no emotional language.  
Length: maximum 180 words.  

Rules:
- Do not infer or assume missing information  
- If any input is incomplete, state: "Insufficient data - follow-up required"  
- Prioritise clarity and decision-making relevance

**📊 Placeholders to fill**

| Placeholder         | Source                 | Example                               |
| ------------------- | ---------------------- | ------------------------------------- |
| `[CATEGORY]`        | P04 output             | Room cleanliness                      |
| `[SUMMARY]`         | P04 output             | Guest found room unclean upon arrival |
| `[URGENCY]`         | P04 output             | High                                  |
| `[INCIDENT_REPORT]` | P06 output (if exists) | Structured report                     |
| `[ACTIONS_TAKEN]`   | Staff input            | Room cleaned, guest offered apology   |

**🏢 Intended Workflow or Task**

This prompt is the final step in the service recovery and incident escalation workflow.

- Trigger:
Complaint marked High urgency (P04)
OR serious incident reported (P06)
- Actor: Duty manager generates escalation summary for senior management
- Timing: Immediate (within 30–60 minutes of issue)
Next step:
- Management decision
- Compensation / recovery actions
- Policy or operational review

Complaint → P04 (triage) → P05 (response)
        → If High → [P07 RUNS]

OR

Incident → P06 (report) → [P07 RUNS]
                         → Management review
                         → Decision / action
**❗ Problem Being Solved**
- Duty managers spend 10–15 minutes per case summarising complex issues for management.
- In high-end hotels handling multiple escalations per week:
- This leads to delays in decision-making

**Key pain points:**
- Inconsistent escalation summaries across managers
- Missing critical information for decision-making
- Slow response in high-risk situations

**⚡ Automation Potential**

**Level: Medium**

| Dimension               | Assessment                                    |
| ----------------------- | --------------------------------------------- |
| Repetitiveness          | Medium - structure consistent, content varies |
| Data availability       | Dependent on upstream prompts (P04, P06)      |
| Human judgment needed   | High - strategic decisions required           |
| Integration possibility | Can integrate with internal reporting tools   |
| Estimated time saving   | ~50–60% (15 min → 6–7 min including review)   |

**Human-in-the-loop role:**
Duty manager validates summary before sending to senior management.

**Business impact:**
- Faster decision-making
- Improved service recovery
- Reduced reputational risk
- Better internal communication

**⚠️ Risks and Limitations**

| Risk                                  | Level  | Mitigation                                                   |
| ------------------------------------- | ------ | ------------------------------------------------------------ |
| Missing or incomplete input data      | Medium | Explicit fallback: "Insufficient data - follow-up required"  |
| Incorrect risk assessment             | High   | Manager review required                                      |
| Over-simplification of complex issues | Medium | Include structured sections (overview, status, risk, action) |
| Escalation used without verification  | High   | Mandatory human validation                                   |

Overall risk rating: HIGH
→ Cannot be fully automated - requires managerial oversight

**🔄 Version History**

**v1.0 - Initial draft**

- Prompt:
Summarise this issue for management.

- Output:
Unstructured, inconsistent, sometimes omitted key risks

- Observed effect:
Managers required full rewrite

- Lesson learned:
Need structured format aligned to decision-making

**v1.1 - Added structured sections**

- Change:

Added sections: overview, status, risk, action
Improved clarity

- Output:
More usable, but sometimes included assumptions

- Observed effect:
Edit time reduced to ~8–10 minutes

- Lesson learned:
Need grounding constraint

**v1.2 - Added grounding + constraints ✅ Current**

- Change:

Added “use ONLY provided information”
Added fallback for missing data
Added strict word limit

- Output:
Clear, concise, decision-ready summaries

- Observed effect:
Edit time reduced to ~5–7 minutes

- Lesson learned:
Structure + grounding = reliable management communication

**📊 A/B Test Results**

Sample: 10 escalation scenarios

| Criteria                    | v1.0  | v1.2  |
| --------------------------- | ----- | ----- |
| Clarity for decision-making | 2/5   | 4.7/5 |
| Completeness                | 2.5/5 | 4.6/5 |
| Consistency                 | 2/5   | 4.8/5 |
| Time to use                 | 1/5   | 4.5/5 |

**🔗 Related Prompts**

Inputs from:

→ P04 - Complaint triage

→ P05 - Complaint response

→ P06 - Incident report

Final stage: Management decision & action
