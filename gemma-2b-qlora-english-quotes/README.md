# Fine-Tuning Gemma 2-2B with QLoRA on English Quotes

This repository contains the code used to fine-tune [google/gemma-2-2b](https://huggingface.co/google/gemma-2-2b) using QLoRA and PEFT techniques on the [Abirate/english_quotes](https://huggingface.co/datasets/Abirate/english_quotes) dataset.

🔗 **Finetuned Model on Hugging Face:**  
👉 [sccsmartcode/gemma-2-2b-qlora-english-quotes](https://huggingface.co/sccsmartcode/gemma-2-2b-qlora-english-quotes)

---

## 📌 Project Overview

- **Base Model**: `google/gemma-2-2b`
- **Fine-tuning Strategy**: QLoRA (Quantized Low-Rank Adaptation)
- **Library Stack**: Hugging Face `transformers`, `trl`, `peft`, `bitsandbytes`
- **Training Samples**: 2000 quotes
- **Goal**: Predict author and tags from a given quote using a ChatML-like prompt format.

---

## 🧠 Prompt Format

Each sample is trained in the following format:

```text
<start_of_turn>user
“Be yourself; everyone else is already taken.”
<end_of_turn>
<start_of_turn>model
Author: Oscar Wilde
Tags: authenticity, individuality
<end_of_turn>
```

---

## 📚 Acknowledgments

* [Google - Gemma 2-2B](https://huggingface.co/google/gemma-2-2b)
* [Hugging Face PEFT](https://github.com/huggingface/peft)
* [Transformers](https://github.com/huggingface/transformers)
* [Abirate/english\_quotes Dataset](https://huggingface.co/datasets/Abirate/english_quotes)
