# 🎓 Intelligent Dialogue System for Postgraduate Program Inquiries

An AI-powered bilingual conversational assistant developed to provide prospective students with instant information about the **MSc in Technologies of Interactive Systems** at the **Aristotle University of Thessaloniki**.

The system combines a modern **React frontend** with a **Rasa Open Source** conversational AI backend, delivering natural language interactions through a stateful API architecture.

---

# 📋 Project Overview

This project was developed to simplify communication between prospective students and the postgraduate program by automating frequently asked questions.

The assistant is capable of providing information about:

- 🎓 Admission requirements
- 📚 Course curriculum
- 📅 Application deadlines
- 💰 Tuition fees
- 🏛️ Program information
- 📞 Contact details
- 🌍 Bilingual conversations (Greek & English)

Using Natural Language Processing (NLP), the chatbot understands user intent, extracts relevant entities, maintains conversational context, and provides accurate responses in real time.

---

# ✨ Features

- 🌍 Greek & English language support
- 🤖 AI-powered conversational assistant
- 🧠 Intent classification
- 🏷️ Entity extraction
- 💬 Context-aware conversations
- ⚡ Custom Rasa actions
- 🔄 REST API communication
- 📝 Markdown message rendering
- 🎨 Interactive quick-reply buttons
- 📱 Responsive React interface

---

# 🏗️ System Architecture

The application is divided into two independent components:

```
Intelligent Dialogue System
│
├── rasa-frontend
│   ├── React
│   ├── Vite
│   ├── Markdown Renderer
│   └── Chat Interface
│
└── rasa-backend
    ├── Rasa Open Source
    ├── Rasa SDK
    ├── Custom Actions
    ├── Intent Classification
    ├── Entity Extraction
    └── REST API
```

The frontend communicates with the backend through the Rasa REST API, while the Rasa SDK executes custom Python actions whenever additional business logic is required.

---

# 🛠️ Technologies Used

### Frontend

- React
- Vite
- JavaScript
- CSS
- Markdown Rendering

### Backend

- Rasa Open Source
- Rasa SDK
- Python
- REST API

### AI & NLP

- Intent Classification
- Entity Recognition
- Dialogue Management
- Context Tracking
- Custom Actions

---

# 📁 Project Structure

```
project-root/
│
├── rasa-frontend/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── vite.config.js
│
└── rasa-backend/
    ├── actions/
    ├── data/
    ├── models/
    ├── domain.yml
    ├── config.yml
    ├── endpoints.yml
    ├── credentials.yml
    └── actions.py
```

---

# 🚀 Backend Setup

Navigate to the backend directory:

```bash
cd rasa-backend
```

## 1. Create a Virtual Environment

```bash
python3 -m venv venv
```

## 2. Activate the Environment

**Linux / macOS**

```bash
source venv/bin/activate
```

**Windows**

```bash
venv\Scripts\activate
```

## 3. Install Dependencies

```bash
pip install --upgrade pip
pip install rasa
```

---

# 🧠 Train the AI Model

Train the conversational model before running the application.

```bash
rasa train
```

---

# ▶️ Run the Rasa Server

Start the Rasa REST server:

```bash
rasa run --enable-api --cors="*"
```

The chatbot API will be available at:

```
http://localhost:5005
```

---

# ⚙️ Run Custom Actions

Open another terminal and execute:

```bash
rasa run actions
```

The Rasa SDK server will start on:

```
http://localhost:5055
```

Custom actions handle dynamic responses and business logic beyond the standard dialogue flow.

---

# 💻 Frontend Setup

Navigate to the frontend directory:

```bash
cd rasa-frontend
```

Install the required packages:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

The web application will be available at:

```
http://localhost:5173
```

---

# 🔄 System Workflow

```
User
 │
 ▼
React Frontend
 │
 ▼
REST API
 │
 ▼
Rasa Open Source
 │
 ├── Intent Classification
 ├── Entity Extraction
 ├── Dialogue Management
 │
 ▼
Custom Actions (Python)
 │
 ▼
Response
 │
 ▼
React Chat Interface
```

---

# 🧠 AI Capabilities

The assistant leverages Rasa's conversational AI framework to provide:

- Intent Classification
- Entity Recognition
- Context Management
- Dialogue State Tracking
- Slot Filling
- Custom Python Actions
- REST API Integration
- Multilingual Conversations

---

# 🎯 Use Cases

The chatbot can answer questions related to:

- Admission process
- Entry requirements
- Tuition fees
- Program curriculum
- Course information
- Academic calendar
- Contact information
- General postgraduate inquiries

---

# 📚 Learning Objectives

This project demonstrates how modern conversational AI systems can be built by combining:

- React for interactive user interfaces
- Rasa Open Source for Natural Language Understanding
- Python for custom backend logic
- REST APIs for frontend-backend communication

It serves as an example of designing and deploying an end-to-end AI chatbot capable of understanding natural language, maintaining conversational context, and providing real-time assistance.

---
