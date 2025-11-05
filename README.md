# 🩺 Healing Hands

A **simple yet powerful Doctor Appointment System** built using **Express.js**, **MongoDB**, and a **React** frontend (production build included).
This project provides a seamless experience for patients, doctors, and admins — from appointment booking to approval and management.

---

## ✨ Features

### 👥 User

* Register and login using **JWT-based authentication**
* Apply to become a doctor
* Book appointments and check doctor availability
* Receive real-time **notifications** for booking updates

### 👨‍⚕️ Doctor

* Get notified when a user books an appointment
* View and manage appointment schedules
* Update appointment status

### 🛡️ Admin

* View all **users** and **doctors**
* Approve or reject doctor applications
* Change account status instantly

---

## ⚙️ Tech Stack

* **Backend:** Node.js, Express.js
* **Database:** MongoDB + Mongoose
* **Frontend:** React (production build served from `client/build`)
* **Auth:** JSON Web Tokens (JWT)

---

## 🚀 Quick Start

### 1️⃣ Install Dependencies

```bash
npm install
```

### 2️⃣ Set Environment Variables

Create a `.env` file in the root directory and add:

```env
MONGO_URL=<your-mongodb-connection-string>
JWT_SECRET=<your-secret-key>
PORT=5000  # optional
```

### 3️⃣ Run the Server

```bash
npm start
```

Your app will run at: **[http://localhost:5000](http://localhost:5000)**

---

## 🧭 API Notes

* **Base Path:** `/api/v1`
* **Auth Header (for protected routes):**

  ```
  Authorization: Bearer <token>
  ```

---

## 🗂️ Project Structure

```
Healing-Hands/
│
├── server.js                 # Entry point
├── config/
│   └── db.js                 # Database connection
│
├── controllers/              # Route controllers (business logic)
├── routes/                   # API routes
├── middlewares/
│   └── authMiddleware.js     # JWT authentication middleware
│
├── models/
│   ├── userModel.js
│   ├── doctorModel.js
│   └── appointmentModel.js
│
└── client/
    └── build/                # Production-ready React frontend
```

---

## 💡 Highlights

* End-to-end system for doctors and patients
* Modular backend with clean architecture
* JWT-secured authentication
* Full admin control panel
* React frontend served directly from Express

---

## 🧑‍💻 Author

**Healing Hands** – Doctor Appointment System
Made with ❤️ using the MERN Stack
