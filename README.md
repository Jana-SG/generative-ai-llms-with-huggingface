# Generative AI & Large Language Models with Hugging Face

This repository contains applied experiments with Transformer-based Large Language Models (LLMs) using Hugging Face and PyTorch.

The project explores three core aspects of modern NLP systems:

- Large-scale model inference with quantization
- Sequence-to-sequence modeling for summarization and question answering
- Fine-tuning causal language models on domain-specific data
- 
---

## Repository Structure

### 1️⃣ Story Generation with BLOOM-7B (Quantized Inference)

- Model: `bigscience/bloom-7b1`
- 8-bit model loading using BitsAndBytes
- Temperature & top-p sampling
- Repetition penalty & no-repeat n-gram constraints
- Creative story generation from prompts

📄 Notebook: `text_generation.ipynb`

---

### 2️⃣ Summarization & Question Answering with T5

- Model: `t5-base`
- Encoder–decoder (Seq2Seq) architecture
- Abstractive summarization
- Context-based question answering
- Beam search decoding

📄 Notebook: `summarization_qa.ipynb`

---

### 3️⃣ Fine-Tuning DistilGPT2 for Poetry Generation

- Base Model: `distilgpt2`
- Dataset: `suayptalha/Poetry-Foundation-Poems`
- Hugging Face `Trainer` API
- Causal Language Modeling objective
- Before vs After fine-tuning comparison

📄 Notebook: `fine_tuning.ipynb`

---

## Technical Highlights

- Efficient LLM inference using 8-bit quantization  
- Controlled text generation via decoding strategies  
- Encoder–decoder vs decoder-only architecture comparison  
- Transfer learning for domain adaptation  
- Training workflows using Hugging Face Trainer  
- Dataset preprocessing with the `datasets` library  

---

## Technologies Used

- Python  
- PyTorch  
- Hugging Face Transformers  
- Hugging Face Datasets  
- BitsAndBytes  
- CUDA (optional GPU acceleration)

## How to Run

- Clone the repository:

 ```bash
  git clone https://github.com/Jana-SG/generative-ai-llms-with-huggingface.git
 ```

- Open any notebook:
  - text_generation.ipynb
  - summarization_qa.ipynb
  - fine_tuning.ipynb

- Run cells sequentially.



