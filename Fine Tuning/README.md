# Task 3

## Overview of the task

the main goal of this task was to compare model behaviour on a task before and after fine tuning(using HuggingFace trainer) on a small dataset
I choose **distilgpt2 (distilgpt2)** and **Poetry-Foundation-Poems(suayptalha/Poetry-Foundation-Poems)** for this task 

## prerequisites 
- ensure you have torch, transformers and datasets libraries installed
    ```bash
    pip install torch transformers accelerate datasets

## How to use the code if you want to compare yourself ?
- download the code on your device 
- open a code editor of your choice
- change the prompt in both before and after fine tuning cells
- run both and compare 

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
