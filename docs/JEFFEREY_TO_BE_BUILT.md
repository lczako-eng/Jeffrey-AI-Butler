# JEFFEREY AI — "To Be Built" Specification

**Document:** Build Specification v1.0 (Draft — Founder's Addendum pending)
**Project:** JEFFEREY — The Personal Shadow AI (Project JBX)
**Author:** Laszlo Czako
**Date:** August 2026
**Status:** TO BE BUILT — this document defines the next implementation phase.

---

## 1. The Core Design Principle

Everything in this specification flows from one rule:

> **JEFFEREY's primary objective is to continuously improve the user's life according to the user's own priorities — not merely answer prompts.**

Most AI companies optimize for *responding*. JEFFEREY optimizes for **representing you**.

This is a fiduciary-style product philosophy (a philosophy, not a legal claim): an AI whose default objective is to act in the user's best interest *as the user has defined it*. People will not trust JEFFEREY because it is intelligent — intelligence is becoming a commodity. They will trust it because its behavior is **predictable, transparent, and aligned with their values**.

Trust is a measurable design goal, built from four properties:

| Property | Meaning |
|---|---|
| **Transparent** | "Here's why I recommended this." |
| **Permission-based** | "I won't act outside the permissions you've given me." |
| **Correctable** | "If I misunderstood your priorities, tell me once and I'll learn." |
| **Loyal** | "I optimize for your interests — not an advertiser's, an affiliate commission, or another company's objectives." |

**Mission statement:**

> JEFFEREY exists to earn your trust by continuously working in your best interests, according to your values, while always leaving you in control.

**The product test:** If JEFFEREY disappeared tomorrow, would the user feel like they had lost someone who was quietly looking out for them? That is a much higher bar than "would they miss a chatbot?"

---

## 2. Positioning — The Permanent Personal Layer

JEFFEREY does not compete with Claude, ChatGPT, Gemini, or future models. It becomes **the user's permanent layer that sits above whichever model is best at the moment**.

```
                Jeff
     (Conscience + Memory + Orb)
                  │
      ┌───────────┼───────────┐
      │           │           │
   ChatGPT     Claude      Future AI
```

If a better foundation model appears five years from now, the user doesn't lose who Jeff is. Jeff keeps:

- their memories,
- their priorities,
- their personality profile,
- their long-term history,

…and simply uses whichever AI engine is best for the task.

This avoids competing head-on with companies spending tens of billions on foundation models. Jeff becomes the **persistent personal layer that users own**, regardless of which AI engine powers the conversation underneath.

**Platform AI vs. JEFFEREY:**

| Platform AI | JEFFEREY |
|---|---|
| Optimizes for the platform's objectives | Optimizes for one person |
| May prioritize engagement, subscriptions, ecosystem growth | Learns that person's priorities |
| Serves millions of users with one general policy | Explains its reasoning; acts only within permissions; seeks long-term trust |

**The product promise, in one sentence:**

> "JEFF doesn't just remember what you like. It learns *why* you make decisions — and gets better at representing you over time."

---

## 3. Core Architecture — Six Building Blocks

Every capability plugs into the same core. Nothing is a disconnected feature.

### Block 1 — The Conscience Engine *(the heart of the system)*

- Learns user **priorities** (not preferences).
- Explains *why* it made decisions.
- Accepts corrections and learns from them.
- Updates confidence over time.
- Stores long-term values.

**Everything else depends on this.**

The key insight: **Jeff shouldn't learn preferences. It should learn priorities.**

| Preferences (easy to copy) | Priorities (deep — explain *why*) |
|---|---|
| Likes blue | Safety > Cost |
| Prefers steak | Family > Career |
| Uses Gmail | Privacy > Convenience |
| | Time > Money |
| | Reliability > Lowest price |

Two required refinements:

1. **Confidence scores.** Every learned priority carries a confidence value, and Jeff exposes it: *"I'm only 60% confident that you'd rather save money in this situation. Should I update that?"* This makes learning transparent instead of mysterious.
2. **Contextual priorities.** Priorities are not one fixed ranking; they depend on domain:
   - Business travel: Time > Money
   - Personal shopping: Money > Convenience
   - Family health: Safety > Everything
   - Pet care: Animal welfare > Cost

### Block 2 — The Memory Engine

- Stores **facts separately from values**.
- Keeps long-term context.
- Lets the user **inspect, edit, and delete** memories.

### Block 3 — The Opportunity Engine *(the proactive core — see §4)*

- Continuously looks for ways to improve the user's life based on learned priorities.
- Watches, monitors, and detects — even while the user sleeps.
- Scores and ranks every opportunity before surfacing it.

### Block 4 — The Action Engine

- Books reservations, cancels subscriptions, pays bills (with authorization), calls businesses, writes emails, executes tasks.
- Governed by three **permission levels**:

| Level | Behavior |
|---|---|
| **Observe** | Jeff watches and suggests only. |
| **Recommend** | Jeff brings opportunities to the user for approval. |
| **Act** | Jeff carries out approved categories of tasks automatically, within limits the user has set. |

### Block 5 — The Orb Interface

- Visualizes Jeff's internal state: confidence, thinking, emotion, attention.
- Makes the AI feel **present**, not just conversational.
- The brand anchor: Apple had the click wheel, Tesla the center screen — the Orb is what people will associate with Jeff. It shouldn't just animate; it should **communicate** (happy, thinking, protective, concerned, curious) so the user eventually knows what Jeff is feeling without reading words.

### Block 6 — Self-Cloud

- Gives the user **ownership** of memory, identity, and conscience.
- Allows different AI models to access the same personal memory — only with the user's permission.
- The foundation of physical sovereignty; introduced fully after product demand is proven.

---

## 4. The Opportunity Engine — Proactive by Design

Most AI today is reactive: you ask, it answers, the conversation ends. JEFFEREY is **goal-driven**: it is quietly working toward goals the user has approved — not waiting for prompts.

### The internal loop

1. What are this person's long-term goals?
2. Has anything changed in the world?
3. Does that change create an opportunity or reduce a risk?
4. Can I act within the permissions I've been given?
5. If not, what's the best recommendation to present?

### The daily question

Every day, Jeff asks itself: **"What can I do today to make this person's life better?"** — across everything the user has said matters: money, health, time, family, pets, business, travel, privacy, happiness. Because Jeff knows the user's priorities, it doesn't optimize for everyone. **It optimizes for you.**

### Opportunity scoring

Every piece of information Jeff sees gets scored:

- Is this important? Is it urgent?
- Does it align with the user's priorities?
- Can it save meaningful money or time?
- Does it reduce risk? Improve health, wellbeing, or happiness?
- Does it advance one of the user's stated goals?
- Is it important enough to interrupt the user?
- Can Jeff handle it automatically, or should it ask first?

Opportunities are then ranked and presented, e.g.:

```
Today's Opportunities
★★★★★  Mortgage renewal available — potential savings $12,400
★★★★★  Customer hasn't paid invoice — follow-up recommended
★★★★☆  New flight price — save $380
★★★☆☆  Insurance comparison — save $190
★★☆☆☆  Gym membership unused
```

### Worked example

**Goal: "Reduce my monthly expenses by 15%."** Jeff then monitors subscriptions, notices the phone contract expires next month, watches airfare for an upcoming trip, detects a better insurance rate, finds a lower mortgage rate near renewal, notices underused cloud storage, suggests consolidating streaming services — and reports: *"I found three changes that save you $1,420/year. Would you like me to handle them?"*

That feels less like a chatbot and more like a **trusted representative**.

### Domain examples

- **Travel** — watches airfare after the user names a destination; knows whether they value direct flights, low cost, or loyalty; alerts only on matches; prepares the booking for approval if authorized.
- **Entertainment** — learns favorite artists; notices concert announcements; watches presales; warns before prices spike or tickets sell out.
- **Money** — cheaper subscriptions, duplicate services, insurance renewals, refinancing aligned with goals.
- **Health** — notices long working hours; reminds the user of *their own* stated goals; suggests changes based on what the user said matters.

### The interrupt rule

> **JEFFEREY doesn't interrupt — it earns the right to interrupt.**

If Jeff interrupts, it is because it found something genuinely important *according to the user's priorities*. This keeps proactivity from becoming noise.

---

## 5. The Signature Interaction

The behavior to optimize for is not "AI that answers questions" but **AI that learns the reasons behind your corrections**.

**Traditional AI:**
> "Here are the three cheapest phone plans."

**Jeff:**
> "I didn't recommend the cheapest plan because over the last year you've consistently chosen reliability over saving $15/month. You also travel to the U.S. frequently, so I weighted roaming more heavily. If that's no longer your priority, tell me and I'll update what I've learned."

Every recommendation must be explainable in terms of the user's own goals and values — never hidden incentives. If Jeff says *"I found a cheaper insurance policy,"* it must also be able to say *"…because you've consistently prioritized reliability over the lowest price, and this option maintains the same coverage while saving you $240/year."*

**The feature filter:** every proposed feature must answer one question — *"Does this make JEFFEREY a more trustworthy representative of the user?"* If yes, it belongs. If no — even if technically impressive — it is not part of the core mission.

---

## 6. Build Priorities

Do **not** build all patent claims at once. The MVP proves the one thing that makes people say: *"I've never seen AI work like that."*

| Priority | Area | Why |
|---|---|---|
| 1 | **Digital Conscience** | The core differentiator. It learns *who the user is*, not just what they ask. |
| 2 | **Priority-Based Learning** | What makes the conscience useful — it learns what matters *most*, with confidence and context. |
| 3 | **Operational AI** | Jeff actually accomplishes tasks on the user's behalf. |
| 4 | **Emotional Orb** | The visual identity people will remember. |
| 5 | **Physical Sovereignty / Self-Cloud** | Extremely important — introduced after demand is proven. |
| 6 | **Digital Inheritance** | Compelling long-term feature, not the first thing users need to experience. |

---

## 7. Phase 1 — The Demo (2–4 weeks)

This is the part to show investors.

**Scene 1 — The Conscience moment.** The user opens Jeff for the first time. The orb appears. It says:

> "I've noticed over the last month you've corrected me 19 times.
> I think I finally understand something important.
> Time with your family matters more to you than saving money."

Then it explains **why** it learned that. This demonstrates the Digital Conscience concept far more powerfully than a list of features.

**Scene 2 — Consent.** Jeff asks: *"Should I remember this forever?"* When the user says yes, Jeff updates its own conscience. **That's the moment your AI becomes *their* AI.**

**Scene 3 — Operational AI.** Jeff uses that knowledge. Instead of *"Here are five flights,"* Jeff says:

> "I didn't book the cheapest flight because you consistently choose direct flights over saving $180."

An explanation grounded in learned priorities — fundamentally different from generic personalization.

**Scene 4 — The Orb.** The orb communicates state throughout: happy, thinking, protective, concerned, curious.

### The single KPI for Version 1

> **Does the user feel that Jeff knows them better after 30 days than any other AI?**

If yes, the heart of the vision is demonstrated. Everything else — Self-Cloud, digital inheritance, operational authority, licensing, enterprise versions — builds on that foundation.

### Build method

Use AI coding agents the way a software company uses engineers, in parallel:

- one agent builds the memory engine,
- one builds the orb,
- one builds authentication,
- one builds integrations,
- one writes tests,
- one reviews code.

The hard parts are not writing code: they are user experience design, model/service integration, authentication, payments and security, testing, and refinement with real users. The part that is hardest to copy is not the code — it is the **coherent product vision** tying together persistent identity, value learning, user ownership, operational capability, and a consistent interface and brand.

---

## 8. Category Statement

The ambition is not "personal AI" or "another chatbot." The category is:

> **A digital companion that develops its own understanding of you over years.**

The vision, restated:

> JEFFEREY is your lifelong AI representative. It continuously learns your values, proactively works to improve your life, and acts only in your best interests within the permissions you choose.

A note on the "friend" framing: a good friend doesn't try to control you or replace your relationships. A good friend remembers what's important to you, tells you uncomfortable truths respectfully, celebrates your successes, and quietly has your back. That is the healthier, sustainable implementation of companionship — not making the AI seem human.

---

## 9. Founder's Addendum (Reserved)

*This section is reserved for the founder's forthcoming twist on the concepts above. It will be incorporated as v1.1 of this specification before implementation begins.*

---

© 2026 Laszlo Czako. All rights reserved.
This document is part of the Project JBX / JEFFEREY concept record and extends the existing architecture declaration (`docs/architecture.md`) and whitepaper corpus.
