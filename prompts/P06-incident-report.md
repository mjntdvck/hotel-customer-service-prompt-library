**🏨 P06 · Incident report draft (Luxury Hotel – Melbourne)**
**📌 Prompt Text (v1.1 - current)**

Copy this exactly into your AI tool. Replace all [PLACEHOLDERS] before running.

You are an operations manager at a 5-star luxury hotel in Melbourne.

Using ONLY the information provided below, write a structured incident report.
Do not infer, assume, or add any information that is not explicitly stated.

Incident notes: [INCIDENT_NOTES]

Your report must include:

1. Summary (2–3 sentences: what happened, when, where)
2. Timeline (bullet points with approximate times if available)
3. Root cause (ONLY if explicitly stated - otherwise write: "Root cause: Insufficient data - follow-up required")
4. Immediate actions taken
5. Recommended next steps

Tone: factual, neutral, and professional.  
Style: third-person, objective.  
Length: maximum 250 words.  

If any section cannot be completed:
- Write: "Insufficient data - follow-up required"

**📊 Placeholders to fill**

| Placeholder        | Source                      | Example                                                                                     |
| ------------------ | --------------------------- | ------------------------------------------------------------------------------------------- |
| `[INCIDENT_NOTES]` | Staff report / internal log | "Guest slipped near pool area at 6pm. No warning sign visible. Staff provided first aid..." |

**🏢 Intended Workflow or Task**

This prompt is Step 1 of the incident management workflow, supporting internal reporting and escalation.

- Trigger: Incident reported by staff or guest
- Actor: Duty manager generates report and reviews output
- Timing: Within 1–2 hours of incident
Next step:
- Manager sign-off
- Escalation if required (P07)
- Record stored in incident management system
Incident reported → Staff notes recorded → [P06 RUNS]
                                  → Manager reviews draft
                                  → Report submitted
                                  → If serious → P07 escalation

**❗ Problem Being Solved**
- Duty managers spend 20–30 minutes per incident drafting structured reports.
- In a hotel with ~10–15 incidents per week:
- This results in 3–7 hours of reporting workload weekly

**Key pain points:**
- Inconsistent report structure across managers
- Missing critical details (timeline, actions)
- Risk of inaccurate or assumed information in reports

**⚡ Automation Potential**
**Level: Medium**

| Dimension               | Assessment                                              |
| ----------------------- | ------------------------------------------------------- |
| Repetitiveness          | High - same report structure required                   |
| Data availability       | Depends on quality of incident notes                    |
| Human judgment needed   | High - factual verification required                    |
| Integration possibility | Output can be uploaded into incident management systems |
| Estimated time saving   | ~50–60% (30 min → 12–15 min including review)           |

**Human-in-the-loop role:**
Duty manager must verify all facts before submission (mandatory).

**Business impact:**
- Improved reporting consistency
- Reduced administrative workload
- Lower compliance and legal risk

**⚠️ Risks and Limitations**

| Risk                                               | Level    | Mitigation                                                    |
| -------------------------------------------------- | -------- | ------------------------------------------------------------- |
| Model invents details not in notes (hallucination) | **High** | Strict grounding constraint ("use ONLY provided information") |
| Incomplete notes lead to incomplete reports        | Medium   | Fallback phrase "Insufficient data - follow-up required"      |
| Report used without verification                   | **High** | Mandatory manager sign-off policy                             |
| Legal implications from incorrect reporting        | **High** | Require validation against CCTV, logs, and witness statements |

Overall risk rating: HIGH
→ Never fully automated - requires strict human oversight

**🔄 Version History**
**v1.0 - Initial draft**

- Prompt:
Write an incident report based on these notes.

- Output:
Well-written but added assumed causes and missing details

- Observed effect:
Risk of inaccurate reporting → unacceptable in operational context

- Lesson learned:
Need grounding constraint to prevent hallucination

**v1.1 - Added grounding constraint and fallback ✅ Current**

- Change:

Added "use ONLY provided information"
Added fallback for missing data
Added strict structure

- Output:
Accurate, structured, no fabricated details

- Observed effect:
0 hallucinations across test cases

- Lesson learned:
Grounding constraints are critical for factual reporting

**📊 A/B Test Results**

Sample: 8 incident reports (realistic scenarios)

| Criteria           | v1.0   | v1.1 |
| ------------------ | ------ | ---- |
| Factual accuracy   | 2/5    | 5/5  |
| Hallucination rate | High   | 0%   |
| Usability          | Medium | High |
| Need for rewriting | High   | Low  |

**🔗 Related Prompts**

Next: P07 - Escalation summary

Related:

→ P04 - Complaint triage

→ P05 - Complaint response
