# Apna MEET – Zoom Clone | Full Stack SDE Assignment

A production-ready **Zoom-inspired Video Conferencing Platform** built as a Full Stack Web Application. The application replicates the core meeting workflow of Zoom, allowing users to create instant meetings, join meetings using a unique meeting ID or invite link, manage meeting history, and experience real-time video communication through WebRTC.

**Live Demo:** <YOUR_DEPLOYMENT_LINK>

**GitHub Repository:** https://github.com/Kavish-Paraswar/Apna-MEET

---

# Assignment Overview

This project was developed to satisfy the requirements of the **Full Stack Software Development Assignment (Zoom Clone)**.

The primary objective was to recreate Zoom's meeting workflow while maintaining a clean architecture, modular codebase, responsive UI, and scalable backend.

---

# Tech Stack

## Frontend

- React.js
- React Router DOM
- Material UI
- Axios
- Socket.IO Client
- WebRTC

## Backend

- Node.js
- Express.js
- Socket.IO
- MongoDB
- Mongoose
- bcrypt
- JWT Authentication

## Database

- MongoDB Atlas

---

# Assignment Requirements Mapping

## 1. Landing Dashboard ✅

Implemented a professional dashboard inspired by Zoom.

### Features

- Modern responsive interface
- Navigation Bar
- User Authentication
- Create Meeting
- Join Meeting
- Meeting History
- Clean UI similar to Zoom
- Responsive Layout

---

## 2. Instant Meeting Creation ✅

Implemented.

### Features

- Create meeting instantly
- Automatically generates unique Meeting ID
- Creates shareable meeting link
- Redirects directly to meeting room
- Stores meeting activity for logged-in users

---

## 3. Join Meeting ✅

Implemented.

### Features

- Join using Meeting ID
- Join using invite link
- Meeting validation
- Redirect to active meeting
- Real-time participant synchronization

---

## 4. Video Conferencing ✅

Implemented using WebRTC + Socket.IO.

### Features

- Peer-to-peer video calling
- Audio communication
- Multiple participants
- Automatic connection establishment
- Live participant synchronization

---

## 5. Live Chat ✅

Implemented.

### Features

- Real-time messaging
- Instant updates
- Socket.IO powered communication
- Meeting-specific conversations

---

## 6. Meeting History ✅

Implemented.

### Features

- Stores previously joined meetings
- Displays user meeting history
- Allows quick rejoining of previous meetings

---

## 7. Responsive UI ✅

Implemented.

Supports

- Desktop
- Tablet
- Mobile

Responsive layouts ensure a consistent experience across different screen sizes.

---

# Bonus Features Implemented

- User Authentication
- Secure Password Hashing
- JWT Authentication
- Persistent Login
- Meeting History
- Responsive Design
- Real-time Communication
- Socket.IO Integration
- WebRTC Integration
- MongoDB Database Integration

---

# Application Workflow

```text
User Login
      │
      ▼
Dashboard
      │
      ├──────────────┐
      │              │
      ▼              ▼
New Meeting      Join Meeting
      │              │
      ▼              ▼
Meeting Created   Meeting Validation
      │              │
      └──────┬───────┘
             ▼
      Video Conference
             │
             ▼
        Live Chat
             │
             ▼
       Meeting Ends
             │
             ▼
Meeting History Updated
```

---

# Project Architecture

```text
                React Frontend
                      │
             REST APIs + Socket.IO
                      │
               Express Backend
                      │
       ┌──────────────┴──────────────┐
       │                             │
   MongoDB Database             Socket.IO
                                      │
                                 WebRTC Signaling
                                      │
                              Peer-to-Peer Video
```

---

# Folder Structure

```text
Apna-MEET

├── frontend
│   ├── public
│   ├── src
│   │   ├── components
│   │   ├── pages
│   │   ├── context
│   │   ├── utils
│   │   └── assets
│   └── package.json
│
├── backend
│   ├── controllers
│   ├── middleware
│   ├── models
│   ├── routes
│   ├── socket
│   ├── database
│   └── server.js
│
└── README.md
```

---

# Database Design

## User Collection

| Field | Description |
|--------|-------------|
| name | User Name |
| username | Unique Username |
| password | Encrypted Password |
| createdAt | Creation Timestamp |

---

## Meeting Activity Collection

| Field | Description |
|--------|-------------|
| userId | User Reference |
| meetingCode | Meeting ID |
| joinedAt | Timestamp |

---

# Core Functionalities

## Authentication

- Register
- Login
- Secure password hashing
- JWT Authentication
- Protected Routes

---

## Meeting Management

- Create Meeting
- Join Meeting
- Generate Meeting IDs
- Meeting Validation
- Meeting History

---

## Real-Time Communication

- WebRTC Video Calling
- Socket.IO Signaling
- Live Chat
- Participant Synchronization

---

# API Endpoints

## Authentication

### Register

```http
POST /api/v1/users/register
```

### Login

```http
POST /api/v1/users/login
```

---

## Meeting APIs

### Save Meeting Activity

```http
POST /api/v1/users/add_to_activity
```

### Get Meeting History

```http
GET /api/v1/users/get_all_activity
```

---

# Installation

Clone Repository

```bash
git clone https://github.com/Kavish-Paraswar/Apna-MEET.git
```

Frontend

```bash
cd frontend

npm install

npm start
```

Backend

```bash
cd backend

npm install

npm run dev
```

---

# Environment Variables

Backend

```env
PORT=8000

MONGODB_URI=your_mongodb_connection_string

JWT_SECRET=your_secret_key

CLIENT_URL=http://localhost:3000
```

---

# Deployment

Frontend

- Vercel

Backend

- Render

Database

- MongoDB Atlas

---

# Future Enhancements

- Screen Sharing
- Meeting Scheduling
- Host Controls
- Remove Participants
- Mute All
- Waiting Room
- Meeting Passwords
- File Sharing
- Recording Meetings
- Calendar Integration
- Dark Mode
- Virtual Background
- Breakout Rooms

---

# Assignment Evaluation Checklist

| Requirement | Status |
|-------------|--------|
| Landing Dashboard | ✅ |
| Instant Meeting Creation | ✅ |
| Join Meeting | ✅ |
| Video Conferencing | ✅ |
| Real-Time Chat | ✅ |
| Meeting History | ✅ |
| Responsive UI | ✅ |
| Database Integration | ✅ |
| Clean Code Structure | ✅ |
| Modular Architecture | ✅ |
| REST APIs | ✅ |
| Authentication (Bonus) | ✅ |

---

# Key Highlights

- Zoom-inspired UI and meeting workflow
- Full Stack MERN Architecture
- Secure User Authentication
- Real-Time Video Conferencing using WebRTC
- Socket.IO based signaling and communication
- MongoDB Database Integration
- Responsive Design
- Clean Modular Codebase
- Production-ready Architecture
- Easily Extendable for Future Features

---

# Author

**Kavish Paraswar**

GitHub: https://github.com/Kavish-Paraswar

LinkedIn: https://www.linkedin.com/in/kavish-paraswar/
