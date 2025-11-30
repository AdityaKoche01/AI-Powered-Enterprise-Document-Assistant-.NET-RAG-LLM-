# AI-Powered Enterprise Document Assistant (.NET + RAG + LLM)

This project is a document question-answering system built using .NET, ChromaDB, React, and LLMs (OpenAI/Qwen). It processes PDF documents, generates embeddings, stores them in ChromaDB, and provides context-based answers through a retrieval-augmented approach.

---

## Features

- Upload and store PDF documents  
- Extract text and split it into smaller chunks  
- Generate embeddings and save them in ChromaDB  
- Retrieve relevant sections using similarity search  
- Use an LLM to answer questions with proper context  
- Simple React interface for uploading files and asking questions  

---

## Tech Stack

**Backend:** .NET 8, ChromaDB, OpenAI/Qwen API  
**Frontend:** React, Vite, TailwindCSS  
**Other:** PDF text extraction libraries, Axios  

---

## Project Structure

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

yaml
Copy code

---

## How It Works

1. User uploads a PDF  
2. Backend extracts text and splits it into small sections  
3. Embeddings are generated and stored in ChromaDB  
4. When a question is asked, relevant chunks are retrieved  
5. The LLM uses those chunks to generate an answer  

---

## Running the Project

### Backend
```bash
cd backend
dotnet restore
dotnet run
Frontend
bash
Copy code
cd frontend
npm install
npm run dev
API Endpoints
Method	Endpoint	Description
POST	/upload	Upload and process PDF
POST	/query	Ask a question
GET	/documents	List stored documents

Use Cases
HR or policy document search

Finance or compliance document lookup

Internal knowledge management

Legal or contract-related queries
