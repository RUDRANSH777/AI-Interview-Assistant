# 🚀 AI Interview Coach

### AI-Powered Interview Preparation Platform Using Local LLMs

![Python](https://img.shields.io/badge/Python-3.10+-blue)
![FastAPI](https://img.shields.io/badge/FastAPI-Backend-green)
![React](https://img.shields.io/badge/React-19-blue)
![TypeScript](https://img.shields.io/badge/TypeScript-5.x-blue)
![Ollama](https://img.shields.io/badge/Ollama-Local%20LLM-orange)
![License](https://img.shields.io/badge/License-MIT-yellow)

AI Interview Coach is an intelligent full-stack interview preparation platform that simulates real-world technical and behavioral interviews using locally hosted Large Language Models (LLMs).

The platform analyzes a candidate's resume and job description, generates personalized interview questions, evaluates responses in real time, and provides detailed performance analytics—all while maintaining complete privacy through local AI inference.

Built with **FastAPI, React, TypeScript, Ollama, DeepSeek, Whisper, OCR, and modern web technologies**, the system delivers an immersive interview experience without relying on expensive cloud-based AI APIs.

---

## ✨ Key Highlights

* 🎯 Personalized interview generation from Resume and Job Description
* 🎙️ Voice-enabled interview experience using Speech-to-Text and Text-to-Speech
* 🧠 AI-powered technical, project-based, and behavioral question generation
* 📊 Real-time answer evaluation with actionable feedback
* 📈 Performance tracking and interview analytics dashboard
* 🎥 Live webcam preview and microphone monitoring
* 🌗 Modern responsive UI with Dark and Light themes
* 🔒 Fully local AI execution using Ollama and DeepSeek
* ⚡ Zero API costs and complete data privacy

---

## 📌 Problem Statement

Interview preparation often lacks personalization, structured feedback, and realistic practice environments. Most existing AI-powered interview platforms depend on cloud-based services that introduce recurring costs and privacy concerns.

AI Interview Coach addresses these challenges by providing a fully local interview preparation platform capable of:

* Understanding candidate profiles through resume analysis
* Interpreting role requirements from job descriptions
* Generating personalized interview questions
* Conducting realistic interview sessions
* Evaluating responses with AI-driven scoring
* Tracking progress across multiple interview attempts

---

## 🏗️ System Architecture

```text
Resume + Job Description
            │
            ▼
   OCR Extraction Layer
            │
            ▼
      FastAPI Backend
            │
 ┌──────────┼──────────┐
 │          │          │
 ▼          ▼          ▼
Interview  Session   Evaluation
 Engine    Manager     Engine
 │
 ▼
DeepSeek LLM (Ollama)
 │
 ▼
React Frontend
 │
 ▼
Analytics Dashboard
```

---

# 🎯 Core Features

## 📄 Resume & Job Description Analysis

Upload resumes and job descriptions in PDF or image format. The system extracts relevant information using OCR and contextual analysis to create a personalized interview experience.

## 🎙️ Voice-Enabled Interviews

* Microsoft Edge Neural Text-to-Speech
* OpenAI Whisper Speech-to-Text
* Voice Activity Detection
* Real-time microphone monitoring

## 🧠 Intelligent Interview Generation

### Introduction Phase

* Self-introduction
* Career background
* Academic journey

### Technical Phase

* Data Structures & Algorithms
* Programming Concepts
* Project Discussions
* Technology-Specific Questions

### Behavioral Phase

* STAR Method Questions
* Leadership Scenarios
* Teamwork Situations
* Problem-Solving Assessments

## 📊 AI-Powered Answer Evaluation

Every response is evaluated on:

* Technical Knowledge
* Problem Solving
* Communication Skills
* Relevance
* Clarity

The candidate receives:

* Numerical Score (0–10)
* Constructive Feedback
* Areas of Improvement
* Suggested Better Responses

## 📈 Performance Analytics Dashboard

Track growth through:

* Overall Interview Score
* Question-Wise Performance
* Technical vs Behavioral Analysis
* Session History
* Performance Trends
* Improvement Tracking

## 🎥 Live Interview Environment

The interview room includes:

* Live webcam feed
* Microphone level visualizer
* Voice and text response options
* Real-time AI interaction

## 🔒 Privacy-First Architecture

Unlike cloud-based solutions:

✅ Resume data never leaves the user's system

✅ Interview responses remain local

✅ No external AI API calls

✅ Zero usage-based costs

All AI inference is performed through Ollama-powered local models.

---

# 🛠️ Technology Stack

## Backend

| Technology    | Purpose                  |
| ------------- | ------------------------ |
| Python 3.10+  | Core Backend             |
| FastAPI       | REST API Server          |
| Ollama        | Local LLM Runtime        |
| DeepSeek-V3   | Interview Intelligence   |
| LangChain     | Prompt Orchestration     |
| Whisper       | Speech Recognition       |
| Edge TTS      | AI Interviewer Voice     |
| Tesseract OCR | Resume Extraction        |
| pdf2image     | PDF Processing           |
| webrtcvad     | Voice Activity Detection |

## Frontend

| Technology    | Purpose                 |
| ------------- | ----------------------- |
| React 19      | Frontend Framework      |
| TypeScript    | Type Safety             |
| Vite          | Build Tool              |
| Tailwind CSS  | Styling                 |
| Framer Motion | Animations              |
| Recharts      | Analytics Visualization |
| React Router  | Navigation              |
| Lucide React  | Icons                   |

---

# 🔄 Interview Workflow

```text
Upload Resume + Job Description
                │
                ▼
      OCR & Content Analysis
                │
                ▼
      Generate Interview Plan
                │
                ▼
      Introduction Phase
                │
                ▼
       Technical Phase
                │
                ▼
      Behavioral Phase
                │
                ▼
      AI-Based Evaluation
                │
                ▼
      Analytics Dashboard
```

---

# ⚙️ Installation

## 1. Install Ollama

```bash
ollama pull deepseek-v3.1:671b-cloud
```

## 2. Clone Repository

```bash
git clone https://github.com/RUDRANSH777/AI-Interview-Assistant.git

cd AI-Interview-Assistant
```

## Backend Setup

```bash
cd backend

pip install -r requirement.txt

uvicorn main:app --reload --host 127.0.0.1 --port 8000
```

## Frontend Setup

```bash
cd frontend

npm install

npm run dev
```

Open:

```text
http://localhost:5173
```

---

# 📖 How to Use

1. Launch the application
2. Upload Resume
3. Upload Job Description
4. Select target role and experience level
5. Generate Interview Plan
6. Start Interview Session
7. Respond through voice or text
8. Receive AI-generated feedback
9. Review analytics dashboard
10. Track improvement over time

---

# 🔌 API Endpoints

## Health Check

```http
GET /api/health
```

## Create Interview Session

```http
POST /api/upload
```

## Continue Interview

```http
POST /api/chat
```

---

# 🧪 Testing

```bash
python test_upload.py

python test_chat.py

python test_pdf2image.py
```

---

# 🚀 Future Enhancements

* User Authentication
* PostgreSQL Integration
* Docker Support
* Coding Interview Module
* ATS Resume Analysis
* RAG-Based Resume Understanding
* Multi-Language Interviews
* Cloud Deployment

---

# 🤝 Acknowledgements

Special thanks to:

* Ollama
* DeepSeek AI
* OpenAI Whisper
* Microsoft Edge TTS
* LangChain

for providing the technologies that made this project possible.

---

# 📜 License

MIT License © 2026 

---

### ⭐ If you found this project useful, consider giving it a star on GitHub!
