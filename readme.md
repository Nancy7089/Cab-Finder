# Cab-Finder
# 🚖 Uber Clone - MERN Stack

A full-stack ride-hailing app clone inspired by Uber, built using the MERN stack (MongoDB, Express.js, React.js, and Node.js). This project allows users to book rides, track drivers, and simulate a real-time ride experience.

## ✨ Features

### 👥 User
- Sign Up / Log In (JWT Authentication)
- Book a ride (enter pickup and drop location)
- View ride status and track driver location
- Payment method placeholder
- View past rides and ride history

### 🚗 Driver
- Driver sign in
- Accept or reject rides
- Real-time ride tracking
- Update ride status (Arrived, On Trip, Completed)

### 🧑‍💻 Admin
- View all users and drivers
- Manage bookings
- View analytics and dashboard

---

## 🛠️ Tech Stack

| Layer        | Technology              |
|--------------|--------------------------|
| Frontend     | React.js, Tailwind CSS, React Router |
| Backend      | Node.js, Express.js      |
| Database     | MongoDB (Mongoose)       |
| Authentication | JWT + Bcrypt             |
| Maps & Geo   | Mapbox / Google Maps API |
| Real-time    | Socket.IO                |
| Deployment   | Render / Vercel / MongoDB Atlas |

---

## 📁 Folder Structure

```bash
uber-clone/
├── backend/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── config/
│   └── server.js
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── context/
│   │   ├── App.js
│   │   └── index.js
├── .env
├── package.json
├── README.md

⚙️ Setup Instructions

1. Clone the Repository
git clone https://github.com/your-username/uber-clone.git
cd uber-clone

2. Backend Setup
cd backend
npm install

Create a .env file in backend/:

PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret

Run the server:
npm run dev

3. Frontend Setup
cd ../frontend
npm install

Create a .env file in frontend/:
REACT_APP_BACKEND_URL=http://localhost:5000
REACT_APP_MAPBOX_TOKEN=your_mapbox_token

Run the frontend:
npm start
