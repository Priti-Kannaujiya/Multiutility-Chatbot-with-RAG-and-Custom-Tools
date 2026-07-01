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
1. Built the chatbot workflow using LangGraph.
2. Used ChatOpenAI to generate intelligent responses.
3. Loaded PDF documents using PyPDFLoader.
4. Split PDF text into chunks using RecursiveCharacterTextSplitter.
5. Stored document embeddings in the FAISS vector database.
6. Added RAG-based document retrieval for PDF question answering.
7. Added DuckDuckGo search support for web-based queries.
8.Created custom tools like a calculator for utility-based questions.
9. Added SqliteSaver checkpointing to maintain conversation memory.
10. Connected all tools inside an agentic workflow so the chatbot can decide whether to answer directly, search documents, search the web, or use a tool.

