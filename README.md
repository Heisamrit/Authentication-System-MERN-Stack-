# MERN-Stack-Authentication-System

A full-stack authentication system built with the **MERN stack** (MongoDB, Express.js, React, Node.js). This project includes a backend API for user authentication and a React-based frontend for user interaction. It uses **JWT** for secure authentication, **MongoDB Atlas** for data storage, and supports clean development with `.env` configuration.

---

## 🛍️ Table of Contents

* [Project Overview](#project-overview)
* [File Structure](#file-structure)
* [Environment Setup](#environment-setup)
* [Running the Project](#running-the-project)
* [Troubleshooting](#troubleshooting)

---

## 📌 Project Overview

This MERN stack project implements:

* User registration and login
* JWT-based authentication
* Password hashing using `bcryptjs`
* Secure API routes
* MongoDB Atlas integration
* React-based UI

MongoDB Compass is recommended for managing the database visually.

---

## 📁 File Structure

```
MERN-Stack-Authentication-System/
├── backend/
│   ├── config/              # Database connection configuration
│   ├── controller/          # Express controllers for handling API logic
│   ├── models/              # Mongoose models for MongoDB schemas
│   ├── routes/              # Express route definitions
│   ├── .env                 # Backend environment variables
│   ├── index.js             # Express server entry point
│   └── package.json         # Backend dependencies
├── frontend/
│   ├── public/              # Static assets
│   ├── src/                 # React components and pages
│   ├── .env                 # Frontend environment variables
│   └── package.json         # Frontend dependencies
```

---

## ⚙️ Environment Setup

### 🧉 Prerequisites

* Node.js v14.18.0 or above
* MongoDB Atlas account
* MongoDB Compass (optional)
* Homebrew (macOS only, optional)
* Git

---

### 🔧 Step-by-Step Setup

#### 1. Clone the Repository

```bash
git clone https://github.com/Heisamrit/Authentication-System-MERN-Stack-.git
cd Authentication-System-MERN-Stack-
```

#### 2. Backend Setup

```bash
cd backend
touch .env
```

Add to `.env`:

```env
MONGO_URI=<your-mongodb-atlas-connection-string>
JWT_SECRET=<your-jwt-secret>
PORT=5001
```

Then install dependencies:

```bash
npm install
```

#### 3. Frontend Setup

```bash
cd ../frontend
touch .env
```

Add to `.env`:

```env
REACT_APP_API_URL=http://localhost:5001
```

Then install dependencies:

```bash
npm install
```

---

## 🚀 Running the Project

### Start Backend

```bash
cd backend
npm start
```

> Runs on `http://localhost:5001`

### Start Frontend

```bash
cd frontend
npm start
```

> Runs on `http://localhost:3000`

Then open [http://localhost:3000](http://localhost:3000) in your browser to use the app.

---

## 🛠️ Troubleshooting

### Port Already in Use

```bash
lsof -i :5001
kill -9 <PID>
```

Or change the backend port in `.env`.

### MongoDB Compass macOS Issues

* Go to **System Settings > Privacy & Security > Full Disk Access** and add MongoDB Compass.
* Temporarily disable Gatekeeper:

  ```bash
  sudo spctl --master-disable
  ```

### NPM Warnings

Update packages:

```bash
npm install <package>@latest
```

### MongoDB Atlas Not Connecting

* Ensure your **IP is whitelisted** in MongoDB Atlas.
* Double-check your **connection string** in `.env`.


Add screenshots here to show your UI.<img width="826" height="513" alt="Screenshot 2025-07-11 at 7 56 15 PM" src="https://github.com/user-attachments/assets/caef168c-09d2-4eb0-b33f-ad103a5a5731" />

<img width="826" height="513" alt="Screenshot 2025-07-11 at 7 56 21 PM" src="https://github.com/user-attachments/assets/c995382d-decb-4b58-a88c-6ea3f12be210" />

---
 📄 License

MIT License

---

## ✍️ Author

**Amrit Saini**
[GitHub Repo](https://github.com/Heisamrit/Authentication-System-MERN-Stack-)
