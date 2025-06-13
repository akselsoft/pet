---
title: Advanced Pattern Evaluation (Schema Version)
layout: default
description: Full example of PET pattern evaluation using ON, PN, UP, and CUG terms
---

# 🧠 Advanced Pattern Evaluation (Node-Based Schema)

This schema-based example walks through how a PET system interprets a recurring set of patterns using the same initial [example](../evaluation-advanced) and the formal architecture:

- **ON** — Object Node
- **PN** — Pattern Node
- **UP** — Understanding Pattern
- **SPN** — Sub-Pattern Node
- **CUG** — Current Understanding Graph
- **HUG** — Historical Understanding Graph

---

## 🐕 Example Scenario: “Dog Licks Boy in Park”

---

### Day 1

- **Input**: Sight engine reports a composite signal of `Dog licks boy in park`.
- **PN1** is generated and linked to 4 **SPNs**: `Dog`, `Lick`, `Boy`, `Park`.
- **SPNs** are converted (or linked) to **ONs**.
- These ONs are bound by a relationship edge set (EN).
- A new **UP1** is formed in the **CUG**:
  - PN1 + {ON_Dog, ON_Lick, ON_Boy, ON_Park}
  - Trust initialized (100%)
  - Evaluation: `UP1 => Exists`

---

### Day 2

- **PN2** with `Dog licks boy on street` is input.
- SPNs extracted: `Dog`, `Lick`, `Boy`, `Street`
- All match existing ONs except `Street` (new ON added)
- **PN2** evaluated as similar to UP1.
- Reinforces **UP1**:
  - Trust level increases
  - Edge added for location variance
- No new UP is created. PN2 is archived in HUG, referenced by UP1.

---

### Day 3

- **PN3** with `Dog licks boy in park` again.
- Full match with UP1 and ON set.
- Reinforcement increases further.
- No contradiction or ambiguity.
- Archived in HUG.

---

### Day 4 – Contradiction

- **PN4**: `Dog bites boy in car`
- ONs: Dog, Bite (new), Boy, Car (new)
- Mapped to new **UP2** in CUG:
  - Represents contradiction to UP1
- Recursion Engine activates:
  - Evaluates impact on UP1:
    - Location (car vs. park)
    - Action (bite vs. lick)
  - Partial overlap with ONs (Dog, Boy)
  - Adjusts trust in UP1
  - Lick re-evaluated across UPs and ONs

---

## 🧠 Recap of Node Dynamics

| Element | Description |
|--------|-------------|
| **PN** | Individual pattern instance |
| **ON** | Canonical object/action node |
| **UP** | Generalized pattern of understanding |
| **SPN** | Extracted sub-nodes from sensor input |
| **EN** | Edges that bind ONs in a relational context |
| **CUG** | Graph of current trusted UPs |
| **HUG** | Archive of past PN evaluations |

---

## 🧠 Concept Refinement from Contradictions

“Lick” is now connected across:

- `Dog licks boy` (affection)
- `Tiger licks cub` (grooming)
- `Dog licks wound` (healing)
- `Team licks opponent` (domination)

From these:

- `Lick` ON forms higher abstraction:
  - → Affection (exists)
  - → Grooming (exists)
  - → Domination (context-dependent)

---

## 🧭 Summary

- Every PN contributes to memory (HUG) and may refine or challenge UPs (CUG).
- Contradictions lower trust, generate new UPs, or reclassify ON meanings.
- Continuity is recursively evaluated from stable UPs reinforced over time.
- New understanding often emerges from contradictions, not repetition.

---

**Last updated:** 2025-06-12
