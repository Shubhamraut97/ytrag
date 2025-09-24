RAG Using LangChain

This Jupyter notebook demonstrates a simple Retrieval-Augmented Generation (RAG) system using LangChain. It fetches a YouTube video transcript, processes it into chunks, embeds the chunks using OpenAI embeddings, stores them in a FAISS vector store, and sets up a chain for querying the content with an LLM (GPT-4o-mini).

The example uses a transcript from a Lex Fridman podcast interview with Demis Hassabis (CEO of DeepMind) on AI topics like protein folding, games, and more.

Features





Fetches YouTube transcript using youtube-transcript-api.



Splits text into chunks with RecursiveCharacterTextSplitter.



Generates embeddings with OpenAI's text-embedding-3-small.



Stores embeddings in a FAISS vector database.



Sets up a retriever for similarity search.



Builds a LangChain chain for RAG: retrieval, prompt augmentation, and generation using gpt-4o-mini.



Includes error handling for transcripts (e.g., if captions are disabled).






Requirements

Python 3.12+
OpenAI API key (set as OPENAI_API_KEY environment variable).
Libraries: youtube-transcript-api, langchain-community, langchain-openai, faiss-cpu, tiktoken, python-dotenv.
