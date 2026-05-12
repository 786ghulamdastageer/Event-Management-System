# NexusEvents - Event Management System

A full-stack MERN application for managing and discovering events. Users can view events, see detailed information, and create new events.

---

# Technology Stack

| Layer | Technology |
|-------|------------|
| Frontend | React, React Bootstrap, Axios, React Router DOM |
| Backend | Node.js, Express.js |
| Database | MongoDB, Mongoose |
| Tools | Git, GitHub, Postman |

---

# Folder Structure

```text
event-management-system/
│
├── README.md
│
├── backend/
│   ├── config/
│   │   └── db.js
│   ├── models/
│   │   └── Event.js
│   ├── routes/
│   │   └── eventRoutes.js
│   ├── controllers/
│   │   └── eventController.js
│   ├── server.js
│   ├── package.json
│   └── .env
│
└── frontend/
    ├── src/
    │   ├── components/
    │   │   ├── NavbarComponent.js
    │   │   ├── EventCard.js
    │   │   └── Footer.js
    │   ├── pages/
    │   │   ├── Home.js
    │   │   ├── EventDetails.js
    │   │   └── CreateEvent.js
    │   ├── services/
    │   │   └── api.js
    │   └── App.js
    │
    ├── public/
    └── package.json
```

---

# Installation

## Prerequisites

- Node.js installed
- MongoDB installed or MongoDB Atlas account
- Git installed

---

# Step 1: Clone Repository

```bash
git clone https://github.com/your-username/event-management-system.git
cd event-management-system
```

---

# Step 2: Install Backend Dependencies

```bash
cd backend
npm install
```

---

# Step 3: Install Frontend Dependencies

```bash
cd frontend
npm install
```

---

# Step 4: Setup Environment Variables

Create a `.env` file inside the `backend` folder:

```env
PORT=5000
MONGO_URI=mongodb+srv://username:password@cluster.mongodb.net/ems
```

---

# How to Run the Project

## Run Backend

```bash
cd backend
npm start
```

Backend runs on:

```text
http://localhost:5000
```

---

## Run Frontend

Open another terminal:

```bash
cd frontend
npm start
```

Frontend runs on:

```text
http://localhost:3000
```

---

# Access Application

Open browser and visit:

```text
http://localhost:3000
```

---

# Backend API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| GET | `/api/events` | Get all events |
| GET | `/api/events/:id` | Get single event |
| POST | `/api/events` | Create new event |
| PUT | `/api/events/:id` | Update event |
| DELETE | `/api/events/:id` | Delete event |

---

# Sample API Response

```json
{
  "success": true,
  "count": 5,
  "data": [
    {
      "_id": "65abc123def456",
      "title": "Coding Competition",
      "description": "Solve algorithmic problems",
      "date": "2024-12-25",
      "time": "10:00 AM",
      "location": "FAST University",
      "organizer": "CS Department",
      "price": 0
    }
  ]
}
```

---

# Frontend Pages

| Page | Route | Description |
|---|---|---|
| Home | `/` | Displays all events |
| Event Details | `/events/:id` | Shows full event information |
| Create Event | `/create-event` | Form to create event |

---

# Database Schema

## Event Model

| Field | Type | Required |
|---|---|---|
| title | String | Yes |
| description | String | Yes |
| date | Date | Yes |
| time | String | Yes |
| location | String | Yes |
| organizer | String | Yes |
| price | Number | No |
| imageUrl | String | No |

---

# Available Scripts

## Backend

| Command | Description |
|---|---|
| npm start | Start backend server |

---

## Frontend

| Command | Description |
|---|---|
| npm start | Start frontend development server |
| npm run build | Create production build |

---

# Testing with Postman

1. Open Postman
2. Set Base URL:

```text
http://localhost:5000/api
```

3. Test GET Request:

```text
http://localhost:5000/api/events
```

4. Test POST Request using JSON body

---

# Common Issues and Solutions

| Issue | Solution |
|---|---|
| MongoDB connection failed | Check MONGO_URI in .env |
| Port already in use | Change PORT number |
| CORS error | Make sure backend is running |
| Events not loading | Check backend and frontend servers |

---

# Features Implemented

- View all events
- Event details page
- Create new events
- Responsive frontend design
- RESTful API
- MongoDB integration
- React Bootstrap UI

---

# Future Improvements

- User Authentication
- Event Registration
- Search and Filters
- Payment Integration
- Admin Dashboard
- Image Upload System

---

# Deployment

## Backend Deployment

```bash
npm start
```

---

## Frontend Deployment

```bash
npm run build
```

---

# Author

NexusEvents Development Team
