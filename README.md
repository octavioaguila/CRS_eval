# 🔍 CRS_eval 🔍

Welcome to our project's repository! 

## Index
- [Dataset Comparison](#dataset-comparison)
- [Uncertainty](#uncertainty)

## Dataset Comparison

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
