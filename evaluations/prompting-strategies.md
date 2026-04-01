**# ⚙️ Prompting Strategies**

This prompt library applies a set of structured prompting strategies to ensure outputs are consistent, reliable, and suitable for real-world hotel operations in a 5-star luxury context.

Each strategy is selected based on the nature of the workflow (customer-facing, operational, or management-level) and the level of automation required.

---

## 1. RACE Framework (Role - Action - Context - Expectation)

**Prompts:** P01, P02, P03, P05, P09, P10  

The RACE framework is used to ensure clarity and consistency in natural language outputs.

- **Role:** Defines the perspective (e.g. guest relations manager, concierge, front desk)
- **Action:** Specifies the task (e.g. draft email, respond to complaint)
- **Context:** Provides business and guest details
- **Expectation:** Defines output structure, tone, and constraints

**Why used:**
Customer-facing communication requires consistent tone, structure, and professionalism, especially in luxury hospitality.

**Impact:**
- Reduced variability in tone and structure  
- Improved brand consistency  
- Higher “send-ready” output rate  

---

**## 2. Structured Output Constraints**

**Prompts:** All prompts  

All prompts include explicit constraints such as:
- Word limits (e.g. 120-180 words)
- Required sections (e.g. apology, acknowledgement, next steps)
- Tone instructions (e.g. “refined”, “empathetic”, “not sales-heavy”)

**Why used:**
Unconstrained prompts often produce verbose or inconsistent outputs that require manual editing.

**Impact:**
- Outputs become production-ready  
- Reduced editing time (up to ~80%)  
- Improved operational efficiency  

---

## 3. Conditional Logic (Rule-Based Prompting)

**Prompts:** P03, P05, P08, P09  

Prompts include conditional instructions such as:
- If urgency is High → adjust tone and response  
- If availability is Limited → offer alternatives  
- If review is Negative → include apology and reassurance  

**Why used:**
Real-world service workflows require different responses based on context and conditions.

**Impact:**
- More context-aware responses  
- Reduced need for human rewriting  
- Improved service quality and consistency  

---

## 4. JSON Output for System Integration

**Prompts:** P04  

P04 uses structured JSON output to enable machine-readable results:

```json
{
  "category": "...",
  "urgency": "...",
  "summary": "...",
  "reason": "..."
}
```
**Why used:**
The output must integrate with CRM or ticketing systems for automated routing.

**Impact:**

- Enables full automation of complaint triage
- Eliminates manual classification work
- Supports real-time system integration

**5. Grounding Constraints (Anti-Hallucination)**

**Prompts:** P06, P07

Prompts include explicit instructions such as:

- “Use ONLY the information provided”
- “Do not infer or assume”
- “If data is missing, state: Insufficient data”

**Why used:**
Operational and incident reporting requires factual accuracy and has legal implications.

**Impact:**

- Eliminates hallucinated information
- Improves reliability in high-risk contexts
- Supports compliance and auditability

**6. Tone Control and Brand Alignment**

**Prompts:** P01, P02, P03, P05, P08, P09, P10

All customer-facing prompts include strict tone requirements:

- “Luxury hospitality standard”
- “Warm, refined, professional”
- “Not defensive / not overly promotional”

**Why used:**
Inconsistent tone can damage brand perception, especially in a 5-star hotel environment.

**Impact:**

- Maintains consistent brand voice
- Enhances guest experience
- Reduces reputational risk

**7. Explicit Exclusion Rules**

**Prompts:** P01, P05, P08, P09, P10

Prompts explicitly define what must NOT be included:

- Pricing or discounts
- Internal operational details
- Legal or defensive language

**Why used:**
AI models may introduce irrelevant or inappropriate content if not constrained.

**Impact:**

- Prevents sensitive or inappropriate outputs
- Improves safety and compliance
- Reduces need for post-editing

**8. Workflow Chaining Design**

**Prompts:** All (system-level design)

Prompts are designed to work as part of a connected workflow:

P01 → P02 (Pre-arrival)
P03 → P08 → P07 (In-stay service)
P04 → P05 → P07 (Complaint handling)
P06 → P07 (Incident management)
P09 → P10 (Post-stay)

**Why used:**

Individual prompts are less valuable than a coordinated system that supports end-to-end operations.

**Impact:**

- Enables automation across the full guest journey
- Improves operational efficiency
- Aligns AI outputs with real business processes

**Summary**

This prompt library combines structured prompting techniques, conditional logic, system integration, and governance controls to deliver reliable and scalable AI-assisted workflows.

The strategies ensure that outputs are not only linguistically correct, but also operationally useful, brand-aligned, and safe for deployment in a real-world luxury hotel environment.
---
