**🏨 P05 · Complaint response draft (Luxury Hotel – Melbourne)**

**📌 Prompt Text (v1.2 - current)**

Copy this exactly into your AI tool. Replace all [PLACEHOLDERS] before running.

You are a guest relations manager at a 5-star luxury hotel in Melbourne.

Draft a professional and empathetic response to a guest complaint.

Guest details:
- Guest name: [GUEST_NAME]
- Complaint category: [CATEGORY]
- Complaint summary: [SUMMARY]
- Urgency level: [URGENCY] (Low / Medium / High)

Your response must include:
1. A sincere apology (regardless of fault)
2. A clear acknowledgement of the issue
3. Reassurance that the issue is being addressed
4. A brief explanation or next step (if appropriate)
5. A closing line offering further assistance

Tone: empathetic, calm, and refined - aligned with luxury hospitality standards.  
Style: professional and reassuring, not defensive.  
Length: maximum 150 words.  

If urgency is High:
- Emphasise urgency and immediate action
- Include a stronger reassurance statement

Do not include:
- Blame toward staff or systems
- Legal language
- Internal investigation details

**📊 Placeholders to fill**
  
| Placeholder    | Source          | Example                                    |
| -------------- | --------------- | ------------------------------------------ |
| `[GUEST_NAME]` | PMS             | Ms. Nguyen                                 |
| `[CATEGORY]`   | Output from P04 | Room cleanliness                           |
| `[SUMMARY]`    | Output from P04 | Room was not properly cleaned upon arrival |
| `[URGENCY]`    | Output from P04 | High                                       |

**🏢 Intended Workflow or Task**

This prompt is Step 2 of the complaint handling workflow, following P04 (triage).
- Trigger: Complaint classified and prioritised by P04
- Actor: Guest relations team reviews and sends response
- Timing: Within minutes of complaint receipt

Next step:
- Issue resolved
- Follow-up if needed
- Escalation triggered if unresolved (P07)

**Complaint received → P04 (triage) → [P05 RUNS] → Draft response generated
                                          → Staff reviews → Response sent
                                          → If unresolved → P07 escalation**
                                          
**❗ Problem Being Solved**
- Guest relations staff spend 5–10 minutes per complaint drafting personalised responses.
- In a 5-star hotel handling ~80 complaints per day:
- This results in 6–13 hours of communication workload daily

**Key pain points:**
- Inconsistent tone across staff (risk to brand image)
- Delayed responses → escalation of guest dissatisfaction
- Poorly worded responses leading to negative reviews

**⚡ Automation Potential**

**Level: High**

| Dimension               | Assessment                                              |
| ----------------------- | ------------------------------------------------------- |
| Repetitiveness          | High - structured response pattern                      |
| Data availability       | Provided by P04 output                                  |
| Human judgment needed   | Medium - tone and appropriateness must be reviewed      |
| Integration possibility | Can integrate with CRM or guest communication platforms |
| Estimated time saving   | ~70–80% (10 min → 2–3 min review)                       |

**Human-in-the-loop role:**
Guest relations staff review tone, accuracy, and appropriateness before sending.

**Business impact:**
- Faster response times
- Improved service recovery
- Reduced negative reviews
- Stronger brand consistency

**⚠️ Risks and Limitations**

| Risk                                        | Level  | Mitigation                                            |
| ------------------------------------------- | ------ | ----------------------------------------------------- |
| Over-apologising or inappropriate tone      | Medium | Tone constraints + staff review                       |
| Response not aligned with actual resolution | High   | Staff must confirm operational actions before sending |
| Generic responses reduce guest satisfaction | Low    | Personalisation via summary and category              |
| Sensitive complaints handled improperly     | High   | High urgency triggers escalation review (P07)         |

**Overall risk rating: MEDIUM–HIGH**
→ Requires human validation before sending

**🔄 Version History**
**v1.0 - Initial draft**

Prompt:
Write a reply to a hotel complaint.

- Output:
Generic, sometimes defensive tone, inconsistent structure

- Observed effect:
Required rewriting → limited time saving

- Lesson learned:
Need structured response format + tone control

**v1.1 - Added structure and tone guidelines**

- Change:

Added apology + acknowledgement + reassurance structure
Defined tone (empathetic, professional)

- Output:
Improved quality, but sometimes too long or overly verbose

- Observed effect:
Edit time reduced to ~5 minutes

- Lesson learned:
Need length constraint and urgency handling

**v1.2 - Added constraints and urgency logic ✅ Current**

- Change:

Added 150-word limit
Added urgency-specific instructions
Added exclusions (no blame, no legal language)

- Output:
Consistent, professional, and brand-aligned responses

- Observed effect:
Edit time reduced to ~2–3 minutes

- Lesson learned:
Explicit constraints ensure consistent service quality

**📊 A/B Test Results**

Sample: 20 guest complaints (mixed severity)

| Criteria              | v1.0  | v1.2  |
| --------------------- | ----- | ----- |
| Tone appropriateness  | 2.5/5 | 4.8/5 |
| Clarity and structure | 2/5   | 4.7/5 |
| Speed of use          | 1.5/5 | 4.5/5 |
| Need for editing      | High  | Low   |

**🔗 Related Prompts**

Previous: P04 - Complaint triage

Next: P07 - Escalation summary

Related:

→ P03 - Service request response
