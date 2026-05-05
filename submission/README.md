# LLM 20 Questions Baseline Agent

## Overview
This repository contains the baseline implementation for the Kaggle LLM 20 Questions competition. The baseline is based on the official Kaggle starter notebook and uses the Gemma 7B instruction-tuned model.

## Competition
Kaggle: LLM 20 Questions

## Model Used
- Gemma 7b-it-quant
- Hosted through Kaggle model input

## Baseline Implementation
The baseline agent is implemented in `submission/main.py`.

The agent handles three turn types:

- `ask`: generates a yes/no question
- `guess`: predicts the hidden keyword
- `answer`: gives a yes/no response

## Output
The notebook generates:

```text
submission.tar.gz

## Baseline Implementation

This baseline uses the official Gemma 7B instruction-tuned model provided in the Kaggle starter notebook.

The implementation includes:
- Gemma model loading (7b-it-quant)
- Questioner agent for asking and guessing
- Answerer agent for yes/no responses
- Prompt formatting and few-shot examples

The agent is executed through `agent_fn()` following Kaggle competition requirements.

Note:
Model weights are loaded from Kaggle environment:
`/kaggle/input/gemma/pytorch/7b-it-quant/2`
