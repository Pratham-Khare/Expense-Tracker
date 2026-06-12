# SpendWise 💰

A full-stack MERN application for tracking income and expenses. Users can securely manage their financial records, monitor spending patterns, view financial summaries, and export transaction data to Excel.

---

## Features

### Authentication
- User Registration
- User Login
- JWT-Based Authentication
- Protected Routes

### User Management
- View Profile
- Update Profile Information
- Update Password

### Income Management
- Add Income
- View Income Records
- Update Income Entries
- Delete Income Entries
- Income Overview
- Export Income Data to Excel

### Expense Management
- Add Expenses
- View Expense Records
- Update Expense Entries
- Delete Expense Entries
- Expense Overview
- Export Expense Data to Excel

### Dashboard
- Financial Summary
- Income Overview
- Expense Overview
- Recent Transactions

---

## Tech Stack

### Frontend
- React
- Vite
- JavaScript
- CSS

### Backend
- Node.js
- Express.js

### Database
- MongoDB
- Mongoose

### Authentication
- JSON Web Token (JWT)

---

## Project Structure

```text
SpendWise
│
├── backend
│   ├── config
│   ├── controllers
│   ├── middleware
│   ├── models
│   ├── routes
│   ├── utils
│   └── server.js
│
├── frontend
│   ├── public
│   ├── src
│   │   ├── assets
│   │   ├── components
│   │   ├── pages
│   │   └── utils
│   └── App.jsx
│
└── README.md
```

---

## Installation

### Clone Repository

```bash
git clone https://github.com/your-username/SpendWise.git
cd SpendWise
```

---

## Backend Setup

```bash
cd backend
npm install
```

Create a `.env` file inside the backend directory:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
CLIENT_URL=http://localhost:5173
```

Start the backend server:

```bash
npm start
```

---

## Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

Frontend will run on:

```text
http://localhost:5173
```

---

## API Routes

### User

```http
POST /user/register
POST /user/login
GET  /user/me
PUT  /user/profile
PUT  /user/password
```

### Income

```http
POST   /income/add
GET    /income/get
PUT    /income/update/:id
DELETE /income/delete/:id
GET    /income/overview
GET    /income/downloadexcel
```

### Expense

```http
POST   /expense/add
GET    /expense/get
PUT    /expense/update/:id
DELETE /expense/delete/:id
GET    /expense/overview
GET    /expense/downloadexcel
```

### Dashboard

```http
GET /dashboard
```

---
## Author

**Pratham**

Built as a MERN Stack project for learning and practicing full-stack web development.