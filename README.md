# AI-Powered-Enterprise-Document-Assistant-.NET-RAG-LLM-
A production-ready document Q&amp;A system built using .NET, ChromaDB, React, and LLMs (OpenAI/Qwen). The system ingests enterprise PDFs, chunks and embeds content, performs vector similarity search, and generates accurate, context-aware answers with citations.


Features

Upload and store PDF documents

Extract text and split it into meaningful chunks

Generate embeddings and save them in ChromaDB

Search relevant content using similarity search

Use an LLM to generate answers based on retrieved context

Simple React interface for uploading files and asking questions

Tech Stack

Backend: .NET 8, ChromaDB, OpenAI/Qwen API
Frontend: React, Vite, Tailwind
Other: PDF text extraction libraries, Axios

Project Structure
/backend
  /Controllers
  /Services
  /RAG
    Chunker.cs
    Embedder.cs
    VectorStore.cs
    Retriever.cs
    LLMClient.cs

/frontend
  /src
    /components
    /pages
    /api

How It Works

User uploads a PDF

Backend extracts text and splits it into smaller sections

Embeddings are created and stored in ChromaDB

When a user asks a question, the system finds the closest matching chunks

The LLM uses those chunks to generate an answer

Running the Project
Backend
cd backend
dotnet restore
dotnet run

Frontend
cd frontend
npm install
npm run dev

Endpoints
Method	Endpoint	Description
POST	/upload	Upload and process a PDF
POST	/query	Ask a question
GET	/documents	List stored documents
Use Cases

Searching HR or policy documents

Finance or compliance document lookup

Internal knowledge base

Legal or contract-related queries
