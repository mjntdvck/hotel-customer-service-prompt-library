**🏨 P01 · Pre-arrival personalised welcome email (Luxury Hotel – Melbourne)**

**📌 Prompt Text (v1.2 - current)**

Copy this exactly into your AI tool. Replace all [PLACEHOLDERS] before running.

You are a guest experience manager at a 5-star luxury hotel in Melbourne.

Draft a personalised pre-arrival welcome email for a guest named [GUEST_NAME] who has booked a [ROOM_TYPE] from [CHECK_IN_DATE] to [CHECK_OUT_DATE].

Guest profile:
- Booking purpose: [PURPOSE] (e.g. leisure / business / special occasion)
- Special notes: [SPECIAL_REQUESTS] (if none, write "None")

Include the following sections:
1. Warm welcome and appreciation for choosing the hotel
2. Personalised acknowledgement of their purpose of stay (e.g. business trip, anniversary)
3. Summary of booking details (room type, dates)
4. Key pre-arrival information:
   - Check-in time and express check-in option
   - Airport transfer availability
   - Concierge services (restaurant bookings, tours)
5. One personalised recommendation based on guest purpose (e.g. fine dining, local attractions)
6. Offer of assistance before arrival (contact concierge team)

Tone: warm, refined, and professional - aligned with luxury hospitality standards.  
Length: maximum 180 words.  
Do not include: pricing details, internal notes, or operational instructions.

**📊 Placeholders to fill**

| Placeholder          | Source                   | Example          |
| -------------------- | ------------------------ | ---------------- |
| `[GUEST_NAME]`       | Booking system (PMS)     | Mr. Nguyen       |
| `[ROOM_TYPE]`        | PMS reservation          | Deluxe King Room |
| `[CHECK_IN_DATE]`    | PMS                      | 12 April 2026    |
| `[CHECK_OUT_DATE]`   | PMS                      | 15 April 2026    |
| `[PURPOSE]`          | Booking notes / inferred | Anniversary      |
| `[SPECIAL_REQUESTS]` | Guest notes              | Late check-in    |

**🏢 Intended Workflow or Task**

This prompt is Step 1 of the pre-arrival guest communication workflow.

- Trigger: Booking confirmed in Property Management System (PMS)
- Actor: Guest Experience / Front Office team reviews and sends email
- Timing: 48–72 hours before guest arrival

Next step: Follow-up concierge interaction (P02 - personalised itinerary or service upsell)

Booking confirmed → [P01 RUNS] → Staff reviews → Email sent to guest
                                          → Guest replies / concierge engagement
                                          → P02 triggered (if needed)

**❗ Problem Being Solved**
- Front office staff spend approximately 10–15 minutes per guest drafting personalised pre-arrival emails.
- In a 5-star hotel with ~120 arrivals per week:
- This equates to 20–30 hours of manual email drafting per week

Key pain points:
- Inconsistent tone across staff (not always aligned with luxury brand standards)
- Missed opportunities for upselling services (transport, dining, concierge)
- Delayed communication → reduced guest satisfaction before arrival

**⚡ Automation Potential**

**Level: High**

| Dimension               | Assessment                                               |
| ----------------------- | -------------------------------------------------------- |
| Repetitiveness          | High - similar structure across all bookings             |
| Data availability       | All inputs available in PMS                              |
| Human judgment needed   | Low - mainly tone and personalization check              |
| Integration possibility | Can be triggered automatically via PMS + CRM integration |
| Estimated time saving   | ~80% (15 min → 3 min review time)                        |

**Human-in-the-loop role:**
Staff verify guest details and tone alignment before sending. No full rewrite required at v1.2.

**Business impact:**
- Improves response consistency
- Enhances guest experience pre-arrival
- Increases likelihood of upselling concierge services

**⚠️ Risks and Limitations**

| Risk                                                          | Level  | Mitigation                                                                      |
| ------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------- |
| Over-personalisation based on incorrect or missing guest data | Medium | Validate PMS fields before prompt runs; fallback to neutral phrasing if missing |
| Generic output reduces luxury brand perception                | Low    | Prompt includes tone constraints (“refined, luxury hospitality”)                |
| Sensitive guest data exposure                                 | Medium | Limit inputs to non-sensitive booking data; exclude payment details             |
| Inappropriate recommendations for guest purpose               | Low    | Staff review step before sending                                                |

Overall risk rating: LOW–MEDIUM
→ Suitable for near-full automation with light human review.

**🔄 Version History**
**v1.0 - Initial draft**

- Prompt:
Write a welcome email for a hotel guest before arrival.

- Output:
Generic, lacked personalisation, no structure, inconsistent tone

- Observed effect:
Required full rewrite → no time saving

- Lesson learned:
Need role definition + structured sections + guest context

**v1.1 - Added role and structure**

- Change:

Added role (“guest experience manager”)
Added structured sections

- Output:
Improved clarity and tone, but sometimes too long (~250 words)

- Observed effect:
Edit time reduced to ~6–8 minutes

- Lesson learned:
Need word limit + constraints

**v1.2 - Added constraints and personalisation logic ✅ Current**

- Change:

Added 180-word limit
Added personalised recommendation section
Added exclusions

- Output:
Consistent, luxury-level tone, mostly send-ready

- Observed effect:
Edit time reduced to ~2–3 minutes

- Lesson learned:
Constraints + contextual inputs = production-ready outputs

**📊 A/B Test Results**

Sample: 10 guest bookings (mixed purposes)

| Criteria                | v1.0   | v1.2    |
| ----------------------- | ------ | ------- |
| Tone consistency        | 2/5    | 4.6/5   |
| Personalisation quality | 1.5/5  | 4.5/5   |
| Send-ready without edit | 0/5    | 4/5     |
| Average edit time       | 15 min | 2–3 min |

**🔗 Related Prompts**

Next: P02 - Personalised itinerary / concierge upsell

Later chain:

→ Complaint handling

→ Service requests

→ Review response
