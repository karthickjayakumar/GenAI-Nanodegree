# Custom Chatbot Project

## Overview
This project demonstrates how to use a custom dataset with a language model via Retrieval-Augmented Generation (RAG). It leverages a 2023 fashion trends dataset to extend the knowledge of an LLM beyond its original training data.

## Dataset
The dataset **"2023_fashion_trends.csv"** contains information on the latest fashion trends, allowing the chatbot to answer questions about recent updates not covered by GPT-3.5's training (limited to 2022).

## Features
- **Data Wrangling**: Load, clean, and prepare the dataset.
- **Custom Query Completion**: Use OpenAI's Completion model for dataset-based queries.
- **RAG**: Generate embeddings to retrieve relevant context for accurate responses.
- **Performance Comparison**: Compare context-aware completions with general completions.

## Installation
Ensure Python is installed, then run:
```sh
pip install -r requirements.txt
```

## Dependencies
- `pandas`: Data manipulation.
- `openai`: Interact with GPT models.
- `numpy`: Numerical operations.
- `tiktoken`: Tokenizer for prompt creation.

## Usage
1. **API Key**: Set your OpenAI API key:
   ```python
   openai.api_key = "YOUR_API_KEY"
   ```
2. **Run the script**: Load the dataset, generate embeddings, and interact with the chatbot.

## Example Queries
- "Tell me about the upcoming fashion trends."
- "What are the pros and cons of oversized bags?"

## Output
The chatbot provides responses using context retrieved from the dataset, extending beyond GPT-3.5's original knowledge.




