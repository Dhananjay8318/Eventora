# Eventora - MERN Stack Event Management Platform

Eventora is a full-stack **MERN (MongoDB, Express.js, React.js, Node.js)** event management platform that allows users to discover, register, and book events. The application includes secure authentication, OTP verification, password hashing, JWT-based authorization, event management, bookings, payments, and separate user and admin dashboards.

## 🚀 Features

### 👤 User Features

* User registration and login
* OTP-based email verification
* Secure password hashing
* JWT-based authentication and authorization
* User profile management
* Browse and search events
* View detailed event information
* Book events
* View booking history
* Payment integration
* Payment success and failure handling
* Responsive user interface

### 🔐 Authentication & Security

* JWT-based authentication
* Protected routes using JWT middleware
* OTP verification for user registration
* Secure password hashing using bcrypt
* Authentication middleware for protected APIs
* Role-based access for users and administrators
* Secure API request handling

### 🛠️ Admin Features

* Admin authentication
* Admin dashboard
* Create events
* Update events
* Delete events
* Manage event details
* View and manage bookings
* Manage users and event-related data

### 📅 Event Management

* Create and manage events
* Event title and description
* Event date and time
* Event location
* Event image
* Event capacity
* Event booking system
* Event details page

### 💳 Payment

* Online event booking/payment
* Payment success page
* Payment failure page
* Booking confirmation after successful payment

## 🧑‍💻 Tech Stack

### Frontend

* React.js
* React Router
* JavaScript
* HTML5
* CSS3
* Axios
* Responsive UI

### Backend

* Node.js
* Express.js
* MongoDB
* Mongoose
* JWT
* bcrypt
* OTP verification
* REST APIs

### Database

* MongoDB

### Authentication

* JSON Web Token (JWT)
* bcrypt password hashing
* OTP-based verification

## 📁 Project Structure

```text
Eventora-MERN/
│
├── backend/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── config/
│   ├── utils/
│   ├── server.js
│   └── package.json
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── assets/
│   │   ├── App.jsx
│   │   └── main.jsx
│   ├── public/
│   └── package.json
│
├── .gitignore
└── README.md
```

## 🔑 Authentication Flow

```text
User Registration
       ↓
Enter User Details
       ↓
OTP Sent to Email
       ↓
OTP Verification
       ↓
Password Hashed using bcrypt
       ↓
User Account Created
       ↓
Login
       ↓
JWT Token Generated
       ↓
Protected Routes
       ↓
JWT Token Verification
```

## 🔒 Security Implementation

Eventora implements multiple security mechanisms:

* Passwords are hashed before storing them in MongoDB.
* JWT tokens are generated after successful authentication.
* Protected routes verify JWT tokens before allowing access.
* OTP verification helps validate user email addresses.
* Middleware is used to protect authenticated APIs.
* Sensitive configuration values are stored using environment variables.

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/Dhananjay8318/Eventora.git
```

### 2. Navigate to the Project

```bash
cd Eventora
```

### 3. Backend Setup

```bash
cd backend
npm install
```

Create a `.env` file inside the backend folder:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
EMAIL_USER=your_email
EMAIL_PASSWORD=your_email_password
```

Start the backend server:

```bash
npm start
```

or, if using nodemon:

```bash
npm run dev
```

### 4. Frontend Setup

Open another terminal:

```bash
cd frontend
npm install
npm run dev
```

The frontend will run on the Vite development server.

## 🌐 API Overview

### Authentication

```text
POST /api/auth/register
POST /api/auth/verify-otp
POST /api/auth/login
```

### User

```text
GET /api/user/profile
PUT /api/user/profile
```

### Events

```text
GET /api/events
GET /api/events/:id
POST /api/events
PUT /api/events/:id
DELETE /api/events/:id
```

### Booking

```text
POST /api/bookings
GET /api/bookings
```

> API routes may vary depending on the current backend implementation.

## 🖥️ Application Modules

### User Module

Users can register, verify their email using OTP, log in securely, browse events, and make bookings.

### Event Module

Users can view available events while administrators can create, update, and delete events.

### Booking Module

Users can book events and view their booking history.

### Admin Module

Administrators can manage events, users, and bookings through the admin dashboard.

### Payment Module

The application provides payment processing along with success and failure handling.

## 📸 Screenshots

Add screenshots of your application here:

```text
screenshots/
├── home.png
├── login.png
├── register.png
├── otp-verification.png
├── events.png
├── event-details.png
├── user-dashboard.png
└── admin-dashboard.png
```

## 🔮 Future Improvements

* Event recommendation system
* Advanced event search and filtering
* QR-code based ticket verification
* Email notifications
* Event reminders
* Real-time notifications
* Analytics dashboard
* Cloud image storage
* Deployment with CI/CD

## 👨‍💻 Author

**Dhananjay Yadav**

GitHub:
https://github.com/Dhananjay8318

## ⭐ Project

If you find this project useful, consider giving the repository a ⭐ on GitHub.

---

**Eventora** - A full-stack MERN event management platform with secure authentication, OTP verification, JWT authorization, password hashing, event booking, payments, and admin management.
