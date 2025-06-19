# 🗳️ Live Polling System
Live -- https://poll-client-rouge.vercel.app/
Backend(Render) -- https://poll-server-7bjj.onrender.com

A real-time interactive **polling application** designed for classroom or collaborative environments, where **teachers can create polls** and **students can respond** in real-time. Built using React, Redux, Socket.io, and Express.js.

---

## 🚀 Features

### 👨‍🏫 Teacher Functionality
- ✅ Create new live polls with questions and multiple options.
- ✅ Configure a timer (30/60/90 seconds) for how long students can respond.
- ✅ Mark one or more options as correct.
- ✅ Only allowed to create a new poll **after previous one finishes** (i.e., all students answer or timer ends).
- ✅ View **live poll results** in real-time.
- ✅ Access **past poll history** (persisted).
- ✅ Kick out a student (optional enhancement).
- ✅ Chat with students through the integrated chat system.

### 👨‍🎓 Student Functionality
- ✅ Enter a **unique name per browser tab** (for anonymity, without login).
- ✅ Participate in live polls when available.
- ✅ **Submit answer within 60 seconds**, or it auto-submits and moves to results.
- ✅ View **live poll results** after answering.
- ✅ Interact with teacher and other students via chat.

### 💬 Chat System
- ✅ Integrated chat with real-time messaging using Socket.io.
- ✅ Typing indicator animation.
- ✅ Styled with Tailwind, responsive UI.

---

## 🛠️ Tech Stack

### 🌐 Frontend
- **React.js** – Component-based modern UI
- **Redux Toolkit** – Global state management (auth, role, etc.)
- **Socket.io-client** – Real-time communication with backend
- **React Hook Form + Zod** – Form handling & validation (for file uploads or extensions)
- **Tailwind CSS** – Utility-first responsive styling
- **React TSParticles** – Background animation on Login Page

### 🖥️ Backend
- **Express.js** – REST API for auth, poll history, chat
- **Socket.io** – WebSocket support for live updates and polling
- **MongoDB** – Poll & chat data storage

---

## 📁 Folder Structure Overview
frontend/
├── src/
│ ├── components/ # Shared UI Components
│ ├── pages/ # LoginPage, TeacherLandingPage, etc.
│ ├── features/auth/ # Redux slice for auth state
│ └── assets/ # Images, SVGs
backend/
├── src/
│ ├── controllers/
│ ├── services/
│ ├── routes/
│ ├── config/ # Cloudinary, Redis configs
│ └── socket.js # All socket event handlers


---

## ⚙️ Setup Instructions

### 📦 Prerequisites
- Node.js (v18+)
- MongoDB instance (local or cloud)

---

### 🧑‍💻 1. Clone the Repository(Frontend And Backend)

```bash
git clone https://github.com/PrakharRanjan2909/poll-client.git
git clone https://github.com/PrakharRanjan2909/poll-server.git

```
🔧 2. Backend Setup
```bash
cd poll-server
npm install
```

Make .env and configure:
PORT=3000
MONGODB_URI=mongodb://localhost:27017/pollapp

Start The server
```bash 
npm run dev
```
3. Frontend Setup
```bash 
cd poll-client
npm install
```
Create .env file
VITE_NODE_ENV=development
VITE_API_BASE_URL=http://localhost:3000

```bash 
npm run dev
```


 



