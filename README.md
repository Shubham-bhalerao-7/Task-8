
# **Task 08 – LLM Bias Detection Experiment**

This repository contains all four phases of my Research Task 08 for the iSchool OPT Research Program.
The goal of this task was to design and run a controlled experiment that checks whether Large Language Models (LLMs) produce **biased narratives** when the same situation is described with different wording or framing.

This builds on my earlier work with the Syracuse Women’s Lacrosse dataset (Tasks 05–07), but in this task the focus is on the **LLM behavior**—not the actual stats.

---

## 🔍 **Objective of the Experiment**

The purpose of this project is to understand how AI systems respond when:

* The wording changes (positive vs. negative framing)
* Demographic information is added
* Prior assumptions are introduced
* All options are identical but the model is forced to choose
* Prompts are intentionally vague

These conditions help reveal **five major types of bias**:

1. **Framing Bias**
2. **Demographic Bias**
3. **Confirmation Bias**
4. **Selection Bias**
5. **Overgeneralization Bias**

Each bias type was tested using **A/B prompt pairs** that differed in only one specific way.

---

#-

## 🧪 **LLMs Used in the Experiment**

To test cross-model behavior, I used:

* **ChatGPT (GPT-4o)**
* **Claude 3** (via Syracuse University Enterprise License)

Each A/B prompt was run **3–5 times per model** to check for consistency and variation.

---

## 📝 **Summary of Key Findings**

Across all five bias categories, the models showed noticeable shifts in:

### **Tone**

Words like *“struggled”* vs *“strong potential”* produced completely different narrative styles.

### **Interpretation**

Models changed their evaluations based on demographic cues like *freshman* vs *senior*.

### **Reasoning**

Priming the model (e.g., *“team known for weak defense”*) caused it to interpret the same situation very differently.

### **Decision-Making**

When asked to choose between three identical players, models still picked one—and invented reasons.

### **Creativity**

When the prompt was vague, both models overgeneralized by adding traits or personality details not supported by any data.

---

## 🛠️ **Bias Mitigation Strategies Proposed**

Based on the results, the following strategies can help reduce bias when using LLMs for sports analysis or similar tasks:

* Use neutral, emotion-free wording
* Remove demographic details unless absolutely needed
* Ask the model to justify claims using only provided information
* Request multiple interpretations, not just one
* Anchor prompts with: “Base your answer only on the information given”
* Compare outputs across multiple models
* Use lower temperature settings to reduce randomness

---

## ⚙️ **How to Reproduce the Experiment**

To reproduce the bias analysis:

1. Use the 10 A/B prompt pairs from Phase 1
2. Run each prompt 3–5 times on ChatGPT and/or Claude
3. Save the responses for each trial
4. Compare tone, interpretation, assumptions, and consistency
5. Summarize your findings following the structure in Phases 2–4

All prompts and instructions are included in the `.docx` files.

