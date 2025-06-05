# Sample Walkthrough: Recognizing Patterns Before Structure

This is a high-level walkthrough of how a pattern engine might begin to operate before any formal database or graph structure is in place.

---

## Step 1: Initial Observation

> A child sees a brown, four-legged animal with a wagging tail.

### Pattern Noticed

- Shape: 4 legs, small head, moving tail
- Color: brown
- Motion: wagging tail
- Sound: bark

> These are captured as raw **patterns**.

---

## Step 2: Label Association

> Someone points and says: “Dog.”

### Result

- The system **labels** the observed pattern as `Dog`.

Now a soft association begins to form between the **multi-sensory pattern** and the **word**.

---

## Step 3: Reinforcement

> Over time, the child sees other animals with similar patterns and hears the word "Dog" again.

### Reinforced Pattern

- Pattern group: `{4 legs + wagging tail + bark}` → likely `Dog`

---

## Step 4: Rule Formation (Implicit)

The system now begins to **form generalizations** like:

- “Dog” usually has 4 legs.
- “Dog” may bark.
- “Dog” is not a cat (difference pattern emerging).
  
These aren’t rules in logic—they’re **accumulated probability-weighted patterns**.

---

## Step 5: Anomaly or Correction

> One day the child sees a statue of a dog.

### System Reaction

- Visually matches “Dog” pattern
- No sound, no movement

Possible outcomes:

- Adjust pattern confidence: Not all “Dogs” move or bark.
- Add new sub-pattern: “Some dogs are not alive.”

---

## Step 6: Conflict

> The child is bitten by a dog.

New pattern:

- `Dog` → `Pain`

This introduces a **new pattern link**:

- `Dog` may be `Dangerous`

But this conflicts with:

- `Dog` → `Friendly`

The system now starts to track **contradictory patterns** and context (e.g., *not all dogs are dangerous*).

---

## What This Walkthrough Shows

- The system **accumulates pattern links**, not hard truths.
- Associations are formed from **input and feedback**.
- Contradictions are handled by **splitting contexts** or lowering confidence.
- No graph structure is needed yet—just **recursive pattern registration and comparison**.

---

Next: [Explore the Schema](./db) to see how this is formalized in a Graph and KeyPair database.

---

layout: default
title: Walkthrough Index
---

# 🧪 PET Walkthroughs: From Observation to Belief

This section walks through how PET-based systems evolve understanding through pattern exposure.  
The goal is to illustrate the **steps that occur before and during formal pattern encoding** in the schema.

---

## 🧭 High-Level Stages of Pattern Development

PET walks through the world like a child learning to name and relate what it sees. The stages below form the cognitive arc:

### 1. Observation  
>
> A pattern is received via one or more sensory inputs (e.g., visual, audio, tactile).  
Patterns: shape, color, sound, motion...

### 2. Association  
>
> A label or name is applied (e.g., “Dog”) — sometimes guessed, sometimes taught.

### 3. Reinforcement  
>
> The same pattern shows up repeatedly — strengthening the label.

### 4. Generalization  
>
> The system starts noticing shared properties across similar patterns and begins forming implicit categories.

### 5. Anomaly or Contradiction  
>
> A new input violates the assumed pattern (e.g., a dog statue). The system adjusts confidence or context.

### 6. Conflict and Refinement  
>
> Conflicting experiences (e.g., Dog → Friendly vs Dog → Pain) force the system to split contexts or downgrade beliefs.

---

## 🔍 Browse the Example Gallery

To see how these stages appear in real scenarios:

- [Walkthrough Gallery](./gallery.md)

Scenarios include:

- Recognizing a face
- Learning “Dog = Dangerous”
- Rewriting beliefs after new experiences
- Recursive conflict resolution in belief systems

---

## 📘 Next Steps

Once familiar with how raw patterns become beliefs, [Explore the Schema](../schema/) to see how this is structured using nodes, edges, and understanding history.
