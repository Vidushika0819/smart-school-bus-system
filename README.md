# 🚍 SafeGo – Smart School Bus & Safety Monitoring Portal

SafeGo is a full MERN-stack web application designed to improve school bus safety, student monitoring, and trip management.
This system supports parents, drivers, coordinators, and school admins, providing real-time updates, alerts, and bus tracking simulation.

## ⭐ Features

### 👨‍👩‍👧 Parent Portal

View assigned trips

Track bus location (manual update system)

Receive boarding/checkout alerts

Manage student profiles

### 🚌 Coordinator Panel

Update bus location at each stop

Mark student check-in & check-out

Manage trip schedules

Safety alert handling

### 🧑‍🏫 Admin Module

Manage drivers

Manage buses

Create and assign trips

View student activity logs

### 💳 Payment & Cost Handling

Fee calculation

Payment history

Receipt generation

## 🎯 Tech Stack

### Frontend

React.js

Tailwind CSS / Material UI

Axios

Context API / Redux (if used)

### Backend

Node.js

Express.js

JWT authentication

REST API architecture

### Database

MongoDB (Cloud or Local)

## 🚀 Quick Start Guide

### Prerequisites
- **Node.js** (v16 or higher) - [Download here](https://nodejs.org/)
- **MongoDB** (local installation) - [Download here](https://www.mongodb.com/try/download/community)
- **Git** - [Download here](https://git-scm.com/)

### 1. Clone the Repository
```bash
git clone https://github.com/Vidushika0819/SafeGo.git
cd SafeGo
```

### 2. Backend Setup

#### Install Dependencies
```bash
cd backend
npm install
```

#### Database Setup
1. **Start MongoDB** (if using local MongoDB):
   ```bash
   # On Windows (run as Administrator)
   net start MongoDB

   # Or use MongoDB Compass to start the service
   ```

2. **Seed the Database** (optional - creates sample users):
   ```bash
   npm run seed
   ```

#### Environment Configuration
The `.env` file is already configured for local MongoDB. If you want to use MongoDB Atlas instead:
1. Uncomment the Atlas connection string in `backend/.env`
2. Replace with your MongoDB Atlas connection string

#### Start Backend Server
```bash
# Development mode (with auto-restart)
npm run dev

# Or production mode
npm start
```

Backend will run on: `http://localhost:5000`

### 3. Frontend Setup

#### Install Dependencies
```bash
cd ../frontend
npm install
```

#### Start Frontend Development Server
```bash
npm start
```

Frontend will run on: `http://localhost:3000`

### 4. Access the Application

Open your browser and go to: `http://localhost:3000`

## 📋 Default Login Credentials

After running the seed script, you can login with these accounts:

### Admin Account
- **Email:** admin@safego.com
- **Password:** admin123

### Parent Account
- **Email:** parent@safego.com
- **Password:** parent123

### Coordinator Account
- **Email:** coordinator@safego.com
- **Password:** coordinator123

### Driver Account
- **Email:** driver@safego.com
- **Password:** driver123

## 🏗️ Project Structure

```
SafeGo/
├── backend/                 # Node.js/Express API
│   ├── Controllers/         # Route controllers
│   ├── Models/             # MongoDB models
│   ├── Routes/             # API routes
│   ├── __tests__/          # Backend tests
│   ├── app.js              # Main application file
│   ├── package.json        # Backend dependencies
│   └── .env                # Environment variables
├── frontend/               # React application
│   ├── src/
│   │   ├── components/     # React components
│   │   ├── context/        # React context
│   │   └── __tests__/      # Frontend tests
│   ├── public/             # Static assets
│   └── package.json        # Frontend dependencies
└── README.md              # This file
```

## 🧪 Running Tests

### Backend Tests
```bash
cd backend
npm test
```

### Frontend Tests
```bash
cd frontend
npm test
```

## 🔧 Available Scripts

### Backend
- `npm start` - Start production server
- `npm run dev` - Start development server with nodemon
- `npm test` - Run Jest tests
- `npm run seed` - Seed database with sample data

### Frontend
- `npm start` - Start development server
- `npm run build` - Build for production
- `npm test` - Run React tests
- `npm run eject` - Eject from Create React App

## 🌐 API Endpoints

- **Authentication:** `/api/auth`
- **Admin:** `/api/admin`
- **Parent:** `/api/parent`
- **Coordinator:** `/api/coordinator`
- **Driver:** `/api/driver`
- **Children:** `/api/children`
- **Trip Assignments:** `/api/trip-assignments`
- **Buses:** `/api/buses`
- **Trips:** `/api/trips`

## 🐛 Troubleshooting

### Common Issues:

1. **MongoDB Connection Error**
   - Ensure MongoDB is running: `net start MongoDB`
   - Check `.env` file has correct connection string

2. **Port Already in Use**
   - Backend: Change port in `backend/app.js`
   - Frontend: Port 3000 is usually auto-assigned

3. **npm install fails**
   - Clear npm cache: `npm cache clean --force`
   - Delete node_modules and reinstall

4. **CORS Errors**
   - Backend has CORS configured for frontend requests

## 📄 License

This project is released under the MIT License.
See the LICENSE file for more details.

## 👩‍💻 Developer

Vidushika Madhushani
GitHub: Vidushika0819

---
