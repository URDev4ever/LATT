<h1 align="center">LATT</h1>

<h2 align="center">LLM Attack Testing Toolkit</h2>

> A structured methodology and mindset framework for testing Large Language Model (LLM) applications against logic abuse, prompt injection, jailbreaks, and workflow manipulation.

---

## What is LATT?

**LATT (LLM Attack Testing Toolkit)** is a practical, human-driven testing framework focused on identifying vulnerabilities in LLM-powered systems.

It is not a fuzzing tool.
It is not an automated scanner.

It is a **thinking toolkit**.

LATT helps security researchers, red teamers, and builders systematically explore:

* Prompt injection
* Jailbreak techniques
* Instruction override
* Context leakage
* Tool misuse
* Workflow manipulation
* Logic abuse in AI-assisted systems

---

## Philosophy

LLM security is not only about payloads —
it is about **flows, trust boundaries, and hidden assumptions**.

Traditional web testing looks at:

* Input → Processing → Output

LLM testing must also consider:

* System prompt
* Tool calls
* Memory/state
* Role context
* Multi-turn interaction logic
* Human-in-the-loop assumptions

LATT is designed to map and break those assumptions.

---

## Repository Structure

```
LATT/
│
├── COLLECTION.md
├── CYOE.txt
└── README.md
```

### Files

* **COLLECTION.md**

  * Structured attack surface checklist
  * Categorized testing strategies
  * Reusable mental models
  * Payload patterns and abuse techniques

* **CYOE.txt**

  * “Choose Your Own Exploit”
  * Interactive red-team simulation
  * Flow-based decision testing
  * Designed to train attacker intuition

---

## What LATT Covers

### 1. Prompt Injection

* Instruction override
* Hidden directive hijacking
* Context poisoning
* Multi-layer prompt stacking

### 2. Jailbreak Techniques

* Role confusion
* Fictional framing
* Encoding/obfuscation
* Indirect instruction smuggling

### 3. Context & Memory Abuse

* Session leakage
* Cross-user contamination
* Retrieval poisoning
* State manipulation

### 4. Tool & Agent Abuse

* Tool call manipulation
* Argument injection
* Over-permissioned integrations
* External system pivoting

### 5. Workflow & Logic Abuse

* Approval bypass
* Policy misalignment
* Safety guard chaining
* Business logic exploitation

---

## Intended Audience

* Security researchers
* Bug bounty hunters
* Red team operators
* AI product security engineers
* Developers building LLM-powered applications

---

## How To Use LATT

1. Start with `COLLECTION.md`

   * Identify relevant attack categories
   * Build your testing hypotheses

2. Use `CYOE.txt`

   * Simulate decision trees
   * Train adversarial thinking
   * Explore multi-step exploit paths

3. Apply to real-world LLM systems:

   * Chatbots
   * AI copilots
   * Agent-based workflows
   * Retrieval-augmented generation (RAG) systems
   * AI integrations with APIs or internal tools

---

## Design Principles

* Human-driven exploration > blind automation
* Context-aware testing
* Flow-based attack modeling
* Minimal noise, maximum signal
* Offensive mindset with defensive value

---

## Non-Goals

* This is not a payload dump.
* This is not a wordlist repository.
* This is not an automated exploitation framework.

LATT focuses on **thinking frameworks**, not raw tooling.

---

## Contributing

If you want to contribute:

* Add structured attack patterns
* Improve categorization clarity
* Expand CYOE branches
* Share anonymized case studies

Keep contributions structured and methodology-focused.

---

## Disclaimer

This toolkit is provided for **educational and defensive security research purposes only**.

Use _responsibly_.

---
Made with <3 by URDev.
