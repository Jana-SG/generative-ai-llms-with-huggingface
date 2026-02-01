# Fine-Tuning DistilGPT2 for Poetry Generation

## Overview

This notebook explores the behavioral differences of a pretrained language model before and after fine-tuning.

The base model `distilgpt2` is fine-tuned on a subset of the `suayptalha/Poetry-Foundation-Poems` dataset using the Hugging Face `Trainer` API. The goal is to observe how domain-specific fine-tuning influences text generation quality and stylistic coherence.

---

## Model & Dataset

- **Base Model:** `distilgpt2`
- **Architecture:** Decoder-only Transformer (Causal Language Model)
- **Dataset:** `suayptalha/Poetry-Foundation-Poems`
- **Framework:** PyTorch + Hugging Face Transformers
- **Training Interface:** Hugging Face `Trainer`

---

## Training Pipeline

- Tokenization with appropriate padding and truncation
- Train/test split (80/20)
- Causal Language Modeling objective
- Evaluation at each epoch
- Controlled generation for comparison

---

## Installation

Install required libraries:

```bash
pip install torch transformers accelerate datasets
```

## How to use 
- Open the notebook 
- Run the preprocessing and training cells
- Modify the prompt in the before fine-tuning generation cell
- Run the after fine-tuning generation cell
- Compare stylistic and structural differences

## Usage 
### Example input 
> Write a short 5 line poem about rainfall

### Example output 
-Before fine tuning
>I would like to get to know your favourite story about the rain. What was it like in that song?
>I think you are going to like the story about the rain.
>So, what would you like to see you go to the rain.
>My idea is to go to a place

-After fine tuning 
>a few dozen people who walk through the streets
>and see the rain.
>In the dark, one hears a sound,
>and one hears the light.
>One hears the wind.

## Key Concepts Demonstrated

- Open the notebook
- Run the preprocessing and training cells
- Modify the prompt in the before fine-tuning generation cell
- Run the after fine-tuning generation cell
- Compare stylistic and structural differences

