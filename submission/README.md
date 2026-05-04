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
