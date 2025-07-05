
# 🎬 Online Movie Booking System

An end-to-end online movie ticket booking platform built using modern web technologies including **Next.js**, **TypeScript**, **Tailwind CSS**, **Node.js**, and **MongoDB**. The platform allows users to browse movies, view showtimes, book tickets, make payments, and manage bookings in a user-friendly interface.

---

## 🚀 Tech Stack

| Layer        | Technology                            |
|--------------|----------------------------------------|
| Frontend     | [Next.js](https://nextjs.org/), [React](https://reactjs.org/), [TypeScript](https://www.typescriptlang.org/), [Tailwind CSS](https://tailwindcss.com/) |
| Backend      | [Node.js](https://nodejs.org/), [Express](https://expressjs.com/) |
| Database     | [MongoDB](https://www.mongodb.com/)   |
| Authentication | JSON Web Tokens (JWT) |

---

## 📦 Features

- 🎥 **Browse Movies**: View currently available movies with posters, ratings, and descriptions.
- 🕒 **Showtimes & Venues**: Check available showtimes, screen types, and seat layouts.
- 🪑 **Seat Booking**: Real-time seat availability and booking with dynamic pricing.
- 🔐 **User Authentication**: Signup, login, JWT-based session handling.


---

## 🛠️ Project Structure

```
/client           # Next.js frontend
  ├── components
  ├── pages
  ├── styles
  └── utils

/server           # Node.js backend
  ├── controllers
  ├── models       # Mongoose schemas
  ├── routes
  ├── middlewares
  └── utils

.env              # Environment configuration
README.md
```

---

## 🧪 Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/movie-booking-app.git
cd movie-booking-app
```

### 2. Setup Environment Variables

Create `.env` files in both `/client` and `/server` folders.

#### `/server/.env`
```env
PORT=5000
MONGO_URI=mongodb+srv://<your_mongo_url>
JWT_SECRET=your_jwt_secret
```

#### `/client/.env.local`
```env
NEXT_PUBLIC_API_URL=http://localhost:5000
```

### 3. Install Dependencies

#### Frontend
```bash
cd client
npm install
```

#### Backend
```bash
cd server
npm install
```

### 4. Run the App

#### Start Backend
```bash
cd server
npm run dev
```

#### Start Frontend
```bash
cd client
npm run dev
```

Visit `http://localhost:3000` to view the app.

---

## 🧩 API Endpoints (Backend)

| Method | Endpoint             | Description                 |
|--------|----------------------|-----------------------------|
| POST   | `/api/auth/register` | Register user               |
| POST   | `/api/auth/login`    | Login user & generate token |
| GET    | `/api/movies`        | Get list of movies          |
| POST   | `/api/bookings`      | Book a ticket               |
| GET    | `/api/bookings/me`   | Get user’s bookings         |

> Admin-specific endpoints are protected via middleware and JWT.


## 📌 Future Improvements

- ✅ Email & SMS Booking Confirmations  
- ✅ Search & Filter Functionality  
- ✅ Multi-language Support  
- ✅ Reviews and Ratings  
- ✅ Loyalty Points & Coupons  

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

