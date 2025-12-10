🌟 Smart Inventory AI 
NLP + Voice Powered Inventory Management System

🚀 Live Demo

Frontend: https://smartinventory-1-p0ss.onrender.com

Backend API: https://smartinventory-l965.onrender.com


🎯 Overview

Smart Inventory AI is an intelligent, modern, voice-enabled inventory management system that uses:

Natural Language Processing (NLP)

Conversational AI (Groq LLaMA 3.3)

Voice Input + Voice Output

MongoDB-based real-time inventory management

Users can simply talk to the AI:

“Add 5 apples at ₹50”
“Show me all electronics”
“Reduce 3 bananas”
“What needs restocking?”

The system automatically updates inventory, detects intent, and gives a professional response — in chat or voice.

✨ Key Features
🤖 AI-Powered NLP Engine

Understands natural sentences.

Performs inventory actions based on user intent.

Supports multi-language text input (English, Marathi, Hindi, etc.).


🎤 Voice Interaction

Voice input using Web Speech API.

AI-generated voice responses.

Real-time conversational mode.


📦 Inventory Management

Add, update, delete and fetch items.

Auto-category detection.

Auto min-stock calculation.

Price averaging logic when adding items.

Low-stock detection.

Total inventory value calculation.


📝 Human-like AI Conversation

Friendly, expressive assistant.

Uses memory to maintain conversation flow.

Small-talk support.



🏗️ Project Architecture
Frontend (React + Tailwind + Web Speech API)
          |
          |  User Commands (text/voice)
          ▼
Backend (Node.js + Express)
          |
          |  Natural Language Command
          ▼
Groq LLaMA 3.3 Model (AI Intent Parser)
          |
          |  Structured JSON Intent
          ▼
MongoDB (Inventory Database)




🔌 API Flow (How the System Works)
1. User sends a message

Through text or voice → React → /api/ai/process

2. Backend sends message to Groq AI

AI returns something like:

[
  {
    "intent": "add_item",
    "item": "apple",
    "quantity": 5,
    "price": 50
  }
]

3. Backend executes database operations

Updates MongoDB accordingly.

4. Backend returns a conversational message

Example:

"Added 5 apples 🍎! Your stock is now 12."

5. Frontend displays it & speaks it

Chat updates + voice output.

🖼️ Screenshots



/screenshots/dashboard.png
/screenshots/chat.png
/screenshots/voice.png

🛠️ Tech Stack
Frontend

React.js

TailwindCSS

Lucide Icons

Web Speech API

Axios

Backend

Node.js

Express.js

MongoDB / Mongoose

Groq LLaMA 3.3 NLP Model

Other

Render (Deployment)

GitHub (Version Control)

⚙️ Installation & Setup
Clone Repo
git clone https://github.com/Omii2510/SmartInventory
cd SmartInventoryAI

Backend Setup
cd backend
npm install


Create .env:

PORT=5000
MONGO_URI=your_mongo_connection_string
GROQ_API_KEY=your_groq_key
GROQ_MODEL=llama-3.3-70b-versatile


Start backend:

npm start

Frontend Setup
cd frontend
npm install
npm run dev

🎯 DFD (Data Flow Diagram)
Level 0 – Context Diagram
User
  ↕ (text/voice commands)
Smart Inventory AI System
  ↕ (database operations)
MongoDB

Level 1 – Detailed Flow
User → Frontend → AI Processor → Groq NLP
Groq NLP → AI Intent → Backend Router → DB Operations → Response to User

📌 Future Enhancements

Full multilingual voice output (Hindi, Marathi, etc.)

Image/barcode scanning

Admin dashboard with analytics

Export inventory reports (PDF/Excel)

Multi-user login system

👨‍💻 Developer

Name
B.Tech CSE • OM SHEDAGE • ROHIT GAIKWAD • PRATHMESH SOSE • SUJIT CHAVAN •JAY ITHAPE

⭐ Support the Project

If you like this project:

⭐ Star the repository on GitHub!
