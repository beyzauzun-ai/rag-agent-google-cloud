# 🎮 RAG Agent Game on Google Cloud

An interactive **Retrieval-Augmented Generation (RAG) Agent** deployed on **Google Cloud Run**, wrapped in a game-like interface.

🚀 This project combines:
- RAG pipeline
- Vector search
- Cloud-native deployment
- Gamified UI experience

---

## 🎬 Demo

![Demo](demo.gif)

---

## 🔗 Live Demo

🎮 Play the game:  
👉 https://agentverse-dungeon-779887056122.us-central1.run.app/

🤖 RAG Agent Endpoint:  
👉 https://scholar-agent-779887056122.us-central1.run.app/

---

## 🧠 What is this project?

This project demonstrates how to build and deploy a **RAG-based AI agent** using Google Cloud.

RAG (Retrieval-Augmented Generation) enhances LLMs by retrieving relevant information before generating responses. :contentReference[oaicite:0]{index=0}

In this project:
- User queries are converted into embeddings
- Relevant documents are retrieved from a vector database
- The model generates context-aware answers

---

## ⚙️ Architecture
```
User Query
↓
Embedding Model
↓
Vector Search (PostgreSQL / Vector DB)
↓
Relevant Context
↓
LLM (Gemini)
↓
Final Answer

```
---

## 🛠️ Tech Stack

- ☁️ Google Cloud Run
- 🤖 Gemini (LLM)
- 🧠 RAG Architecture
- 🗄️ PostgreSQL (Vector Storage)
- 🐳 Docker
- 🔄 Cloud Build
- ⚡ Python

---

## 🚀 Features

- ✅ Semantic search with embeddings  
- ✅ Context-aware AI responses  
- ✅ Cloud-native deployment  
- ✅ Interactive game interface  
- ✅ Scalable API endpoint  

---

## 📂 Project Structure

```
├── data/ # Dataset
├── pipeline/ # RAG pipeline logic
├── scholar/ # Agent logic
├── data_setup.sh # Data preparation
├── set_env.sh # Environment setup
├── init.sh # Initialization
├── cloudbuild.yaml # Build config
```
---

## ⚡ Setup & Run

### 1. Clone repo
```bash
git clone https://github.com/beyzauzun-ai/rag-agent-google-cloud.git
cd rag-agent-google-cloud
```
### 2. Setup environment
bash set_env.sh
### 3. Run locally
python main.pY

##☁️ Deployment
This project is deployed using:

Docker containerization
Google Cloud Build
Cloud Run (serverless deployment)

## 💡 Key Learnings

How RAG systems work end-to-end
Vector search vs keyword search
Deploying AI agents on Google Cloud
Building interactive AI applications

👩‍💻 Author
Beyza Uzun

AI & Data Enthusiast
