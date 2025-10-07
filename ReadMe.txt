# 🏥 Medibot: AI-Powered Medical Chatbot with RAG & LLMs

---

## 📘 Overview
**Medibot** is an AI-powered **medical chatbot** that provides **context-aware answers** using a medical knowledge base.  
It leverages **Large Language Models (LLMs)** integrated with **Retrieval-Augmented Generation (RAG)** to deliver accurate, knowledge-grounded responses.  

The system uses **Hugging Face Transformers** for model architecture and **Groq LLM API** for fast inference.  
A **vector database** stores and retrieves information from a **medical encyclopedia** located in the `data` folder.  

The chatbot is accessible through a **Streamlit UI**, making it interactive and user-friendly.

---

## 🧠 Key Features
- Provides **medical-related answers** using a structured knowledge base.  
- Uses **RAG (Retrieval-Augmented Generation)** for accurate, context-aware responses.  
- Combines **Hugging Face Transformers** with **Groq LLM API** for fast, cost-efficient inference.  
- Integrates a **vector database** for memory retrieval from the medical encyclopedia.  
- Interactive **Streamlit frontend** for real-time conversation.

---

## 🛠️ Tools & Technologies
- **Python**  
- **Hugging Face Transformers** (model framework)  
- **Groq LLM API** (model inference)  
- **LangChain / RAG Frameworks**  
- **Vector Databases (FAISS)**  
- **Streamlit**  
- **dotenv** (for environment variable management)  
- **Medical encyclopedia dataset** (stored in the `data` folder)

---

## ⚙️ Setup Instructions

### 1️⃣ Create Environment Variables
Create a `.env` file in your project folder and add your Groq API token:
GROQ_API_TOKEN=your_api_key_here

---

### 2️⃣ Install Dependencies
Run the following commands in your terminal:
pip install uv
uv add -r requirements.txt
💡 Ensure your `requirements.txt` includes packages such as `transformers`, `langchain`, `streamlit`, `faiss-cpu`, `python-dotenv`, etc.

---

### 3️⃣ Initialize Memory and Connect LLM
Run the following scripts sequentially:
uv run create_memory_for_llm.py
uv run connect_memory_with_llm.py
These scripts load the **medical encyclopedia** into the vector database and connect it to the LLM for knowledge retrieval.  

---

### 4️⃣ Launch the Chatbot Interface
Start the Streamlit application to interact with Medibot:
uv run streamlit run medibot.py
Open the provided local URL in your browser to chat with the model in real time.  

---

## 📊 Output
- Medibot delivers **context-aware medical answers** using the knowledge base.  
- Vector database ensures **relevant and accurate information retrieval**.  
- Streamlit UI allows **easy, real-time interaction** with the chatbot.
