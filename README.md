# Financial-LLM-Alignment: Curriculum SFT & DPO 📈

This repository hosts the code and models for a high-precision financial LLM pipeline. By combining **Curriculum Learning** and **Direct Preference Optimization (DPO)**, we enable mid-sized models (12B) to outperform larger 20B baselines.

## 🚀 Key Results
- **Judge:** Llama-3.3-70B-Versatile
- **Best Model:** Nemo-12B (Curriculum+DPO)
- **Top Score:** 30.70/40 (Beating GPT-OSS-20B Baseline)
- **Win Rate:** 80% against other fine-tuned models.

## 📦 Model Links (Hugging Face)
| Model | Type | Link |
| :--- | :--- | :--- |
| **Nemo-12B** | Curriculum+DPO | [HF Link](https://huggingface.co/J-Aamir/mistral-nemo-12b-financial-curriculum-dpo) |
| **Phi-3.5 Mini** | Financial-DPO | [HF Link](https://huggingface.co/J-Aamir/phi3.5-mini-financial-dpo) |
| **Qwen-7B** | Improved SFT | [HF Link](https://huggingface.co/J-Aamir/Fin-Qwen-7B-LoRA) |
| **Mistral-7B** | Standard SFT | [HF Link](https://huggingface.co/J-Aamir/Fin-Mistral-7B-LoRA) |

## 📊 Methodology
We employed a two-stage training strategy:
1. **Curriculum SFT:** Training on a difficulty-ranked subset of financial data (Easy -> Medium -> Hard).
2. **DPO Alignment:** Direct Preference Optimization to ensure the model prioritizes depth and accuracy over generic responses.

## 📈 Training Loss
The Nemo-12B training achieved a Final DPO loss of **0.1869**, showing strong convergence and alignment with financial expertise.

