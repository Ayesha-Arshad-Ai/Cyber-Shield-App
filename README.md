# 🛡️ CyberShield
### AI-Powered Cyberbullying Detection Platform

CyberShield is a **full-stack AI-powered platform** designed to detect and prevent cyberbullying across user-generated content such as posts, comments, private messages, and images.

The platform integrates **FastAPI backend services, a React frontend, MongoDB storage, and Google Gemini AI moderation** to ensure safer digital interactions.

CyberShield demonstrates how **AI moderation systems can be integrated into social platforms to promote responsible online communication.**

---

# 📌 Overview

CyberShield provides a secure social interaction platform where users can:

- Create and interact with posts
- Communicate via private messaging
- Detect cyberbullying in real time
- Automatically clean toxic language
- Analyze uploaded images for harmful content

All user content passes through an **AI moderation layer before it is published or delivered**.

---

# ✨ Key Features

## 🔐 Secure Authentication
- User signup and login
- JWT-based authentication
- Secure API access
- Profile management

---

## 📝 Social Post System

Users can interact through posts:

- Create text posts
- Upload image posts
- Like and comment on posts
- Search posts across the platform

Before publishing content, CyberShield analyzes posts to detect harmful language.

---

## 🤖 AI Cyberbullying Detection

CyberShield integrates **Google Gemini AI** for real-time moderation.

The system detects:

- harassment
- offensive language
- bullying phrases
- toxic communication

If harmful content is detected:

- the message is blocked
- the user receives safer wording suggestions

---

## 💬 Private Messaging System

CyberShield includes a moderated chat system where users can:

- view other users
- send private messages
- access chat history

All messages pass through AI moderation before delivery.

---

## 🧹 Cyber-Free AI Tools

CyberShield includes AI utilities to clean harmful content.

### Cyber Free Text
Removes toxic language from text and generates safer alternatives.

### Cyber Free Image
Analyzes uploaded images to detect abusive or harmful visual content.

---

# 🧱 System Architecture

```
React Frontend
      │
      │ REST API
      ▼
FastAPI Backend
      │
      │
      ▼
MongoDB Database
      │
      │
      ▼
Gemini AI Moderation Layer
```

---

# 🧰 Technology Stack

| Layer | Technology | Purpose |
|------|------------|---------|
| Frontend | React.js | User interface |
| Styling | Tailwind CSS | UI styling |
| Backend | FastAPI | API framework |
| Database | MongoDB | Data storage |
| AI Moderation | Google Gemini | Cyberbullying detection |
| Authentication | JWT | Secure authentication |

---

# 📂 Project Structure

```
CyberShield
│
├── Backend
│   ├── main.py
│   ├── config.py
│   ├── database.py
│   ├── models.py
│   │
│   ├── routes
│   │   ├── users.py
│   │   ├── posts.py
│   │   ├── chatbot.py
│   │   └── cyber_free.py
│   │
│   └── requirements.txt
│
├── Frontend
│   ├── src
│   │   ├── components
│   │   ├── pages
│   │   ├── App.jsx
│   │   └── main.jsx
│
└── README.md
```

---

# ⚙️ Installation

## Clone Repository

```bash
git clone https://github.com/yourusername/CyberShield.git
cd CyberShield
```

---

# 🖥 Backend Setup

Install dependencies

```bash
pip install -r Backend/requirements.txt
```

Create `.env` file

```
MONGO_URL=your_mongodb_connection
JWT_SECRET=your_secret_key
GEMINI_API_KEY=your_gemini_api_key
```

Run backend server

```bash
cd Backend
uvicorn main:app --reload
```

Backend runs at

```
http://localhost:8000
```

API documentation

```
http://localhost:8000/docs
```

---

# 💻 Frontend Setup

Navigate to frontend folder

```bash
cd Frontend
```

Install dependencies

```bash
npm install
```

Run development server

```bash
npm run dev
```

Frontend runs at

```
http://localhost:3000
```

---

# 🔍 AI Moderation Workflow

```
User Content
     │
     ▼
Gemini AI Analysis
     │
     ▼
Content Classification
     │
 ┌───────────────┐
 │ Harmful?      │
 └───────────────┘
      │        │
      ▼        ▼
Block Content  Allow Content
Suggest safer  Store & Deliver
message
```

---

# 🔒 Security Features

- JWT authentication
- Protected API routes
- AI moderation pipeline
- Prevention of abusive content
- Secure data storage

---

# 🚀 Future Improvements

Planned enhancements:

- Real-time WebSocket chat
- Admin moderation dashboard
- Community reporting system
- Advanced toxicity detection
- Moderation analytics

---

# 👩‍💻 Author

**Ayesha Arshad**

CyberShield – AI Cyber Safety Platform
