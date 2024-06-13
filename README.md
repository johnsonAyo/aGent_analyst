# Retrieval-Augmented Generation (RAG) Assisted Data Analyst Agent with Cohere and Langchain

Retrieval-Augmented Generation (RAG) is a technique that combines the strengths of pre-trained language models with real-time information retrieval. This allows the agent to provide accurate, contextually relevant, and up-to-date responses by augmenting its knowledge with external data sources. In this project, we use Cohere's Command R+ mode for language generation and Langchain for integrating various tools to create a powerful data analyst agent.

### Tools Used

- Notebook
- Cohere command-r-plus
- langchain
- tavily

Cohere's Command R+ is a language model designed for retrieval-augmented generation tasks. It helps the agent generate accurate and contextually relevant responses by leveraging both pre-trained knowledge and external information retrieval.

To use Cohere's Command R+ mode, you need to set up the API key:

```python
import os
os.environ['COHERE_API_KEY'] = "your_cohere_api_key_here"

# Create the Cohere chat model
from langchain_cohere.chat_models import ChatCohere
chat = ChatCohere(model="command-r-plus", temperature=0.3)
```


```python
Prompt
agent_executor.invoke({
    "input": "What is the latest quarterly revenue of Tesla and what recent events have influenced it?"
})

Output 
 "Tesla's latest quarterly revenue was $21.30 billion for Q1 2024, marking a decrease from the $23.33 billion recorded in Q1 2023. This reduction can be attributed to a combination of factors, including the company's decision to decrease the prices of its vehicles by up to 20% in reaction to competition in the global market for electric vehicles and rising inflation rates.",

Alongside with list of web citations
```

## Contributing
If you would like to contribute to this project, please follow these steps:

Fork the repository.
- Create a new branch (git checkout -b feature-branch).
- Commit your changes (git commit -am 'Add new feature').
- Push to the branch (git push origin feature-branch).
- Create a new Pull Request.

