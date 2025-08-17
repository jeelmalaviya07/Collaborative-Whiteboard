# Collaborative Whiteboard 

A real-time collaborative whiteboard built using the MERN stack (MongoDB, Express, React, Node) with Socket.IO for live updates. It allows multiple users to draw, share, and collaborate on the same canvas with authentication, persistence, and sharing features.

---

## ✨ Features

- User authentication (signup/login with JWT - access and refresh Token).
- Create, join, and share whiteboards with your personal room.
- Real-time drawing sync using WebSockets.
- Undo/Redo and customization on tool support on whiteboard.
- Clean React frontend with protected routes.

---

## 🚀 Getting Started

## 1. Clone the repository
```bash
git clone https://github.com/jeelmalaviya07/Collaborative-Whiteboard.git
cd Collaborative-Whiteboard-MERN-Project
```

### 2. Backend setup

```bash
cd backend
npm install
```

* Create a `.env` file:

  ```env
  MONGO_URI=your_mongodb_connection
  JWT_SECRET=your_jwt_secret
  PORT=5000
  ```
* Start server:

  ```bash
  npm run dev
  ```

### 3. Frontend setup

```bash
cd frontend
npm install
npm run dev
```

---

## 📡 API Routes (Backend)

### Auth / User

* `POST /api/users/signup` → Register new user.
* `POST /api/users/login` → Login & receive JWT.
* `GET /api/users/me` → Get current user (protected).

### Whiteboards

* `POST /api/whiteboards/create` → Create new whiteboard.
* `GET /api/whiteboards/user` → Get all whiteboards of logged-in user.
* `GET /api/whiteboards/:id` → Get specific whiteboard.
* `POST /api/whiteboards/join/:id` → Join existing whiteboard.
* `DELETE /api/whiteboards/:id` → Delete a whiteboard.

---

## 🖼 Frontend Highlights

* Login/Signup pages with context-based auth.
* Dashboard to manage and join boards.
* Whiteboard UI with tools, sidebar, and chat integration.
* Protected routes via React Router + custom PrivateRoute.

---

## ⚡ Tech Stack

* Frontend: React, Vite, Context API
* Backend: Node.js, Express.js
* Database: MongoDB (Mongoose)
* Real-time: Socket.IO
* Auth: JWT

---

## 📌 Future Improvements

* Role-based access (host vs participant).
* Export boards as images/PDFs.
* Import image on whiteboard.

---


```
