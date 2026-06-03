# 🚀 Backend NRApp - Microservices System

Hệ thống backend được xây dựng theo kiến trúc **Microservices** sử dụng các service độc lập để quản lý người dùng, công việc, lịch làm việc, chat realtime và gửi mail.

---

# 🏗️ Architecture

```bash
                ┌──────────────────┐
                │    Frontend      │
                └────────┬─────────┘
                         │
                ┌────────▼─────────┐
                │   API Gateway    │
                └────────┬─────────┘
     ┌───────────────────┼───────────────────┐
     │                   │                   │
┌────▼────┐      ┌──────▼─────┐      ┌──────▼─────┐
│ USER    │      │ TODO       │      │ WORKSCHEDULE│
│ SERVICE │      │ SERVICE    │      │ SERVICE     │
└────┬────┘      └──────┬─────┘      └──────┬─────┘
     │                  │                   │
     └──────────┬───────┴───────────┬───────┘
                │                   │
         ┌──────▼──────┐    ┌──────▼──────┐
         │ MAIL SERVICE│    │ CHAT SERVICE│
         └─────────────┘    └─────────────┘
```

---

# 📦 Services

## 🔐 USER_SERVICE

Quản lý:

* Authentication / Authorization
* JWT
* User profile
* Role & Permission

Repository:
https://github.com/lethanh2006/USER_SERVICE

---

## ✅ TODO_SERVICE

Quản lý:

* Todo
* Task
* Deadline
* Progress tracking

Repository:
https://github.com/lethanh2006/TODO_SERVICE

---

## 📅 WORKSCHEDULE_SERVICE

Quản lý:

* Work schedule
* Calendar
* Shift / timeline
* Schedule management

Repository:
https://github.com/lethanh2006/WORKSCHEDULE_SERVICE

---

## 📧 MAIL_SERVICE

Chức năng:

* Send OTP
* Notification mail
* Verification mail

Repository:
https://github.com/lethanh2006/MAIL_SERVICE

---

## 💬 CHAT_SERVICE

Chức năng:

* Realtime chat
* Socket communication
* Message management

Repository:
https://github.com/lethanh2006/CHAT_SERVICE

---

## 🌐 API_GATEWAY

Chức năng:

* Centralized routing
* Authentication middleware
* Request forwarding
* Security & rate limiting

Repository:
https://github.com/lethanh2006/API-GATEWAY

---

# ⚙️ Tech Stack

* Node.js
* NestJS
* TypeScript
* MongoDB
* Redis
* Socket.IO
* JWT Authentication
* Microservices Architecture

---

# 🚀 Getting Started

## 1. Clone repositories

```bash
git clone https://github.com/lethanh2006/API-GATEWAY
git clone https://github.com/lethanh2006/USER_SERVICE
git clone https://github.com/lethanh2006/TODO_SERVICE
git clone https://github.com/lethanh2006/WORKSCHEDULE_SERVICE
git clone https://github.com/lethanh2006/MAIL_SERVICE
git clone https://github.com/lethanh2006/CHAT_SERVICE
```

---

## 2. Install dependencies

```bash
npm install
```

hoặc

```bash
yarn install
```

---

## 3. Setup environment variables

Tạo file `.env`

Ví dụ:

```env
PORT=3000

MONGO_URI=

JWT_SECRET=

REDIS_HOST=
REDIS_PORT=
```

---

## 4. Run project

```bash
npm run start:dev
```

---

# 📌 Features

* ✅ Microservices architecture
* ✅ API Gateway
* ✅ JWT Authentication
* ✅ Realtime Chat
* ✅ Mail Notification
* ✅ Task Management
* ✅ Schedule Management
* ✅ Scalable system design

---

# 👨‍💻 Author

Thành Lê

GitHub:
https://github.com/lethanh2006
