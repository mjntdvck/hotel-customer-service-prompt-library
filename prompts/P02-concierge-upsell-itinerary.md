**🏨 P02 · Concierge upsell & personalised itinerary (Luxury Hotel - Melbourne)**

**📌 Prompt Text (v1.2 - current)**

Copy this exactly into your AI tool. Replace all [PLACEHOLDERS] before running.

You are a concierge specialist at a 5-star luxury hotel in Melbourne.

Create a personalised pre-arrival itinerary and soft upsell recommendations for a guest named [GUEST_NAME].

Guest details:
- Stay dates: [CHECK_IN_DATE] to [CHECK_OUT_DATE]
- Purpose of stay: [PURPOSE] (e.g. leisure / business / anniversary)
- Interests: [INTERESTS] (e.g. fine dining, shopping, culture, nightlife)
- Special requests: [SPECIAL_REQUESTS] (if none, write "None")

Your output must include:

1. A 2-day suggested itinerary tailored to the guest's purpose and interests:
   - Day 1 (arrival day): light activities
   - Day 2: main experiences
   (Use bullet points)

2. 2-3 personalised concierge recommendations (e.g. restaurants, tours, experiences in Melbourne)

3. Subtle upsell suggestions:
   - Airport transfer
   - Restaurant reservations
   - Premium experiences (e.g. wine tours, spa)

Tone: refined, personalised, and aligned with luxury hospitality standards.  
Style: concierge-style, not sales-heavy - recommendations should feel helpful, not pushy.  
Length: maximum 220 words.  
Do not include: pricing, internal notes, or overly promotional language.

**📊 Placeholders to fill**

| Placeholder          | Source         | Example                    |
| -------------------- | -------------- | -------------------------- |
| `[GUEST_NAME]`       | PMS booking    | Ms. Tran                   |
| `[CHECK_IN_DATE]`    | PMS            | 10 May 2026                |
| `[CHECK_OUT_DATE]`   | PMS            | 12 May 2026                |
| `[PURPOSE]`          | Booking notes  | Leisure                    |
| `[INTERESTS]`        | CRM / inferred | Fine dining, art galleries |
| `[SPECIAL_REQUESTS]` | PMS notes      | Early check-in             |

**🏢 Intended Workflow or Task**

This prompt is Step 2 of the pre-arrival guest engagement workflow, following P01.
- Trigger: Guest receives pre-arrival email (P01) or engages with concierge
- Actor: Concierge team reviews and sends personalised itinerary
- Timing: 24–48 hours before arrival (or upon guest request)

Next step: Guest confirms bookings → reservations made (restaurants, transport, tours)

P01 (Welcome email) → Guest engagement → [P02 RUNS]
                                     → Concierge reviews → Itinerary sent
                                     → Guest confirms → Bookings executed
**❗ Problem Being Solved**
- Concierge staff spend approximately 15-20 minutes per guest crafting personalised itineraries and recommendations.
- In a luxury hotel with ~80 concierge requests per week:
- This results in 20–27 hours of manual work weekly

**Key pain points:**
- Inconsistent quality of recommendations depending on staff experience
- Missed upselling opportunities (premium services not suggested)
- Slow response times during peak periods

**⚡ Automation Potential**
**Level: Medium-High**

| Dimension               | Assessment                                                |
| ----------------------- | --------------------------------------------------------- |
| Repetitiveness          | Medium - structure is similar but content varies          |
| Data availability       | Moderate - depends on guest profile completeness          |
| Human judgment needed   | Medium - recommendations must be accurate and appropriate |
| Integration possibility | Can integrate with CRM + concierge booking systems        |
| Estimated time saving   | ~60-70% (20 min → 6-8 min including review)               |

**Human-in-the-loop role:**
Concierge validates recommendations (availability, suitability, timing) before sending.

**Business impact:**
Increased upsell conversion (transport, dining, experiences)
Higher guest satisfaction through personalisation
More efficient concierge operations

**⚠️ Risks and Limitations**
| Risk                                                | Level  | Mitigation                                       |
| --------------------------------------------------- | ------ | ------------------------------------------------ |
| Recommendations inaccurate or unavailable           | Medium | Concierge verifies availability before sending   |
| Generic or irrelevant suggestions                   | Medium | Use structured guest inputs (purpose, interests) |
| Overly sales-focused tone damages luxury experience | Low    | Prompt enforces “not sales-heavy” tone           |
| Missing guest data leads to weak personalisation    | Medium | Use fallback neutral recommendations             |

**Overall risk rating: MEDIUM**
→ Requires human validation before guest-facing use.

**🔄 Version History**
**v1.0 - Initial draft**

- Prompt:
Suggest things for a hotel guest to do in Melbourne.

- Output:
Generic tourist suggestions, no structure, no personalisation

- Observed effect:
Not usable for luxury concierge service → full rewrite required

- Lesson learned:
Need role + guest context + structured itinerary

**v1.1 - Added structure and guest context**

- Change:

Added concierge role
Added itinerary structure (Day 1 / Day 2)
Included guest purpose and interests

- Output:
More relevant and structured, but sometimes too long and slightly promotional

- Observed effect:
Edit time reduced to ~8–10 minutes

- Lesson learned:
Need constraints on tone and length

**v1.2 - Added tone control and constraints ✅ Current**

- Change:

Added “not sales-heavy” tone constraint
Added 220-word limit
Clarified upsell as “subtle recommendations”

- Output:
Consistent, personalised, luxury-standard content

- Observed effect:
Edit time reduced to ~5-7 minutes

- Lesson learned:
Tone constraints are critical in luxury hospitality contexts

**📊 A/B Test Results**

Sample: 8 concierge scenarios (different guest profiles)

| Criteria                   | v1.0  | v1.2  |
| -------------------------- | ----- | ----- |
| Personalisation quality    | 2/5   | 4.5/5 |
| Relevance to guest profile | 2.5/5 | 4.6/5 |
| Tone (luxury standard)     | 2/5   | 4.7/5 |
| Usability without edits    | 0/5   | 3.5/5 |

**🔗 Related Prompts**

Previous in chain: P01 - Pre-arrival welcome email

Next (optional): P03 - Service request handling

Related:

→ P09 - Review response

→ P10 - Loyalty follow-up
