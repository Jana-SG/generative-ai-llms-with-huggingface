# Summarization & Question Answering with T5

## Overview

This notebook demonstrates sequence-to-sequence modeling using the pretrained `t5-base` model from Hugging Face.

The implementation covers two NLP tasks:

1. Abstractive text summarization of a news article  
2. Question answering based on the same article context  

The model is prompted using task-specific prefixes to perform controlled generation.

---

## Model Details

- **Model:** `t5-base`
- **Architecture:** Encoder-Decoder Transformer (Seq2Seq)
- **Framework:** PyTorch + Hugging Face Transformers
- **Decoding Strategy:** Beam search with configurable parameters

---
## Tasks Implemented

### 1️⃣ Abstractive Summarization

- Input format:
  summarize: <news article text>
- Generates a concise summary of the article.
- Uses beam search decoding for improved output quality.

### 2️⃣ Question Answering

- Input format:
  question: <question> context: <article text>
- Produces an answer based solely on the provided context.

---

## Installation

Install required libraries:

```bash
pip install torch transformers accelerate
```
## How to use 
- Open the notebook
- Provide the path to your news article (in .txt format)
- Run the summarization cell to generate the summary
- Enter your question
- Run the QA cell to generate the answer 

## Usage 
### Example input (saved as a txt)
- summarization 
> https://www.theguardian.com/world/2025/dec/10/louvre-thieves-evaded-police-with-30-seconds-to-spare-investigation-finds

- Question 
> Have the police arrested all the thieves ?

### Example output 
- summarization 
> only one of two security cameras was working near the site where the intruders broke in on the morning of Sunday 19 October . agents in the security control room did not have enough screens to follow the images in real-time . a lack of coordination meant police were initially sent to the wrong place once the alarm was raised . one of the most startling revelations was that the thieves had only 30 seconds to spare before police and private security guards arrived on the scene .

- Answer
> police believe they have arrested all four intruders

## Key Concepts Demonstrated

- Encoder-decoder (Seq2Seq) Transformer architecture  
- Task-specific prompting using T5 input prefixes  
- Beam search decoding for improved generation quality  
- Context-conditioned answer generation  
- Abstractive text summarization techniques  

