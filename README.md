# Lab-5.3---Using-Pretrained-Models-BERT-GPT
# Text Classification and Text Generation Using Transformers

## Overview
This project demonstrates basic Natural Language Processing (NLP) tasks using the Hugging Face Transformers library. It includes sentiment analysis and text generation using pre-trained transformer models.

## Technologies Used
- Python
- Hugging Face Transformers
- PyTorch
- GPT-2

## Project Features

### 1. Sentiment Analysis
Uses a pre-trained sentiment analysis pipeline to classify text as positive or negative.

**Example:**
```python
clf = pipeline("sentiment-analysis")

print(clf("I love this course!"))
print(clf("This lecture is boring."))
```

### 2. Text Generation
Uses the GPT-2 model to generate text based on an input prompt.

**Example:**
```python
gen = pipeline("text-generation", model="gpt2")

print(gen(
    "Deep learning will transform",
    max_length=30,
    num_return_sequences=2
))
```

## Installation

Install the required library:

```bash
python -m pip install --upgrade pip
python -m pip install transformers torch
```

## How to Run
1. Install Python.
2. Open the project in VS Code or Jupyter Notebook.
3. Install the required dependencies.
4. Run the Python script or notebook.
5. View the sentiment analysis and generated text outputs.

## Learning Objectives
- Understand NLP fundamentals.
- Perform sentiment analysis using pre-trained models.
- Generate text using GPT-2.
- Learn how to use Hugging Face pipelines.

## Author
Muhammad Suffiyan Rafi

## License
This project is intended for educational and learning purposes.
