# 🌳 Daily Reflection Tree

A deterministic, structured reflection system designed to help employees analyze their day through guided thinking — **without using any LLM at runtime**.

---

## 🎯 Objective

This project implements a **decision-tree-based reflection agent** that walks a user through three psychological dimensions:

1. **Locus of Control** (Victim ↔ Victor)
2. **Orientation** (Entitlement ↔ Contribution)
3. **Radius of Concern** (Self ↔ Others)

The system ensures:

* Predictable outcomes
* Consistent experience
* Structured introspection

---

## 🧠 Core Idea

Instead of free-form AI conversations, this system uses a **deterministic tree**:

* Every question has fixed options
* Every option leads to a predefined path
* Reflections are pre-written and context-aware
* No randomness or AI calls at runtime

---

## 📁 Project Structure

```
.
├── tree/
│   ├── reflection-tree.tsv      # Core decision tree (data structure)
│   └── tree-diagram.md          # Visual flow (Mermaid diagram)
│
├── docs/
│   ├── write-up.md              # Design explanation and rationale
│   └── reference-guide.txt      # File format and usage guide
│
└── README.md
```

---

## 🔄 How It Works

1. User starts reflection session
2. System asks structured questions
3. User selects from fixed options
4. Tree branches based on answers
5. Signals are recorded (axis-wise)
6. Reflection messages are shown
7. Final summary synthesizes responses

---

## 🧩 Node Types Used

* **start** → Begins session
* **question** → User selects an option
* **decision** → Routes flow based on answer
* **reflection** → Provides insight
* **bridge** → Moves between axes
* **summary** → Final synthesis
* **end** → Closes session

---

## 📊 Axes Explained

### 1. Locus of Control

* Internal → Ownership of actions
* External → Blaming circumstances

### 2. Orientation

* Contribution → Focus on giving
* Entitlement → Focus on receiving

### 3. Radius of Concern

* Self → Personal perspective
* Others → Broader awareness

---

## 🛠️ How to View Files

### TSV File

* Open `reflection-tree.tsv` in Excel (recommended)
* Or view in VS Code as raw data

### Markdown Files

* Open `.md` files in VS Code
* Press `Ctrl + Shift + V` for preview

### Mermaid Diagram

* Requires extension:

  * **Markdown Preview Enhanced** (recommended)
* Then preview `tree-diagram.md`

---

## ⚙️ Key Features

* Fully deterministic system
* No LLM usage at runtime
* Structured psychological framework
* Clear branching logic
* Interpolated reflections

---

## 🚀 Possible Extensions

* CLI / Web-based agent implementation
* Signal-based scoring system
* Multi-day reflection tracking
* Enhanced UI visualization

---

## 🧾 Notes

* All files are text-based formats (`.tsv`, `.md`, `.txt`)
* Designed for clarity, traceability, and extensibility

---

## 👤 Author

Yashraj Singh

---

**End of Project**
