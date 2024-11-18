# HomeMatch - Personalized Real Estate Listings Application

## Overview
HomeMatch is an application developed for "Future Homes Realty" to provide a personalized experience for clients interacting with real estate listings. By leveraging Large Language Models (LLMs) and vector databases, HomeMatch transforms standard listings into tailored narratives that match each buyer's preferences.

## Features
- **Generate Listings**: Automatically generate multiple property listings using OpenAI's LLM.
- **Store Listings**: Store generated listings in ChromaDB for semantic search.
- **Collect Buyer Preferences**: Gather and interpret buyer preferences using natural language input.
- **Semantic Search**: Use embeddings to match listings with buyer preferences.
- **Personalized Descriptions**: Personalize property descriptions to highlight features relevant to each buyer.

## Project Components
1. **Data Generation**: Create synthetic real estate listings using an LLM.
2. **Vector Database**: Store listings as embeddings in ChromaDB for fast semantic search.
3. **Preference-Based Search**: Match listings using buyer preferences.
4. **Personalized Descriptions**: Enhance listing descriptions to align with buyer needs.

## Installation
Ensure Python is installed, then run:

```sh
pip install pandas langchain==0.0.305 openai==0.28.1 chromadb==0.4.12 pydantic<2.0 fastapi sentence-transformers transformers tiktoken jupyter
```

## Running the Project
Run the project in a Jupyter notebook:

### Step 1: Set Up Environment
- **Install Dependencies**: Use the command provided above.
- **Import Libraries**: Import necessary libraries.

### Step 2: Generate Listings
- Use OpenAI LLM to generate at least 10 listings.
- Save the listings as a CSV file.

### Step 3: Set Up Vector Database
- Configure ChromaDB to store listings.
- Generate and store embeddings.

### Step 4: Collect Buyer Preferences
- Define buyer preferences interactively or hard-code values.

### Step 5: Perform Semantic Search
- Use preferences to query the database and retrieve matching listings.

### Step 6: Personalize Descriptions
- Use an LLM to personalize matching listings.

## Example Workflow
1. **Generate Listings**: Generate listings with detailed descriptions.
2. **Store Listings**: Save listings in ChromaDB for efficient search.
3. **Collect Preferences**: Gather buyer requirements like location, budget, and features.
4. **Semantic Search**: Find listings matching buyer preferences.
5. **Personalize Results**: Enhance each listing to highlight relevant features.

## Key Technologies
- **Python**: Core programming language.
- **LangChain**: Framework for LLM-powered applications.
- **OpenAI**: Used for generating and personalizing content.
- **ChromaDB**: Vector database for storing embeddings.
- **Pydantic**: Data validation and settings management.
- **FastAPI**: Data handling.

## Dependencies
- `langchain==0.0.305`
- `openai==0.28.1`
- `pydantic<2.0`
- `chromadb==0.4.12`
- `pandas`
- `sentence-transformers`
- `transformers`
- `tiktoken`
- `jupyter`

## Usage
Run the project in a Jupyter notebook. Each code block helps you understand components like generating listings and personalizing them based on user input.

Set your OpenAI API key before running:

```python
OPENAI_API_KEY = 'YOUR_API_KEY_HERE'
os.environ['OPENAI_API_KEY'] = OPENAI_API_KEY
```


