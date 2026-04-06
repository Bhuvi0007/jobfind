# 💼 MERN Job Seeking Web App

A full-stack **Job Portal Application** built using the MERN stack (MongoDB, Express, React, Node.js).
This platform allows users to register, login, post jobs, and apply for jobs.

---

# 🚀 Features

* 🔐 User Authentication (JWT + Cookies)
* 🧑‍💼 Job Posting (Employers)
* 📄 Job Applications (Job Seekers)
* 📊 Dynamic Dashboard (Jobs, Categories, Companies)
* ☁️ File Upload (Cloudinary)
* 🌐 REST API Integration
* 🎯 Real-time Data Rendering (No static data)

---

# 🛠️ Tech Stack

* Frontend: React + Vite
* Backend: Node.js + Express
* Database: MongoDB
* Authentication: JWT
* File Uploads: Cloudinary
* HTTP Client: Axios

---

# 📁 Project Structure

```
jobfind/
│
├── backend/
│   ├── config/
│   │   └── config.env
│   ├── controllers/
│   ├── database/
│   ├── models/
│   ├── routes/
│   ├── middlewares/
│   └── server.js
│
├── frontend/
│   ├── src/
│   ├── components/
│   └── main.jsx
```

---

# ⚙️ Environment Variables Setup

## 📍 Step 1: Create `.env` file

Inside:

```
backend/config/config.env
```

---

## 📄 Add the following:

```
# MongoDB Configuration
MONGO_URI=mongodb://127.0.0.1:27017/jobfind

# Frontend URL (CORS)
FRONTEND_URL=http://localhost:5173

# Cookie Expiry
COOKIE_EXPIRE=7

# Cloudinary Configuration
CLOUDINARY_CLIENT_NAME=your_cloud_name
CLOUDINARY_CLIENT_API=your_api_key
CLOUDINARY_CLIENT_SECRET=your_api_secret

# Server Port
PORT=4000

# JWT Configuration
JWT_SECRET_KEY=your_secret_key
JWT_EXPIRE=7d
```

---

# 🗄️ MongoDB Setup

## Option 1: Local MongoDB

1. Install MongoDB
2. Start service:

   ```
   ```

mongod

```
3. Database auto-created on first run

---

## Option 2: MongoDB Atlas (Recommended)

1. Create account on MongoDB Atlas  
2. Create cluster  
3. Get connection string  
4. Replace in `.env`:

```

MONGO_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/jobfind

```

---

# ☁️ Cloudinary Setup

1. Go to https://cloudinary.com  
2. Create account  
3. Copy:
   - Cloud Name
   - API Key
   - API Secret  
4. Paste into `.env`

---

# 📦 Backend Setup

```

cd backend
npm install
npm run dev

```

Server runs at:

```

http://localhost:4000

```

---

# 💻 Frontend Setup

```

cd frontend
npm install
npm run dev

```

Frontend runs at:

```

http://localhost:5173

```

---

# 🔗 API Endpoints

## User Routes

- POST `/api/v1/user/register`
- POST `/api/v1/user/login`
- GET `/api/v1/user/logout`

---

## Job Routes

- GET `/api/v1/job/getall`
- POST `/api/v1/job/post`
- PUT `/api/v1/job/update/:id`
- DELETE `/api/v1/job/delete/:id`

---

## Application Routes

- POST `/api/v1/application/apply`
- GET `/api/v1/application/getall`

---

# 🧪 Testing the App

1. Register a user  
2. Login  
3. Post a job  
4. View jobs  
5. Apply for jobs  

---

# 🧠 Key Concepts Implemented

- RESTful API Design
- JWT Authentication with Cookies
- Role-based Access (Employer / Job Seeker)
- Dynamic UI Rendering from Database
- CORS Handling
- Secure Password Hashing (bcrypt)

---

# 🚨 Common Issues & Fixes

## ❌ CORS Error
✔️ Ensure:
```

methods (not method)
withCredentials: true

```

---

## ❌ MongoDB Not Connecting
✔️ Check:
```

MONGO_URI
dotenv config loaded

```

---

## ❌ Port Already in Use
```

npx kill-port 4000

```

---

## ❌ No Data Showing
✔️ Check DB:
```

db.jobs.find()

```

---

# 🚀 Future Improvements

- 🔍 Job Search & Filters
- 📊 Admin Dashboard
- 📧 Email Notifications
- 🔐 Forgot Password Feature
- 🌍 Deployment (Render / Vercel)

---

# 👨‍💻 Author

**Bhuvan M**

- MERN Stack Developer
- Passionate about AI & Web Development

---

# ⭐ Conclusion

This project demonstrates a complete **full-stack MERN application** with real-world features like authentication, job management, and dynamic UI.

---

🔥 Happy Coding!
```
