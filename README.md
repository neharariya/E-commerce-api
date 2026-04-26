# E-Commerce REST API

A robust and scalable RESTful API for an e-commerce platform built with Node.js, Express.js, and MongoDB. It provides comprehensive backend services including user authentication, product management, shopping cart operations, order processing, and payment integration.

## 🚀 Features

- **Authentication & Authorization**: Secure user registration and login using JWT (JSON Web Tokens) and Bcrypt password hashing.
- **Role-Based Access Control (RBAC)**: Middleware to protect routes and differentiate between standard users and administrators.
- **Product Management**: Full CRUD operations for products, including filtering by categories and fetching the newest arrivals.
- **Cart Management**: Add products to cart, update quantities, and manage user-specific shopping carts.
- **Order Processing**: Secure order placement and tracking for users.
- **Analytics Dashboard**: Advanced MongoDB aggregation pipelines to calculate monthly revenue and user growth statistics for administrators.
- **Payment Gateway**: Integration with Stripe API to handle secure payment processing.

## 🛠️ Tech Stack

- **Runtime**: Node.js
- **Framework**: Express.js
- **Database**: MongoDB (Mongoose ORM)
- **Security**: JWT (jsonwebtoken), Bcryptjs, Crypto-js
- **Payments**: Stripe

## 📋 Prerequisites

Before you begin, ensure you have the following installed:
- [Node.js](https://nodejs.org/) (v14 or higher)
- [MongoDB](https://www.mongodb.com/) (Local or MongoDB Atlas)
- [Stripe Account](https://stripe.com/) (For payment gateway API keys)

## ⚙️ Environment Variables

Create a `.env` file in the root directory and add the following variables:

```env
MONGO_URL=your_mongodb_connection_string
JWT_SEC=your_jwt_secret_key
STRIPE_KEY=your_stripe_secret_key
PORT=3000
```

## 🚀 Installation & Getting Started

1. **Clone the repository** (if you haven't already):
   ```bash
   git clone <your-github-repo-url>
   cd E_commerce_api
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Start the server** (Development mode):
   ```bash
   npm start
   ```

The server should now be running on `http://localhost:3000`.

## 📂 Folder Structure

```text
├── config/              # Database and API configurations
├── controllers/         # Logic for handling API requests
├── middlewares/         # JWT verification and role checks
├── models/              # Mongoose database schemas
├── routes/              # Express API route definitions
├── index.js             # Main application entry point
└── package.json         # Project dependencies and scripts
```

## 🌐 API Endpoints (Brief Overview)

- **Auth**: `/api/v1/auth/register`, `/api/v1/auth/login`
- **Users**: `/api/v1/users` (CRUD operations, get stats)
- **Products**: `/api/v1/products` (CRUD operations, filter queries)
- **Carts**: `/api/v1/carts` (CRUD operations per user)
- **Orders**: `/api/v1/orders` (Place orders, get monthly income)
- **Payments**: `/api/v1/payment` (Process Stripe payments)

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! 
