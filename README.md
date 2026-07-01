# Multiutility-Chatbot-with-RAG-and-Custom-Tools
In this end-to-end project, I built a Multiutility Agentic RAG Chatbot using LangGraph. This chatbot can read and understand PDF documents using PyPDF, store and
retrieve relevant information with FAISS vector search, perform web search using DuckDuckGo, and use custom tools like a calculator to answer user queries more 
intelligently. RAG techniques allow the chatbot to retrieve accurate context from documents and combine it with an LLM’s reasoning ability, making responses more 
useful, grounded, and context-aware.

<img width="1672" height="693" alt="image" src="https://github.com/user-attachments/assets/651d440b-734d-4197-a26d-267a11ea2e9e" />

# Description
This project showcases the implementation of a Multiutility Agentic RAG Chatbot using LangGraph. The chatbot can retrieve information from PDF documents, answer 
user questions using an LLM, perform web search with DuckDuckGo, and use custom tools such as a calculator for utility-based queries.

Steps I followed:
I used PyPDFLoader from langchain_community.document_loaders to load and read PDF documents.
I transformed the extracted PDF text into smaller chunks using RecursiveCharacterTextSplitter from langchain_text_splitters.
I generated vector embeddings for the text chunks and stored them in the FAISS vector store for similarity search.
I set up the LLM using ChatOpenAI from langchain_openai.
I created tools such as DuckDuckGo search, and a calculator tool.
I used StateGraph from LangGraph to build an agentic workflow for handling user queries.
I added conditional tool calling using ToolNode and tools_condition.
I used SqliteSaver checkpointing to store and manage conversation memory.
Finally, I connected the chatbot workflow so it can decide when to answer directly, retrieve PDF context, search the web, or call a custom tool.

# Libraries Used
langchain
langchain-community
langchain-core
langchain-openai
langgraph
langgraph-checkpoint-sqlite
faiss-cpu
pypdf
python-dotenv
requests
duckduckgo-search
streamlit
