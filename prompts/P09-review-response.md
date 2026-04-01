**🏨 P09 · Guest review response (Luxury Hotel – Melbourne)**

**📌 Prompt Text (v1.2 - current)**

Copy this exactly into your AI tool. Replace all [PLACEHOLDERS] before running.

You are a guest relations manager at a 5-star luxury hotel in Melbourne.

Draft a professional public response to a guest review.

Review details:
- Guest name (if available): [GUEST_NAME]
- Review type: [REVIEW_TYPE] (Positive / Negative)
- Review content: [REVIEW_TEXT]

Your response must include:

For ALL reviews:
1. A polite acknowledgement and appreciation for feedback
2. A personalised reference to the guest’s experience

If review is Positive:
3. Reinforce positive aspects mentioned
4. Invite the guest to return

If review is Negative:
3. A sincere apology (if applicable)
4. Acknowledgement of specific issue(s)
5. Reassurance of improvement or follow-up action
6. A professional closing inviting further contact offline

Tone: professional, courteous, and aligned with luxury hospitality standards.  
Style: concise, personalised, and brand-protective.  
Length: maximum 140 words.  

Do not include:
- Defensive language  
- Blame toward guest or staff  
- Internal operational details

**📊 Placeholders to fill**

| Placeholder     | Source          | Example                                               |
| --------------- | --------------- | ----------------------------------------------------- |
| `[GUEST_NAME]`  | Review platform | John                                                  |
| `[REVIEW_TYPE]` | Classification  | Negative                                              |
| `[REVIEW_TEXT]` | Review content  | "The service was slow and staff seemed unresponsive." |

**🏢 Intended Workflow or Task**

This prompt is part of the post-stay reputation management workflow.

- Trigger: Guest leaves review on platform (Google, TripAdvisor, Booking.com)
- Actor: Guest relations / marketing team reviews and posts response
- Timing: Within 24–48 hours of review

Next step:
- Monitor follow-up
- Internal feedback loop (improvement actions)
- Potential re-engagement (P10)
Guest leaves review → [P09 RUNS] → Draft response generated
                                   → Staff reviews → Response published
                                   → Feedback loop to operations
                                   → P10 follow-up (optional)

**❗ Problem Being Solved**
- Guest relations teams spend 5–8 minutes per review crafting responses.
- In a hotel receiving ~40–60 reviews per week:
- This results in 3–8 hours of manual effort weekly

Key pain points:
- Inconsistent tone across responses
- Poor handling of negative reviews → reputational damage
- Generic responses reduce perceived authenticity

**⚡ Automation Potential**

Level: High

| Dimension               | Assessment                                 |
| ----------------------- | ------------------------------------------ |
| Repetitiveness          | High - structured response patterns        |
| Data availability       | Always available (review content)          |
| Human judgment needed   | Medium - tone and brand alignment          |
| Integration possibility | Can integrate with review management tools |
| Estimated time saving   | ~70–80% (8 min → 2 min review)             |

**Human-in-the-loop role:**
Staff verify tone, accuracy, and appropriateness before publishing.

**Business impact:**
- Improved online reputation
- Higher guest trust and engagement
- Faster response times
- Increased likelihood of repeat bookings

**⚠️ Risks and Limitations**

| Risk                                              | Level  | Mitigation                           |
| ------------------------------------------------- | ------ | ------------------------------------ |
| Generic responses reduce authenticity             | Medium | Prompt enforces personalisation      |
| Poor handling of negative reviews escalates issue | High   | Structured apology + response format |
| Inappropriate tone damages brand image            | High   | Mandatory staff review               |
| Disclosure of internal issues publicly            | High   | Explicit exclusion rules             |

Overall risk rating: MEDIUM–HIGH
→ Requires human validation before publishing

**🔄 Version History**

**v1.0 - Initial draft**

- Prompt:
Reply to a hotel review.

- Output:
Generic, lacked structure, weak handling of negative feedback

- Observed effect:
Not suitable for brand-facing communication

- Lesson learned:
Need conditional structure (positive vs negative)

**v1.1 - Added conditional logic**

- Change:

Separate handling for positive vs negative reviews
Added apology structure

- Output:
Improved responses but sometimes too long

- Observed effect:
Edit time reduced to ~4 minutes

- Lesson learned:
Need length constraint and tone refinement

**v1.2 - Added constraints and tone control ✅ Current**

- Change:

Added 140-word limit
Refined tone to “brand-protective”
Added exclusions

- Output:
Consistent, professional, and suitable for public platforms

- Observed effect:
Edit time reduced to ~1–2 minutes

- Lesson learned:
Conditional logic + constraints ensure brand-safe responses

**📊 A/B Test Results**

Sample: 20 guest reviews (mixed sentiment)

| Criteria                      | v1.0  | v1.2  |
| ----------------------------- | ----- | ----- |
| Tone appropriateness          | 2.5/5 | 4.8/5 |
| Handling of negative feedback | 2/5   | 4.7/5 |
| Personalisation               | 2/5   | 4.6/5 |
| Publish-ready                 | Low   | High  |

**🔗 Related Prompts**

Next: P10 - Loyalty follow-up

Related:

→ P05 - Complaint response

→ P07 - Escalation summary
