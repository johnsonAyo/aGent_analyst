# Retrieval-Augmented Generation (RAG) Assisted Data Analyst Agent with Cohere and Langchain

Retrieval-Augmented Generation (RAG) is a technique that combines the strengths of pre-trained language models with real-time information retrieval. This allows the agent to provide accurate, contextually relevant, and up-to-date responses by augmenting its knowledge with external data sources. In this project, we use Cohere's Command R+ mode for language generation and Langchain for integrating various tools to create a powerful data analyst agent.

### Tools Used

- Notebook
- Cohere_api_key
- langchain
- TAVILY_API_KEY

Cohere's Command R+ is a language model designed for retrieval-augmented generation tasks. It helps the agent generate accurate and contextually relevant responses by leveraging both pre-trained knowledge and external information retrieval.

To use Cohere's Command R+ mode, you need to set up the API key:

```python
import os
os.environ['COHERE_API_KEY'] = "your_cohere_api_key_here"

# Create the Cohere chat model
from langchain_cohere.chat_models import ChatCohere
chat = ChatCohere(model="command-r-plus", temperature=0.3)
```

## Contributing
If you would like to contribute to this project, please follow these steps:

Fork the repository.
- Create a new branch (git checkout -b feature-branch).
- Commit your changes (git commit -am 'Add new feature').
- Push to the branch (git push origin feature-branch).
- Create a new Pull Request.

