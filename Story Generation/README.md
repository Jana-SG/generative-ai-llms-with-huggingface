# Text Generation with BLOOM-7B (Quantized Inference)

## Overview

This notebook demonstrates autoregressive text generation using the pretrained model `bigscience/bloom-7b1` from Hugging Face.

The model is loaded using 8-bit quantization to reduce memory usage and enable efficient inference on limited GPU resources. Custom decoding parameters are applied to control output diversity and repetition.

---

## Model Details

- **Model:** `bigscience/bloom-7b1`
- **Architecture:** Decoder-only Transformer (Causal Language Model)
- **Inference Optimization:** 8-bit quantization (BitsAndBytes)
- **Framework:** PyTorch + Hugging Face Transformers

---

## Key Concepts Demonstrated

- Loading large LLMs with 8-bit precision
- Controlled text generation using:
  - Temperature scaling
  - Top-p (nucleus sampling)
  - Repetition penalty
  - No-repeat n-gram constraints
- Prompt-based creative story generation

---

## Installation

Install required libraries:

```bash
pip install torch transformers accelerate bitsandbytes


## How to use 
- Open the notebook
- Modify the prompt variable with your desired text input
- Run the generation cell
- Adjust sampling parameters (temperature, top-p, etc.) to explore output variations

## Usage 
### Example input 
>Once upon a time,there was a young child exploring the forest.
>Suddenly, they discovered ancient ruins hidden beneath the overgrown vines.
>The child stepped inside and ...

### Example output 
     found an old man sitting on a rock. He told him to be careful of his steps as he could see through the stones.
      “My son,” said the old man, “I am your father. I have traveled far from my home in order to bring you here. You must not run or jump around so much. Stay still and keep your eyes open. There is danger everywhere!”

      “Why? What’s wrong?” asked the little boy with wide-open eyes.

      “The monsters are coming! They will kill us all!” screamed the old woman, her voice shaking with fear.

       She ran off into the woods crying and screaming. Her cries echoed throughout the forest for miles.

       A few days later, the boy heard a terrible scream that pierced his heart. It came from deep within the          cave where he had been hiding. He rushed out only to find that the old lady had disappeared.

       At first, he thought she had gone back home but then he saw something moving behind him—a huge monster          with black hair and sharp claws.

       The creature grabbed hold of him and pulled him down into its mouth. As it swallowed him whole, the    monster growled loudly. Then it turned away and vanished into the darkness.

       Afterwards, the girl who lived next door began hearing strange noises. Sometimes they were like angry voices shouting at each other; sometimes they sounded like animals calling to one another. Finally, she decided to go investigate.

       One day, when she went outside, she saw the monster again. This time, however, it looked different: it had long gray fur and golden horns. Its eyes glowed bright green while its teeth gleamed white. It seemed even more frightening than before.

       With great difficulty, the little girl managed to get away unharmed. When she got back home, she told her mother everything that happened. Her mother laughed and said: “Nonsense! It’s just a fairy tale. Go back to bed now.” But soon after, she fell asleep too.

       Another morning dawned and the girl woke up feeling very sleepy. She opened her eyes and noticed that there was someone standing beside her. Her eyes widened in surprise as she recognized the monster she’d seen earlier.

       “Have you forgotten me already?” cried the monster. “You can’t hide forever. Come out and face me 

