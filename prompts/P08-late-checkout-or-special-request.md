**🏨 P08 · Special request & late check-out handling (Luxury Hotel – Melbourne)**

**📌 Prompt Text (v1.2 - current)**

Copy this exactly into your AI tool. Replace all [PLACEHOLDERS] before running.

You are a front office supervisor at a 5-star luxury hotel in Melbourne.

Draft a professional response to a guest request that may require approval or depends on availability.

Guest details:
- Guest name: [GUEST_NAME]
- Room number: [ROOM_NUMBER]
- Request type: [REQUEST_TYPE] (e.g. late check-out, early check-in, special arrangement)
- Request details: [REQUEST_DETAILS]
- Availability status: [AVAILABILITY] (Available / Limited / Not available)

Your response must include:

1. A polite acknowledgement of the request
2. A clear response based on availability:
   - If Available → confirm approval
   - If Limited → provide conditional approval or alternative
   - If Not available → politely decline and offer an alternative
3. Any relevant next steps or timing
4. A closing line offering further assistance

Tone: warm, professional, and solution-oriented - aligned with luxury hospitality standards.  
Style: respectful and accommodating, even when declining.  
Length: maximum 130 words.  

Rules:
- Do not promise unavailable services  
- Do not mention internal constraints (e.g. staffing, occupancy levels)  
- Always offer an alternative when declining

**📊 Placeholders to fill**

| Placeholder         | Source               | Example                     |
| ------------------- | -------------------- | --------------------------- |
| `[GUEST_NAME]`      | PMS                  | Mr. Lee                     |
| `[ROOM_NUMBER]`     | PMS                  | 1802                        |
| `[REQUEST_TYPE]`    | Guest interaction    | Late check-out              |
| `[REQUEST_DETAILS]` | Guest request        | Requesting check-out at 3pm |
| `[AVAILABILITY]`    | System / staff input | Limited                     |

**🏢 Intended Workflow or Task**

This prompt is part of the guest service exception handling workflow, managing requests that depend on availability or policy.

- Trigger: Guest submits a request that requires approval or capacity check
- Actor: Front office or duty manager reviews and sends response
- Timing: Within minutes of request

Next step:
- Request fulfilled
- Alternative arranged
- Escalation if guest dissatisfied (P07)

Guest request received → Availability checked → [P08 RUNS]
                                         → Staff reviews → Response sent
                                         → If dissatisfied → P07 escalation
**❗ Problem Being Solved**
- Front office staff spend 3–6 minutes per request crafting responses for special requests.
- In a luxury hotel handling ~50 such requests daily:
- This results in 2.5–5 hours of communication workload per day

**Key pain points:**
- Inconsistent handling of approval vs rejection
- Poor phrasing when declining requests → guest dissatisfaction
- Missed opportunities to offer alternatives-

**⚡ Automation Potential**

**Level: High**

| Dimension               | Assessment                                    |
| ----------------------- | --------------------------------------------- |
| Repetitiveness          | High - similar structure across requests      |
| Data availability       | Requires availability input                   |
| Human judgment needed   | Medium - depends on context                   |
| Integration possibility | Can integrate with PMS and front desk systems |
| Estimated time saving   | ~70–80% (5 min → 1–2 min review)              |

**Human-in-the-loop role:**
Staff confirm availability and appropriateness before sending.

**Business impact:**
- Improved guest satisfaction (even when declining)
- More consistent service delivery
- Reduced workload for front office staff

⚠️ Risks and Limitations

| Risk                                                  | Level  | Mitigation                                         |
| ----------------------------------------------------- | ------ | -------------------------------------------------- |
| Incorrect availability input leads to wrong response  | High   | Staff verification required                        |
| Guest dissatisfaction if decline not handled properly | Medium | Prompt enforces alternative suggestions            |
| Over-promising services                               | High   | Explicit rule: do not promise unavailable services |
| Generic responses reduce luxury experience            | Low    | Tone and structure constraints                     |

Overall risk rating: MEDIUM–HIGH
→ Requires human validation before sending

**🔄 Version History**

**v1.0 - Initial draft**

- Prompt:
Respond to a guest request about late check-out.

- Output:
Basic response, inconsistent handling of approval vs rejection

- Observed effect:
Staff needed to rewrite responses

- Lesson learned:
Need structured logic based on availability

**v1.1 - Added conditional logic**

- Change:

Added availability-based branching (approve / conditional / decline)
Added alternative suggestions

- Output:
More consistent, but sometimes too long

- Observed effect:
Edit time reduced to ~3 minutes

- Lesson learned:
Need concise output constraint

**v1.2 - Added constraints and tone control ✅ Current**

- Change:

Added 130-word limit
Refined tone to “solution-oriented”
Added explicit rules

- Output:
Consistent, professional, and guest-friendly responses

- Observed effect:
Edit time reduced to ~1–2 minutes

- Lesson learned:
Conditional logic + constraints = reliable service communication

**📊 A/B Test Results**

Sample: 12 guest requests (mixed availability scenarios)

| Criteria                | v1.0 | v1.2  |
| ----------------------- | ---- | ----- |
| Consistency of response | 2/5  | 4.7/5 |
| Handling of declines    | 2/5  | 4.6/5 |
| Guest-friendly tone     | 3/5  | 4.8/5 |
| Need for editing        | High | Low   |

**🔗 Related Prompts**

Related:

→ P03 - Service request response

→ P05 - Complaint response

Escalation:

→ P07 - Escalation summary
