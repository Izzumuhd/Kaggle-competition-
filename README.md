# 🧠 LLM 20 Questions – Deep Learning Course Project

This repository contains our work for the **MCTA4363 Deep Learning Course Project**, under **Track 1: Kaggle Competition**.

## 📌 Competition Link
[LLM 20 Questions – Kaggle](https://www.kaggle.com/competitions/llm-20-questions)

---

## 📖 Project Overview
This project focuses on developing an intelligent language-based agent for the **LLM 20 Questions** competition on Kaggle.

The objective is to build an AI agent that can play the classic **20 Questions** game by:
- asking strategic **yes/no questions**
- interpreting previous responses
- making accurate guesses about a hidden keyword

This project is related to **Deep Learning**, particularly in the area of:
- **Natural Language Processing (NLP)**
- **Large Language Models (LLMs)**
- **reasoning and decision-making systems**

---

## 🎯 Objectives
- Develop a working AI agent for the 20 Questions game
- Understand the competition framework and starter implementation
- Compare a **baseline agent** with an **improved strategy**
- Analyze the role of LLMs in interactive reasoning tasks

---

## ⚙️ Methodology
The project is divided into two main stages:

### 1. Baseline Agent
We first study and run the official Kaggle starter notebook to understand how the competition agent works.

### 2. Improved Agent
We then modify the questioning and guessing strategy to make the agent more structured and efficient in narrowing down the hidden keyword.

---

## 🛠️ Tools & Technologies
- Python
- Kaggle Notebooks
- Google Colab (for testing)
- GitHub
- Large Language Model (Gemma starter environment)

---

## 📂 Repository Structure
```bash
.
├── notebooks/        # Kaggle / Colab notebooks
├── src/              # agent logic / helper code
├── results/          # outputs / screenshots / notes
└── README.mdv


## Iterative Model Development Log

| Experiment | Modification | Observation | Outcome |
|---|---|---|---|
| Baseline | Original Gemma 7B starter notebook | Random and inconsistent questions | Weak reasoning performance |
| Experiment 1 | Added strategic prompt engineering | Questions became more context-aware | Improved relevance |
| Experiment 2 | Added structured few-shot examples | Better narrowing sequence | More logical questioning |
| Experiment 3 | Added output sanitization | Removed unwanted prefixes and formatting artifacts | Cleaner outputs |
| Experiment 4 | Added strategic reasoning constraints | Reduced vague and low-information questions | More efficient narrowing |

---

### Key Improvements Implemented

- Prompt engineering for more strategic questioning
- Few-shot learning examples for guided reasoning
- Output sanitization to remove formatting artifacts
- Context-aware narrowing strategy
- Improved keyword guessing consistency

---

### Insights Gained

- Weak prompts caused random and low-quality questions
- Few-shot examples significantly improved logical flow
- LLM outputs require post-processing for stable formatting
- Strategic prompting improves narrowing efficiency in 20 Questions gameplay
- Iterative refinement is important for improving LLM reasoning behavior
