<div align="center">

# 🚗 CarRental
### Full-Stack MERN Car Rental Booking Platform

[![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)](https://react.dev/)
[![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org/)
[![Express](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)](https://expressjs.com/)
[![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)](https://www.mongodb.com/)
[![Tailwind](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=JSON%20web%20tokens)](https://jwt.io/)
[![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://vercel.com/)

🌐 **[Live Demo →](https://car-rental-sigma-bay.vercel.app/)**

</div>

---

## 📌 About This Project

**CarRental** is a full-stack car rental booking web application built with the **MERN stack** (MongoDB, Express, React, Node.js). Users can browse available cars, check details, pick a location and date, and book a car — while admins manage the entire car inventory and view all bookings through a dedicated dashboard.

The frontend and backend are deployed separately on **Vercel**, with **MongoDB Atlas** as the cloud database.

---

## ✨ Features

| Feature | Description |
|---|---|
| 🔐 Authentication | Secure JWT-based user registration & login |
| 🚘 Car Browsing | Browse all available cars with filters |
| 📍 Booking Flow | Select pickup location, date, and book a car |
| 🧾 My Bookings | Users can view their personal booking history |
| 🛠️ Admin Panel | Add cars, manage inventory, and view all bookings |
| 📱 Responsive UI | Built with React + Tailwind CSS |

---

## 🏗️ Tech Stack

### Application
- **Frontend:** React, React Router, Vite, Tailwind CSS, Axios, Context API
- **Backend:** Node.js, Express.js, JWT Authentication
- **Database:** MongoDB Atlas (Cloud) with Mongoose

### Deployment
| Layer | Platform |
|---|---|
| 🎨 Frontend | Vercel |
| ⚙️ Backend | Vercel |
| 🗄️ Database | MongoDB Atlas |

---

## 📁 Project Structure

```
CarRental/
│
├── client/             # React Frontend
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── context/
│   │   ├── assets/
│   │   ├── App.jsx
│   │   ├── main.jsx
│   └── package.json
│
├── server/             # Node + Express Backend
│   ├── controllers/
│   ├── routes/
│   ├── models/
│   ├── middleware/
│   ├── server.js
│   └── package.json
│
└── README.md
```

---

## 🚀 Getting Started (Local Development)

### Prerequisites
- Node.js v18+
- MongoDB Atlas account

### 1. Clone the repository
```bash
git clone https://github.com/Laxmikant-SB/CarRental.git
cd CarRental
```

### 2. Install dependencies

**Frontend**
```bash
cd client
npm install
```

**Backend**
```bash
cd ../server
npm install
```

### 3. Set up environment variables

**`server/.env`**
```env
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
PORT=4000
```

**`client/.env`**
```env
VITE_BACKEND_URL=http://localhost:4000
```

### 4. Run the app

**Start Backend**
```bash
cd server
npm start
```

**Start Frontend**
```bash
cd client
npm run dev
```

Visit **http://localhost:5173** 🎉

---

## 📦 Build for Production

```bash
cd client
npm run build
```

This generates a production-ready build inside the `dist` folder.

---

## 🔗 API Endpoints

### Auth Routes
| Method | Endpoint | Description |
|---|---|---|
| POST | `/api/auth/register` | Register a new user |
| POST | `/api/auth/login` | Login user |

### Car Routes
| Method | Endpoint | Description |
|---|---|---|
| GET | `/api/cars` | List all cars |
| GET | `/api/cars/:id` | Get car details |
| POST | `/api/cars` | Add a new car (Admin only) |

### Booking Routes
| Method | Endpoint | Description |
|---|---|---|
| POST | `/api/bookings` | Create a new booking |
| GET | `/api/bookings/me` | Get logged-in user's bookings |

---

## 🛡️ Authentication Flow

1. User logs in → Backend generates a JWT
2. Frontend stores the token in `localStorage`
3. The token is sent in the header of every protected request
4. Admin routes are protected via dedicated middleware

---

## ✨ Future Enhancements

- 💳 Payment gateway integration (Razorpay / Stripe)
- 🔍 Advanced car filters (price, brand, fuel type)
- ⭐ Reviews & ratings system
- 🏷️ Coupon / discount system
- 📊 Admin analytics dashboard

---

## 👨‍💻 Author

**Laxmikant Babaleshwar**
GitHub: [@Laxmikant-SB](https://github.com/Laxmikant-SB)

---

## 📄 License

This project is open source and available for learning and personal use.
