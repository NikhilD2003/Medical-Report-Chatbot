# Medical-Report-Chatbot
🔍 Key Features:
Buffer-based Retrieval-Augmented Generation (RAG): Ensures the chatbot maintains context across multiple turns, improving coherence and accuracy for follow-up queries.

LLM: mistralai/mistral-small-3.2-24b-instruct:free: A powerful open-weight model used via LangChain to interpret, analyze, and summarize medical content.

Framework: LangChain: Used for chaining document loaders, retrievers, and the chat interface using modular components.

Document Parsing: Utilizes PyMuPDF (via fitz) for accurate and lightweight PDF text extraction.

Custom Chunking Strategy: Chunks of size 60 tokens with 30-token overlap for preserving sentence integrity and maximizing semantic recall.

Persistent Memory: Stores schema, user queries, and past interactions via a SQL database for long-term memory and improved follow-up handling.

Multilingual Prompt Support (optional): Extendable to multilingual inputs using Hugging Face translation pipelines.

💡 Use Case
This chatbot is especially useful for patients or caregivers trying to understand complex medical documents, or even for doctors who want a quick summary or answer without reading the entire report.

🚀 Future Improvements
Add voice input/output support.

Fine-tuned model for Indian medical terminology.

Integration with Weaviate for semantic search.
