# 📝 ThinkBoard — MERN Stack Note Taking App


A full-stack note-taking web application where users can **create, update, and delete notes**. Built with the MERN stack and deployed with a live backend and frontend.

🔗 **Live Demo:** [https://mern-thinkboard-rwt9.vercel.app](https://mern-thinkboard-rwt9.vercel.app)  
💻 **GitHub:** [https://github.com/Verma-Siddharth/mern-thinkboard](https://github.com/Verma-Siddharth/mern-thinkboard)

---

## 🚀 Features

- ✅ Create, update, and delete notes with a title and description
- ✅ Fully functional REST API with proper HTTP methods and status codes
- ✅ Rate limiting using Upstash Redis to prevent API abuse
- ✅ Responsive UI that works on mobile and desktop
- ✅ MongoDB Atlas for cloud database storage
- ✅ Full-stack deployment with separate frontend and backend

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | React.js, Vite |
| Backend | Node.js, Express.js |
| Database | MongoDB, Mongoose, MongoDB Atlas |
| Caching / Rate Limiting | Upstash Redis |
| Deployment (Frontend) | Vercel |
| Deployment (Backend) | Railway |

---

## 📁 Project Structure

```
mern-thinkboard/
├── backend/
│   ├── src/
│   │   ├── config/       # Database connection
│   │   ├── models/       # Mongoose schemas
│   │   ├── routes/       # API routes
│   │   └── server.js     # Entry point
│   └── .env              # Environment variables (not committed)
├── frontend/
│   ├── src/
│   │   ├── components/   # Reusable React components
│   │   ├── pages/        # App pages
│   │   └── main.jsx      # Entry point
└── README.md
```

---

## ⚙️ How to Run Locally

### Prerequisites
- Node.js installed
- MongoDB Atlas account (free)
- Upstash account (free)

### 1. Clone the repository
```bash
git clone https://github.com/Verma-Siddharth/mern-thinkboard.git
cd mern-thinkboard
```

### 2. Set up the Backend
```bash
cd backend
npm install
```

Create a `.env` file inside the `backend` folder:
```
MONGO_URI=your_mongodb_connection_string
UPSTASH_REDIS_REST_URL=your_upstash_rest_url
UPSTASH_REDIS_REST_TOKEN=your_upstash_rest_token
NODE_ENV=development
```

Start the backend server:
```bash
npm run dev
```
Server runs on `http://localhost:5001`

### 3. Set up the Frontend
Open a new terminal:
```bash
cd frontend
npm install
npm run dev
```
App runs on `http://localhost:5173`

---

## 🌐 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/notes` | Get all notes |
| GET | `/api/notes/:id` | Get a single note |
| POST | `/api/notes` | Create a new note |
| PUT | `/api/notes/:id` | Update a note |
| DELETE | `/api/notes/:id` | Delete a note |

---

## 💡 What I Learned

- How to build and structure a **RESTful API** with Node.js and Express
- Connecting a backend to **MongoDB Atlas** using Mongoose
- Implementing **rate limiting** with Redis to protect APIs from abuse
- Managing **environment variables** to keep sensitive data secure
- Configuring **CORS** to allow secure communication between frontend and backend
- **Deploying** a full-stack app with separate frontend and backend services
- Understanding the difference between **SQL and NoSQL** databases

---

## 📦 Deployment

- **Frontend** deployed on [Vercel](https://vercel.com) → [https://mern-thinkboard-rwt9.vercel.app](https://mern-thinkboard-rwt9.vercel.app)
- **Backend** deployed on [Railway](https://railway.app) → [https://mern-thinkboard-production-7bbc.up.railway.app](https://mern-thinkboard-production-7bbc.up.railway.app)
- Database hosted on **MongoDB Atlas** (cloud)
- Redis hosted on **Upstash** (serverless)

---

## 🙋‍♂️ Author

**Siddharth Verma**  
[GitHub](https://github.com/Verma-Siddharth) • [LinkedIn](https://linkedin.com/in/your-linkedin)

---

> ⭐ If you found this project helpful, feel free to star the repository!