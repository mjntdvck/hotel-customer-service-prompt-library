**🏨 P03 · Service request response (Luxury Hotel – Melbourne)**
**📌 Prompt Text (v1.2 - current)**

Copy this exactly into your AI tool. Replace all [PLACEHOLDERS] before running.

You are a front desk associate at a 5-star luxury hotel in Melbourne.

Draft a professional and personalised response to a guest request.

Guest details:
- Guest name: [GUEST_NAME]
- Room number: [ROOM_NUMBER]
- Request: [REQUEST_DETAILS]
- Urgency level: [URGENCY] (Low / Medium / High)

Your response must include:
1. A polite acknowledgement of the request
2. Confirmation that the request is being handled (or completed)
3. Clear next steps or expected timing
4. A closing line offering further assistance

Tone: warm, attentive, and refined - consistent with luxury hospitality standards.  
Style: concise and reassuring.  
Length: maximum 120 words.  

If urgency is High:
- Add an apology for inconvenience
- Emphasise immediate action

Do not include: internal processes, staff names, or operational details.

**📊 Placeholders to fill**
| Placeholder         | Source               | Example                  |
| ------------------- | -------------------- | ------------------------ |
| `[GUEST_NAME]`      | PMS                  | Mr. Smith                |
| `[ROOM_NUMBER]`     | PMS                  | 1205                     |
| `[REQUEST_DETAILS]` | Guest call / app     | Request for extra towels |
| `[URGENCY]`         | Staff classification | Medium                   |

**🏢 Intended Workflow or Task**

This prompt is part of the in-stay guest service workflow, handling real-time guest requests.

Trigger: Guest submits a request (phone, app, or front desk)
Actor: Front desk or guest service agent reviews and sends response
Timing: Immediate (within minutes of request)
Next step: Service fulfilled → guest satisfaction checked → escalation if unresolved (P07)
Guest request received → [P03 RUNS] → Staff reviews → Response sent
                                           → Service fulfilled
                                           → If issue persists → P07 triggered
**❗ Problem Being Solved**

Front desk staff spend **3–5 minutes per request** drafting responses, especially during peak hours.

In a 5-star hotel handling **~150 requests per day**:

This equates to **7.5–12.5 hours of communication workload daily**

Key pain points:

Inconsistent tone across staff members
Delays in response during busy periods
Lack of clarity in communication → repeated follow-ups
**⚡ Automation Potential**
**Level: High**

| Dimension               | Assessment                                         |
| ----------------------- | -------------------------------------------------- |
| Repetitiveness          | Very high - similar structure for most requests    |
| Data availability       | All inputs available from PMS or guest interaction |
| Human judgment needed   | Low - mostly tone and clarity check                |
| Integration possibility | Can integrate with guest service apps or CRM       |
| Estimated time saving   | ~70–80% (5 min → 1–2 min review)                   |

**Human-in-the-loop role:**
Staff verify accuracy (room number, request details) before sending.

**Business impact:**

Faster response times → improved guest satisfaction
Reduced staff workload during peak periods
Consistent luxury-standard communication

**⚠️ Risks and Limitations**
| Risk                                             | Level  | Mitigation                          |
| ------------------------------------------------ | ------ | ----------------------------------- |
| Incorrect or unclear request details             | Medium | Staff verify inputs before sending  |
| Overly generic responses reduce guest experience | Low    | Prompt enforces personalised tone   |
| Urgent issues not escalated properly             | High   | Explicit urgency handling in prompt |
| Miscommunication of service timing               | Medium | Staff confirm realistic timelines   |

Overall risk rating: LOW–MEDIUM
→ Suitable for near-full automation with quick human validation.

**🔄 Version History**
**v1.0 - Initial draft**

Prompt:
Reply to a hotel guest request.

Output:
Too generic, no structure, inconsistent tone

Observed effect:
Required significant rewriting → minimal time saving

Lesson learned:
Need role + structure + clear response components

**v1.1 - Added structure and tone**

Change:

Added role (front desk associate)
Defined required sections
Introduced tone guidelines

Output:
More consistent and usable, but sometimes too long or vague

Observed effect:
Edit time reduced to ~3 minutes

Lesson learned:
Need length constraint and urgency handling

**v1.2 - Added constraints and urgency logic ✅ Current**

Change:

Added 120-word limit
Added urgency-specific instructions
Clarified response structure

Output:
Consistent, concise, and appropriate for guest communication

Observed effect:
Edit time reduced to ~1–2 minutes

Lesson learned:
Explicit constraints + urgency logic = reliable real-time responses

**📊 A/B Test Results**

Sample: 10 guest requests (mixed urgency levels)

| Criteria         | v1.0  | v1.2  |
| ---------------- | ----- | ----- |
| Response clarity | 2.5/5 | 4.7/5 |
| Tone consistency | 2/5   | 4.8/5 |
| Speed of use     | 1/5   | 4.5/5 |
| Need for editing | High  | Low   |

**🔗 Related Prompts**
Previous: P02 - Concierge upsell itinerary
Next: P07 - Escalation summary (if issue unresolved)
Related:
→ P04 - Complaint triage
→ P05 - Complaint response draft
