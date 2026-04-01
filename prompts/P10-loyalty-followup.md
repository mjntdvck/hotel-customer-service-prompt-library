**🏨 P10 · Loyalty follow-up & retention email (Luxury Hotel – Melbourne)**

**📌 Prompt Text (v1.2 - current)**

Copy this exactly into your AI tool. Replace all [PLACEHOLDERS] before running.

You are a guest experience manager at a 5-star luxury hotel in Melbourne.

Draft a personalised post-stay follow-up email to encourage guest retention and future bookings.

Guest details:
- Guest name: [GUEST_NAME]
- Stay summary: [STAY_SUMMARY] (e.g. 2-night leisure stay, business trip)
- Key experience highlights: [HIGHLIGHTS] (e.g. enjoyed spa, dining, service)
- Issues during stay (if any): [ISSUES] (if none, write "None")

Your email must include:

1. A warm thank-you for the guest’s stay
2. A personalised reference to their experience
3. A subtle reinforcement of positive aspects of the hotel
4. If issues were present:
   - A brief acknowledgement
   - Reassurance of improvement
5. An invitation to return in the future
6. A soft call-to-action (e.g. booking again, contacting directly)

Tone: warm, refined, and relationship-focused - aligned with luxury hospitality standards.  
Style: personalised, not promotional or sales-heavy.  
Length: maximum 180 words.  

Do not include:
- Discounts or pricing unless explicitly provided  
- Generic marketing language  
- Internal operational details

**📊 Placeholders to fill**

| Placeholder      | Source            | Example                          |
| ---------------- | ----------------- | -------------------------------- |
| `[GUEST_NAME]`   | PMS / CRM         | Ms. Tran                         |
| `[STAY_SUMMARY]` | PMS               | 3-night leisure stay             |
| `[HIGHLIGHTS]`   | CRM notes         | Enjoyed spa and fine dining      |
| `[ISSUES]`       | P05 / staff notes | Slow room service on first night |

**🏢 Intended Workflow or Task**

This prompt is the final step in the guest journey, focusing on retention and relationship building.

- Trigger: Guest check-out completed
-Actor: Guest relations / CRM team reviews and sends email
- Timing: Within 24–72 hours after check-out

Next step:
- Guest re-engagement
- Future booking
- CRM retention tracking

Guest check-out → P09 (review response, if applicable)
               → [P10 RUNS] → Email drafted
                              → Staff reviews → Email sent
                              → Guest retention / repeat booking
                              
**❗ Problem Being Solved**
- Guest relations teams spend 5–10 minutes per guest drafting personalised follow-up emails.
- In a luxury hotel with ~150 departures per week:
- This results in 12–25 hours of manual workload weekly

**Key pain points:**
- Generic follow-up emails reduce engagement
- Missed opportunity to build long-term relationships
- Inconsistent handling of guest issues in follow-up communication

**⚡ Automation Potential**

**Level: High**

| Dimension               | Assessment                                      |
| ----------------------- | ----------------------------------------------- |
| Repetitiveness          | High - similar structure across guests          |
| Data availability       | Available from PMS and CRM                      |
| Human judgment needed   | Low–Medium - mainly tone and personalisation    |
| Integration possibility | Can integrate with CRM/email automation systems |
| Estimated time saving   | ~70–80% (10 min → 2–3 min review)               |

**Human-in-the-loop role:**
Staff verify tone and personalisation before sending.

**Business impact:**
- Increased repeat bookings
- Stronger guest relationships
- Improved brand loyalty
- Higher lifetime customer value

**⚠️ Risks and Limitations**

| Risk                                        | Level  | Mitigation                                             |
| ------------------------------------------- | ------ | ------------------------------------------------------ |
| Email feels generic or automated            | Medium | Personalisation using highlights and stay summary      |
| Mishandling of past issues                  | High   | Structured acknowledgement and reassurance             |
| Overly promotional tone damages brand image | Medium | Tone constraint: relationship-focused, not sales-heavy |
| Incorrect guest data used                   | High   | Validate CRM data before prompt execution              |

Overall risk rating: MEDIUM
→ Suitable for near-full automation with light human review

**🔄 Version History**
**v1.0 - Initial draft**

- Prompt:
Write a follow-up email after a hotel stay.

- Output:
Generic, lacked personalisation, too promotional

- Observed effect:
Low engagement → not suitable for luxury brand

- Lesson learned:
Need structured personalisation and tone control

**v1.1 - Added personalisation and structure**

- Change:

Included stay summary and highlights
Added acknowledgment of issues

- Output:
More relevant, but sometimes too long and marketing-heavy

- Observed effect:
Edit time reduced to ~5 minutes

- Lesson learned:
Need tone refinement and constraints

**v1.2 - Added constraints and tone control ✅ Current**

- Change:

Added 180-word limit
Refined tone to relationship-focused
Added exclusions

- Output:
Consistent, personalised, and brand-aligned

- Observed effect:
Edit time reduced to ~2–3 minutes

- Lesson learned:
Tone + structured inputs = effective retention communication

**📊 A/B Test Results**

Sample: 15 guest follow-up scenarios

| Criteria                | v1.0  | v1.2  |
| ----------------------- | ----- | ----- |
| Personalisation quality | 2/5   | 4.7/5 |
| Tone alignment          | 2.5/5 | 4.8/5 |
| Engagement potential    | 2/5   | 4.6/5 |
| Need for editing        | High  | Low   |

**🔗 Related Prompts**

Previous: P09 - Review response

Related:

→ P01 - Pre-arrival welcome email

→ P05 - Complaint response
