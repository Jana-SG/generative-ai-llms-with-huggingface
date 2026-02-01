# Task 2

## Overview of the task

the main goal of this task was to use a Hugging Face model to summarize a news article 
and to have the model to answer a question based on that article 
 I choose **T5-base** for this task 

## prerequisites 
- ensure you have torch and transformers libraries installed
    ```bash
    pip install torch transformers accelerate

## How to use the code ?
- download the code on your device 
- open a code editor of your choice
- for the summarization task enter the path to your article in txt format
- run the summarization cell
- for the Question Answering task enter your question
- run the QA cell 

## Usage 
### Example input (saved as a txt)
- summarization 
> https://www.theguardian.com/world/2025/dec/10/louvre-thieves-evaded-police-with-30-seconds-to-spare-investigation-finds

- QA
> Have the police arrested all the thieves ?

### Example output 
- summarization 
> only one of two security cameras was working near the site where the intruders broke in on the morning of Sunday 19 October . agents in the security control room did not have enough screens to follow the images in real-time . a lack of coordination meant police were initially sent to the wrong place once the alarm was raised . one of the most startling revelations was that the thieves had only 30 seconds to spare before police and private security guards arrived on the scene .

- QA
> police believe they have arrested all four intruders


