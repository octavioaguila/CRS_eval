# 🔍 CRS_eval 🔍

Welcome to our project's repository! 

## Index
- [Dataset Comparison](#dataset-comparison)
- [Uncertainty](#uncertainty)

## Dataset Comparison

The dataset comparison experiments are organized in separate notebooks, each corresponding to a specific model and dataset combination. In each notebook, we fine-tune the model using either the PEARL or ReDial dataset and evaluate its performance across a wide range of metrics.

The evaluated metrics include:
Recall@1, BLEU Score, ROUGE-1, ROUGE-2, ROUGE-L, Distinct-1 intra/inter, Distinct-2 intra/inter, BERTScore (F1, Precision, Recall), Novelty Score, and Self-BLEU Score.
Additionally, we test how the models respond to various user prompts.

Below is a list of notebooks and their respective roles:

DeepSeekPEARL.ipynb: Fine-tunes the DeepSeek model on the PEARL dataset. Includes full metric evaluation and prompt testing.

LLama3PEARL.ipynb: Fine-tunes the LLaMA 3 model on the PEARL dataset. Same evaluation process as above.

QwenPEARL.ipynb: Fine-tunes the Qwen model on the PEARL dataset. Includes all metric evaluations and response testing.

DeepSeekReDial.ipynb: Fine-tunes the DeepSeek model on the ReDial dataset. Mirrors the evaluation and testing pipeline used with PEARL.

LLama3ReDial.ipynb: Fine-tunes the LLaMA 3 model on the ReDial dataset with the same evaluation framework.

QwenReDial.ipynb: Fine-tunes the Qwen model on the ReDial dataset, using identical evaluation procedures.

## Uncertainty

The uncertainty experiments are fully contained in *Uncertainty.ipynb* notebook. 

You can find the model's parameters, answers and generated clarifications in our [google drive link](https://drive.google.com/drive/folders/16VGhkEmf3XPGDzkxXye09UbWyKpkzLna?usp=sharing) or in the *uncertainty_data* folder (fine tuned models are only available in google drive).

Here you have a brief description of each file:

- *ambiguous_200.json* : Contains the 200 ambiguos questions dataset.
- *clarifications.json*: Contains 800 clarifications, 4 per ambiguos question.
- *answers_llama3_1shot.jsonl*: Contains 800 answers to the 800 clarifications from the Llama3 model inference.
- *answers_deepseek_1shot.jsonl*:Contains 800 answers to the 800 clarifications from the Deepseek model inference.
- *answers_qwen_1shot.jsonl*: Contains 800 answers to the 800 clarifications from the Qwen model inference.
- *pearl_<model\>_model.zip*: .zip with model's fine tunning in PEARL.
