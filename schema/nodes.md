---

title: Node Types
layout: default
---------------

# 🧩 Node Types in PET

In Pattern Existence Theory, all information is structured as **nodes** connected by meaningful **edges**. This page outlines the different node types used in the PET schema.

---

## 🔹 Object Nodes

* Represent people, places, things, or abstract concepts.
* Have a stable internal label (e.g., `Dog`, `Fire`, `Justice`).
* Can be connected to patterns, events, or other objects.

Example:

```
A child learns that "Dogs are dangerous" because their father said so.

- `id`: U123
- `source`: Father
- `time`: 2023-04-01
- `from`: Dog
- `to`: Danger
- `result`: warning
- `details`: "Father told me dogs bit him as a child"
```

```
Dog → Animal
Dog → Pet
Dog → Dangerous
```

---

## 🔹 Pattern Nodes

* Represent raw sensory input (visual hashes, audio frequencies, tactile signatures).
* May or may not be initially labeled.
* Linked to object nodes after association or training.

Example:

```
Pattern #AB12 → Dog
Pattern #98F1 → Fire Alarm
```

---

## 🔹 Source Nodes

* Represent the origin of information or belief:

  * Teachers
  * Books
  * Direct sensory channels (e.g., Eye1, Ear2)
* Referenced in Understanding Nodes.

Example:

```
Father, Book_Encyclopedia, Sensor_Eye1
```

---

## 🔹 Time Nodes

* Represent a specific moment or time window.
* Used to timestamp Understanding Nodes or Events.

Example:

```
Time_2023-10-01T08:43
```

---

## 🔹 Emotion Nodes (Optional)

* Represent emotional pattern responses (e.g., `Fear`, `Trust`, `Curiosity`).
* Can be linked to understanding or object nodes as qualifiers.

Example:

```
Dog → Fear (after bite)
Dog → Joy (after play)
```

---

## 🧠 Exist and Non-Exist Nodes

* These are **nodes**, not booleans.
* Used to qualify outcomes in Understanding Nodes:

  * `Dog → Danger → NonExist`
  * `Dog → Lick → Exist`

---

## 🔄 Summary Table

| Node Type      | Purpose                           | Example                    |
| -------------- | --------------------------------- | -------------------------- |
| Object Node    | Stable identity or category       | Dog, Person, Fire          |
| Pattern Node   | Raw, unlabeled input              | Pattern\_#AF32             |
| Source Node    | Origin of information             | Father, Book, Sensor\_Mic1 |
| Time Node      | When something occurred           | Time\_2025-07-04T18:01     |
| Emotion Node   | Optional emotional associations   | Joy, Fear                  |
| Exist/NonExist | Result interpretation (as a node) | Exist, NonExist            |

---

[← Back to Schema Overview](./index.md)
