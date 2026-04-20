# Daily Reflection Tree — Design Write-up

## 1. Objective

The goal of this assignment was to design a **deterministic reflection system** that helps an employee analyze their day through a structured conversation.

Unlike LLM-based systems, this design ensures:

* Predictability
* Consistency
* Auditability

The system uses a **decision tree** where every path is predefined, and every user choice leads to a known outcome.

---

## 2. Core Design Philosophy

The reflection tree is designed as a **guided conversation, not a survey**.

Key principles:

* Questions should feel natural and relatable
* Options should represent real thought patterns
* Reflections should reframe thinking without judgment
* The flow should gradually deepen awareness

The structure ensures that users **arrive at insights themselves**, instead of being told what to think.

---

## 3. The Three Axes of Reflection

The entire tree is built around three psychological dimensions:

---

### Axis 1: Locus of Control (Victim ↔ Victor)

This axis captures whether the user perceives events as:

* **External (Victim mindset)** — things happened to them
* **Internal (Victor mindset)** — they influenced outcomes

**Design approach:**

* Start with a general emotional question (“How was your day?”)
* Branch into different follow-ups based on tone (positive vs difficult)
* Add a second layer question to capture behavior after events

**Goal:**
Help users recognize **their role in outcomes**, even in difficult situations.

---

### Axis 2: Orientation (Entitlement ↔ Contribution)

This axis captures whether the user is focused on:

* **What they received (Entitlement)**
* **What they gave (Contribution)**

**Design approach:**

* Ask about a specific moment from the day
* Separate “helping behavior” from “expectation mindset”
* Add follow-up questions to deepen intent (why they acted that way)

**Goal:**
Shift attention from outcomes to **value creation and contribution**.

---

### Axis 3: Radius of Concern (Self ↔ Others)

This axis captures how wide the user’s perspective is:

* **Self-focused** — personal stress, workload
* **Others-focused** — team, colleagues, customers

**Design approach:**

* Start with “who comes to mind first”
* Branch into deeper questions about impact and consideration
* Highlight perspective-taking

**Goal:**
Encourage users to move toward **broader awareness and meaning**.

---

## 4. Tree Structure and Flow

The tree follows a strict sequence:

1. **Axis 1 (Control Awareness)**
2. **Axis 2 (Contribution Orientation)**
3. **Axis 3 (Perspective Expansion)**
4. **Summary (Synthesis)**

This progression is intentional:

* Awareness of control enables responsibility
* Responsibility enables contribution
* Contribution enables broader perspective

Each axis builds on the previous one, creating a **coherent reflection journey**.

---

## 5. Branching Logic

The system uses **decision nodes** to route users based on their responses.

Example:

* Positive vs negative day → different follow-up questions
* Helping vs expectation → different reflection paths
* Self vs others → different perspective reflections

This ensures:

* Relevant follow-up questions
* Personalized (but deterministic) experience
* Meaningful reflections based on actual choices

---

## 6. Use of Signals

Each node can assign a **signal** such as:

* `axis1:internal`
* `axis2:contribution`
* `axis3:others`

These signals:

* Track user tendencies
* Enable structured interpretation
* Can be extended for analytics or scoring (if needed)

The system avoids complex modeling and uses **simple, transparent tagging**.

---

## 7. Reflection Design

Reflection nodes are critical to the experience.

Design principles:

* Non-judgmental tone
* Acknowledge current state
* Gently introduce an alternative perspective

Examples:

* Instead of blaming, highlight “small choices”
* Instead of criticizing, suggest “where you could contribute”
* Instead of forcing change, expand awareness

The goal is **insight, not evaluation**.

---

## 8. Summary Design

The summary node uses **interpolation**:

* References user’s earlier answers
* Reconstructs their reflection path
* Reinforces key behavioral patterns

Example:

* “You described your day as…”
* “You responded by…”
* “You focused on…”

This creates a **personalized closing reflection** without using AI.

---

## 9. Trade-offs and Design Decisions

### 1. Depth vs Simplicity

* Chose moderate depth (30+ nodes)
* Avoided excessive branching to keep flow manageable

### 2. Realism vs Coverage

* Focused on realistic options instead of exhaustive possibilities
* Ensured each option is meaningfully distinct

### 3. Determinism vs Personalization

* No free text or AI interpretation
* Personalization achieved through branching and interpolation

---

## 10. Improvements with More Time

If extended further, I would:

* Add more nuanced intermediate states (not just binary splits)
* Introduce weighted signals for stronger summary insights
* Create multiple reflection styles (short vs deep)
* Build a visual UI for better user experience
* Add session history tracking for longitudinal insights

---

## 11. Conclusion

This reflection tree demonstrates how **human psychological frameworks can be translated into deterministic systems**.

By structuring questions, decisions, and reflections into a tree:

* Ambiguity is reduced
* Insight is preserved
* Experience remains consistent

This approach aligns with the idea of **knowledge engineering** — converting abstract human understanding into structured, navigable systems.

---

**THANK YOU**
