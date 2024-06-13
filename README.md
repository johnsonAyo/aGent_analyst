# Retrieval-Augmented Generation (RAG) Assisted Data Analyst Agent with Cohere and Langchain

In this notebook, we'll see how we can use two tools to create a simple data analyst agent that is able to search the web and run code in a Python interpreter. This agent uses Cohere's Command R+ mode and Langchain.

## Contents

- `Agent_Analyst.ipynb`: The main notebook containing the analysis and agent implementation.

## Overview

The `Agent_Analyst.ipynb` notebook demonstrates how to create a data analyst agent using Retrieval-Augmented Generation (RAG) techniques. The agent can search the web for relevant information and execute Python code for data analysis.

### Tools Used

#### 1. Cohere's Command R+ Mode

Cohere's Command R+ is a language model designed for retrieval-augmented generation tasks. It helps the agent generate accurate and contextually relevant responses by leveraging both pre-trained knowledge and external information retrieval.

To use Cohere's Command R+ mode, you need to set up the API key:

```python
import os
os.environ['COHERE_API_KEY'] = "your_cohere_api_key_here"

# Create the Cohere chat model
from langchain_cohere.chat_models import ChatCohere
chat = ChatCohere(model="command-r-plus", temperature=0.3)
