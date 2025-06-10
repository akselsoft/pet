---
layout: default
title: "Reinforced Dog Encounter"
---

This walkthrough builds on the initial **Dog Encounter** scenario and explores how new experiences reinforce or alter prior interpretations.

Initially, the system associates "Dog" with "Danger" through stories or past warnings. This understanding is stored in a long-term **Understanding Node** that flags the link as `NonExist` (a danger to avoid).

Later, a real-world encounter with a friendly dog (e.g., licking, tail wagging) is processed by the system. A new Understanding Node is created—this time linking "Dog" to "Lick" or "Comfort" with a flag of `Exist`.

Through this scenario, we illustrate:

- How PET handles conflicting interpretations via separate Understanding Nodes.
- The role of experience in gradually shifting neural net weighting.
- The process by which future predictions (short-term graph DB) adapt to new data.

This is a key mechanism for how PET systems evolve their understanding over time while preserving past context.
