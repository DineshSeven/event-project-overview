# event-project-overview

# Event Management Project – Multi-Repo Setup

This project is composed of three separate repositories:

### 📱 Mobile App (Flutter)
**Repo**: [event-app](https://github.com/DineshSeven/event-app.git)

- Built in Flutter.
- Used by event attendees.
- Connects to backend via REST APIs.

### 🖥️ Admin Panel (Flutter Web)
**Repo**: [event-admin-panel](https://github.com/DineshSeven/event-admin-panel.git)

- Web-based admin dashboard.
- Built in Flutter (web).
- Used for managing events, users, reports.
- Authenticates using backend.

### 🛠️ Backend (Node.js + Express)
**Repo**: [event-backend](https://github.com/DineshSeven/event-backend.git)

- Node.js REST API.
- Handles authentication, events, users, etc.
- Used by both app and admin panel.

---

## 🔗 How They Work Together

- The **Flutter app** and **admin panel** both send requests to the **Node.js backend** (shared API).
- Authentication, user data, event info is synced via the backend.
- APIs are defined using RESTful principles.
- Each frontend app has its own `.env` for backend URLs.

---

## 🧠 Notes for Bolt.new

- These are **three separate repositories**.
- All repos follow clean folder structures (`lib/` in Flutter, `src/` in Node).
- Use this repo (`event-project-overview`) as the root for understanding connections between them.
