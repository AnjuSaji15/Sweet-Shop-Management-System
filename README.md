Sweet Shop Management System

A full-stack Sweet Shop Management System developed as part of a TDD Kata.
The application allows users to register, log in, view and purchase sweets, while admin users can manage inventory (add, update, delete, restock sweets).

Features
Authentication

User Registration

User Login

JWT-based Authentication

Role-based access (USER / ADMIN)

Sweet Management

View all sweets

Search sweets by name, category, or price range

Purchase sweets (quantity decreases automatically)

Purchase button disabled when out of stock

🛠 Admin Features

Add new sweets

Update sweet details

Delete sweets

Restock sweets

Tech Stack
Backend

Node.js

Express.js

MySQL (SQL Workbench)

JWT Authentication

Frontend

React.js

Axios

Basic responsive UI

Tools

Git & GitHub

Thunder Client / Postman (API testing)

Project Structure
sweet-shop-management-system/
│
├── backend/
│   ├── src/
│   │   ├── routes/
│   │   ├── middleware/
│   │   ├── config/
│   │   └── app.js
│   └── package.json
│
├── frontend/
│   └── sweet-shop-frontend/
│       ├── src/
│       │   ├── components/
│       │   └── App.js
│       └── package.json
│
├── .gitignore
└── README.md

How to Run the Project Locally
Backend Setup
cd backend
npm install
node src/app.js


Backend runs on: http://localhost:5000

Frontend Setup
cd frontend/sweet-shop-frontend
npm install
npm start


Frontend runs on: http://localhost:3000

API Endpoints (Backend)
Authentication

POST /api/auth/register

POST /api/auth/login

Sweets

GET /api/sweets

GET /api/sweets/search

POST /api/sweets (Admin)

PUT /api/sweets/:id (Admin)

DELETE /api/sweets/:id (Admin)

Inventory

POST /api/sweets/:id/purchase

POST /api/sweets/:id/restock (Admin)
