# RAG Agent with Google Cloud

This project demonstrates an end-to-end Retrieval-Augmented Generation (RAG) system built with Google Cloud.

## Project Overview

The agent uses a vector-based knowledge store to retrieve relevant information and generate context-aware responses.  
It was deployed as a scalable web service using Google Cloud Run and tested through an interactive battle simulation.

## Tech Stack

- Google Cloud Run
- Google Cloud Build
- Cloud SQL for PostgreSQL
- pgvector
- Gemini Embeddings
- Dataflow
- Python

## Features

- Semantic search with vector embeddings
- PostgreSQL + pgvector based knowledge store
- RAG-based response generation
- Cloud Run deployment
- Interactive mini-boss battle demo

## Live Demo

Game UI:  
https://agentverse-dungeon-779887056122.us-central1.run.app/

Agent Endpoint:  
https://scholar-agent-779887056122.us-central1.run.app/

## What I Learned

- How RAG systems retrieve relevant context before generation
- How vector embeddings support semantic search
- How to store and query embeddings with pgvector
- How to build and deploy an AI agent using Google Cloud
- How Cloud Run can serve an AI agent as a scalable web service

## 🚀 Architecture

1. Data is processed and chunked  
2. Text is converted into embeddings using Gemini  
3. Stored in PostgreSQL with pgvector  
4. User query → embedding  
5. Similar documents retrieved  
6. Context passed to LLM → final answer generated
    
## ⚙️ How It Works (RAG Flow)

- **Retrieve:** Convert query to vector & search similar data  
- **Augment:** Add retrieved context to prompt  
- **Generate:** LLM produces final answer  

This approach improves accuracy and reduces hallucinations.

## 📂 Project Structure

pipeline/ # Data processing and embedding
scholar/ # RAG agent logic
data/ # Dataset
