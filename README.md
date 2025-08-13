# FuelMech 🚛🔧 - Fuel & Mechanic Service Management System

FuelMech is a full-stack service platform built with **Node.js** and **EJS** that allows fuel stations and mechanic shops to manage their orders, customers, and services. It supports multiple roles: **Admin**, **Fuel Station**, **Mechanic**, and **Users**. The system also includes authentication, order management, profile handling, and Stripe-based payments.

---

```

## 📂 Folder Structure

FuelMech/
├── config/ # Database and environment configs
├── controllers/ # Business logic for each route
│ ├── adminController.js
│ ├── fuelController.js
│ ├── mechanicController.js
│ └── userController.js
├── middlewares/ # Custom middlewares like auth checks
├── models/ # Mongoose models
│ ├── Admin.js
│ ├── FuelStation.js
│ ├── Mechanic.js
│ ├── User.js
│ ├── Order.js
│ └── OTP.js
├── public/ # Static files (CSS, JS, Images)
│ ├── css/
│ ├── js/
│ └── uploads/ # Uploaded profile and product images
├── routes/ # Express route definitions
│ ├── adminRoutes.js
│ ├── fuelRoutes.js
│ ├── mechanicRoutes.js
│ └── userRoutes.js
├── utils/ # Utility functions (e.g., mail, OTP)
├── views/ # EJS templates
│ ├── admin/
│ ├── fuel/
│ ├── mechanic/
│ ├── user/
│ └── partials/
├── .env # Environment variables
├── app.js # Main Express app entry point
├── package.json
└── README.md

```

---

## 🚀 Features

### ✅ Admin Panel

- View, update, and delete (soft & hard) Fuel Stations, Mechanics, and Users
- Role-based access
- Profile management with optional image update
- Real-time order tracking and status management

### ⛽ Fuel Station Panel

- Dashboard with analytics and status-wise order count
- Add/Manage fuel orders and customer details
- View completed and pending orders
- Profile update with image upload

### 🔧 Mechanic Panel

- Dashboard with repair order insights
- Add/Manage mechanic services
- View, accept, and complete service requests
- Profile management

### 👥 User Panel

- Register and Login with OTP-based authentication
- Place orders for fuel or mechanic help
- Stripe-based secure payments
- Track order status

### 📦 Common Features

- Multer file upload for images
- Flash messages for feedback
- Session-based authentication
- Protected routes via middleware
- Mobile-responsive EJS UI
- Clean error handling
- OTP verification for password reset and signup
- Profile picture upload & update

---

## 🔐 Authentication Flow

1. **Signup / Login (OTP):**

   - OTP sent via mail or SMS.
   - Verifies identity and allows access.

2. **Password Reset:**

   - Forgot password → Get OTP → Verify → Reset password.

3. **Session Management:**
   - Sessions and cookies used for login persistence.

---

## 💳 Payment Integration

- Integrated with **Stripe** for online payments.
- Users can pay for fuel or mechanic orders securely.

---

## 🧰 Tech Stack

| Layer       | Technology                 |
| ----------- | -------------------------- |
| Backend     | Node.js, Express.js        |
| Frontend    | EJS, Bootstrap             |
| Database    | MongoDB with Mongoose      |
| Auth        | Passport.js, Sessions, OTP |
| File Upload | Multer                     |
| Payment     | Stripe                     |

---

## 🖼️ UI Preview (Screenshots)

> 💡 Add these screenshot images in a `/screenshots` folder and reference them below.

### 🔑 OTP Verification

![OTP Verification](./screenshots/otp.png)

### 🧾 Fuel Station Dashboard

![Fuel Dashboard](./screenshots/Fuel%20Dashboard.png)

### 📦 Fuel Orders

![Fuel Orders](./screenshots/fuel%20orders.png)

### 📤 Completed Orders

![Completed Orders](./screenshots/fuel%20completed%20order.png)

### ⌛ Pending Orders

![Pending Orders](./screenshots/fuel%20pending%20order.png)

### 👤 Fuel Profile

![Fuel Profile](./screenshots/fuel%20profile.png)

### 🛠 Mechanic Dashboard

![Mechanic Dashboard](./screenshots/Mechanic%20Dashboard.png)

### 💳 Stripe Payment

![Stripe Payment](./screenshots/payment%20stripe.png)

---

## ⚙️ How to Run This Project

### 1. Clone the repository

```bash
git clone https://github.com/your-username/FuelMech.git
cd FuelMech
```

🧪 Testing
Manual form validation

Tested with MongoDB local and cloud (MongoDB Atlas)

Stripe sandbox testing

Auth route protection tested with different roles

🤝 Contribution Guide
If you'd like to contribute:

Fork the repo

Create a new branch (git checkout -b feature-x)

Commit your changes (git commit -m 'Added something')

Push to the branch (git push origin feature-x)

Open a Pull Request

📄 License
MIT License © 2025 ScriptJet

👨‍💻 Developed By
ScriptJet Team
FuelMech is a project by ScriptJet, focused on building real-world service platforms using modern web technologies.
