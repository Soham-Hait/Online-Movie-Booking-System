<<<<<<< HEAD
# 🎬 Online Movie Booking System

A modern, full-featured online movie ticket booking platform built with **Next.js**, **TypeScript**, **Tailwind CSS**, **Node.js**, and **MongoDB**. This application enables users to browse movies, view showtimes, book seats, apply offers, make secure payments, and manage their bookings—all in a seamless, user-friendly interface.

---

> **Disclaimer:**
> 
> Before running this project, make sure to install all required dependencies for both the frontend and backend. Use the following commands in the respective directories:
> 
> ```bash
> npm install
> # or
> yarn install
> # or
> pnpm install
> ```
> 
> This ensures all necessary packages are available for the project to function correctly.

## 📸 Screenshots

![Screenshot 1](public/Images/Screenshot%202025-07-05%20192244.png)
*Homepage or landing screen of the application.*

![Screenshot 2](public/Images/Screenshot%202025-07-05%20192436.png)
*Movie details or showtimes selection screen.*

![Screenshot 3](public/Images/Screenshot%202025-07-05%20192547.png)
*Seat selection or booking interface.*

![Screenshot 4](public/Images/Screenshot%202025-07-05%20192638.png)
*Booking confirmation or ticket summary screen.*
=======

# 🎬 Online Movie Booking System

An end-to-end online movie ticket booking platform built using modern web technologies including **Next.js**, **TypeScript**, **Tailwind CSS**, **Node.js**, and **MongoDB**. The platform allows users to browse movies, view showtimes, book tickets, make payments, and manage bookings in a user-friendly interface.
>>>>>>> cea2fa71ee275a906440b2bddc16993f4d0070aa

---

## 🚀 Tech Stack

<<<<<<< HEAD
| Layer          | Technology                                                                 |
| -------------- | -------------------------------------------------------------------------- |
| Frontend       | [Next.js](https://nextjs.org/), [React](https://reactjs.org/), [TypeScript](https://www.typescriptlang.org/), [Tailwind CSS](https://tailwindcss.com/) |
| Backend        | [Node.js](https://nodejs.org/), [Express](https://expressjs.com/)          |
| Database       | [MongoDB](https://www.mongodb.com/)                                       |
| Authentication | JSON Web Tokens (JWT), NextAuth                                            |
| Payments       | Razorpay, Stripe (extensible)                                              |

---

## ✨ Features

- 🎥 **Browse Movies**: Discover movies with posters, ratings, genres, and detailed descriptions.
- 🕒 **Showtimes & Cinemas**: View available showtimes, cinema locations, and screen types.
- 🪑 **Seat Selection**: Interactive, real-time seat selection with dynamic pricing.
- 🔐 **User Authentication**: Secure registration, login, and JWT-based session management.
- 🧾 **Booking Management**: View, download, and manage your bookings from a personalized dashboard.
- 💳 **Secure Payments**: Multiple payment methods (Card, UPI, Wallet, Net Banking) with real-time status.
- 🎟️ **Offers & Coupons**: Apply special offers and discount coupons at checkout.
- 🏷️ **Promotions**: Access exclusive deals (e.g., student, couple, first-time user, army discounts).
- 📱 **Responsive UI**: Fully responsive and mobile-friendly design.
- 🛡️ **Admin Controls**: (If enabled) Admin endpoints for managing movies, showtimes, offers, and users.
- 📊 **Analytics & Logging**: (Optional) Track user activity, bookings, and payment status.
- 📨 **Email/SMS Confirmations**: (Planned) Receive booking confirmations and reminders.

---

## 🗂️ Project Structure

```
/app                # Next.js app directory (frontend & API routes)
/components         # Shared React components
/context            # React context providers (e.g., Auth)
/hooks              # Custom React hooks
/lib                # Utility libraries (DB, config, logger, etc.)
/models             # Mongoose schemas (Movie, Booking, User, Payment, etc.)
/public             # Static assets (images, logos)
/styles             # Global styles
/types              # TypeScript type definitions
=======
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
>>>>>>> cea2fa71ee275a906440b2bddc16993f4d0070aa
```

---

<<<<<<< HEAD
## ⚙️ Installation & Setup
=======
## 🧪 Installation and Setup
>>>>>>> cea2fa71ee275a906440b2bddc16993f4d0070aa

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/movie-booking-app.git
cd movie-booking-app
```

<<<<<<< HEAD
### 2. Configure Environment Variables

Create a `.env` file in the project root (or as required by your deployment). **You must set your MongoDB connection string here:**

```
MONGODB_URI=mongodb+srv://<your_mongo_user>:<your_password>@<your_cluster>.mongodb.net/<your_db>?retryWrites=true&w=majority
JWT_SECRET=your_jwt_secret
RAZORPAY_KEY_ID=your_razorpay_key_id
RAZORPAY_KEY_SECRET=your_razorpay_key_secret
# Add any other required environment variables
```

> **Note:** Replace the MongoDB URI placeholder with your actual connection string. You can get this from your [MongoDB Atlas dashboard](https://cloud.mongodb.com/) or your local MongoDB instance.

### 3. Install Dependencies

```bash
npm install
```

### 4. Run the Application

```bash
npm run dev
```

Visit [http://localhost:3000](http://localhost:3000) to view the app.

---

## 🧩 Key API Endpoints

| Method | Endpoint                | Description                  |
|--------|------------------------ |------------------------------|
| POST   | `/api/login`            | User login                   |
| POST   | `/api/register`         | User registration            |
| GET    | `/api/movies`           | List all movies              |
| GET    | `/api/cinemas`          | List all cinemas             |
| POST   | `/api/bookings`         | Book tickets                 |
| GET    | `/api/bookings/me`      | Get user's bookings          |
| POST   | `/api/payments`         | Make a payment               |
| POST   | `/api/coupons`          | Apply a coupon code          |
| GET    | `/api/offers`           | List available offers        |

> **Admin endpoints** are protected and require authentication.

---

## 🚀 Future Enhancements

We are committed to continuously improving the Online Movie Booking System. Planned and upcoming features include:

- 📧 **Email & SMS Booking Confirmations**: Automated notifications for bookings, reminders, and cancellations.
- 🔍 **Advanced Search & Filter**: Enhanced search by genre, language, rating, and more.
- 🌐 **Multi-language Support**: Localized UI for a global audience.
- ⭐ **User Reviews and Ratings**: Share and read feedback on movies and cinemas.
- 🎁 **Loyalty Points & Rewards**: Earn points for bookings and redeem for discounts.
- 🛡️ **Enhanced Admin Dashboard**: Advanced analytics, reporting, and management tools.
- 🏦 **More Payment Integrations**: Support for additional payment gateways and wallets.
- 🧑‍🤝‍🧑 **Group Bookings**: Book tickets for groups with special pricing.
- 🏷️ **Dynamic Offers**: Personalized and time-limited promotions.
- 🏠 **Home Delivery of Tickets**: (Optional) Physical ticket delivery for select locations.
- 🕹️ **Gamification**: Badges, leaderboards, and engagement rewards.

Stay tuned for regular updates and new features!

---

## 📝 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

> **Note:**
> 
> A placeholder for Razorpay payment gateway integration has been added to the project (`/app/api/razorpay/route.ts`). This can be replaced or extended to support any other payment gateway provider as per your requirements.
=======
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
>>>>>>> cea2fa71ee275a906440b2bddc16993f4d0070aa

