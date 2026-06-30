# Repo-IQ 🚀

An AI-powered GitHub Repository exploration tool built using a **RAG (Retrieval-Augmented Generation)** pipeline. This project dynamically clones a GitHub repository, processes its source files into vector embeddings using **ChromaDB**, and allows you to chat with the codebase using **Google's Gemini AI**.

---

## ✨ Features

- **Dynamic Ingestion**: Pass any public GitHub URL and the pipeline automatically clones, chunks, and vectorizes the codebase.
- **Context-Aware AI Answers**: Ask complex questions about the architecture, logic, or flow of the codebase. The Gemini model will answer using only the context retrieved from the source code.
- **Memory/History Aware**: The AI remembers your previous questions in the session, allowing for conversational follow-ups.
- **Slate-Dark UI**: A stunning, modern, and responsive dark interface built with **React** and **Vite** that communicates seamlessly with the Flask backend.
- **Instant Status Feedback**: Clear visibility into clone status and success feedback directly integrated into the dashboard.

---

## 🛠️ Tech Stack

- **Backend**: Python, Flask, Flask-CORS, LangChain, ChromaDB, Gunicorn
- **AI/LLM**: Google Gemini 2.5 Flash (`langchain-google-genai`)
- **Frontend**: React (Vite), React Router DOM, Axios, CSS3

---

## ⚙️ Installation & Setup

### 1. Clone or Navigate to the Project Directory
```bash
cd Repo-IQ
```

### 2. Backend Setup
1. Navigate to the `backend` folder:
   ```bash
   cd backend
   ```
2. Install Python dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Set up the Environment Variables:
   Create or open a `.env` file in the project root directory (or in the `backend/` directory depending on your runner configuration) and configure your Google Gemini API Key:
   ```env
   GOOGLE_API_KEY=your_actual_api_key_here
   ```

### 3. Frontend Setup
1. Navigate to the `client` folder:
   ```bash
   cd ../client
   ```
2. Install Node dependencies:
   ```bash
   npm install
   ```

---

## 🚀 How to Run

### 1. Start the Backend Server
From the `backend` directory, run:
```bash
python app.py
```
*The server will start on `http://127.0.0.1:5000`.*

### 2. Start the Frontend Dev Server
From the `client` directory, run:
```bash
npm run dev
```
*Vite will start the frontend local server (typically at `http://localhost:5173`). Open this URL in your browser.*

### 3. Analyze a Repository
1. Paste a public GitHub URL into the input field (e.g., `https://github.com/username/project`).
2. Click **Analyze**.
3. Wait for cloning and vector embedding to complete (you'll see an "Analyse complete, you can ask questions about the repo" green message).
4. Start chatting with the codebase!

---

***Made with ❤️ by Team: Chicken Biryani (Deon George, Karthik Krishnan, and Dhanush M)***
***In Association with BeyondPrompt-26 by IEEE CS GECT***
