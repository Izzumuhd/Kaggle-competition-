# Iterative Model Development Log

## Project

Development of an LLM-Based Intelligent Agent for the Kaggle LLM 20 Questions Competition

### Team Members

| Member | ID |
|---|---|
| Muhamad Izzudin Bin Muhamad | 2219735 |
| Muhamad Imran Haziq Bin Haizam | 2216429 |

---

## Baseline

**Description**

* Original Gemma 7B Kaggle starter notebook.
* Questioner and Answerer agents implemented using the provided baseline architecture.

**Observed Issues**

* Random and inconsistent questions.
* Repeated questioning patterns.
* Poor keyword narrowing strategy.
* Formatting artifacts in generated responses.
* Unreliable keyword extraction.

---

## Experiment V1 – Prompt Engineering

### Modification

Enhanced the Questioner prompt with strategic instructions:

* Use previous questions and answers as context.
* Avoid repeated questions.
* Focus on narrowing the search space.
* Ask yes/no questions only.

### Observation

Questions became more structured and context-aware.

### Outcome

Improved reasoning flow compared with the baseline.

---

## Experiment V2 – Few-Shot Learning

### Modification

Added few-shot gameplay examples demonstrating:

* Category identification.
* Logical narrowing.
* Correct keyword formatting.

### Observation

The model followed the demonstrated reasoning process more closely.

### Outcome

Improved output consistency and keyword guessing behavior.

---

## Experiment V3 – Output Sanitization

### Modification

Implemented response-cleaning functions using regular expressions.

### Observation

Removed unwanted prefixes such as:

* "Question:"
* "Sure, here's your question:"
* "The answer is:"

### Outcome

Cleaner and more competition-compliant outputs.

---

## Experiment V4 – Rule-Based Guardrails

### Modification

Added explicit reasoning rules:

* Identify person/place/thing first.
* Ask broad questions before specific questions.
* Avoid subjective questions.
* Avoid descriptive questions.
* Use previous context before generating a new question.

Added fallback keyword extraction when output formatting fails.

### Observation

Question generation became more category-oriented and structured.

### Outcome

Improved robustness and consistency of the agent.

---

## Summary of Improvements

| Version  | Main Improvement      | Result                    |
| -------- | --------------------- | ------------------------- |
| Baseline | Original Gemma 7B     | Random questioning        |
| V1       | Prompt Engineering    | More structured questions |
| V2       | Few-Shot Learning     | Better reasoning examples |
| V3       | Output Sanitization   | Cleaner outputs           |
| V4       | Rule-Based Guardrails | More consistent reasoning |

---

## Key Insights

* Prompt engineering significantly affects LLM behavior.
* Few-shot examples improve output consistency.
* Output sanitization is necessary for competition compliance.
* Rule-based guardrails improve reasoning structure.
* Top leaderboard solutions often combine LLM reasoning with algorithmic search strategies.

---

## Future Work

* Implement memory mechanisms to prevent repeated questions.
* Expand few-shot examples across multiple categories.
* Introduce information-gain-based questioning.
* Investigate hybrid LLM + algorithmic search strategies.
* Evaluate performance quantitatively using leaderboard results.
