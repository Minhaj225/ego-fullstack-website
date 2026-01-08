# Full Stack MERN E-Commerce Platform

A robust and scalable e-commerce application built with the MERN stack (MongoDB, Express.js, React, Node.js). This project features a modern storefront for customers and a dedicated admin dashboard for managing products and orders, integrated with secure payment gateways.

## 🚀 Features

### User Features
- **Browse & Filter Products**: Advanced filtering by category, sub-category, and price.
- **Product Details**: View detailed product information, images, and available sizes.
- **Shopping Cart**: Add items to cart, update quantities, and view total cost.
- **Secure Checkout**: Integrated payment gateways (Stripe & Razorpay) for secure transactions.
- **Order History**: Track order status and view past purchases.
- **User Authentication**: Secure login and registration using JWT.

### Admin Features
- **Dashboard**: Overview of application status.
- **Product Management**: Add, edit, and delete products. Support for image uploads via Cloudinary.
- **Order Management**: View customer orders and update shipping statuses (Order Placed, Shipped, Delivered).
- **Inventory Control**: Manage stock and product variants.

## 🛠️ Tech Stack

**Frontend (Store & Admin):**
- React 19
- Vite
- Tailwind CSS
- React Router DOM
- Context API (State Management)

**Backend:**
- Node.js
- Express.js
- Mongoose (ODM)
- JSON Web Token (JWT)
- Bcrypt (Security)

**Integrations:**
- **Database**: MongoDB Atlas
- **Storage**: Cloudinary (Image management)
- **Payments**: Stripe, Razorpay

## 📂 Project Structure

```
├── admin/          # Admin Dashboard (React + Vite)
├── backend/        # API Server (Node/Express)
└── frontend/       # Customer Storefront (React + Vite)
```

## ⚙️ Installation & Setup

### Prerequisites
- Node.js (v18+ recommended)
- MongoDB Connection URI
- Cloudinary Account
- Stripe/Razorpay Account keys

### 1. Backend Setup

Navigate to the backend directory and install dependencies:

```bash
cd backend
npm install
```

Create a `.env` file in the `backend` directory with the following variables:

```env
PORT=4000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
CLOUDINARY_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_SECRET_KEY=your_cloudinary_secret_key
STRIPE_SECRET_KEY=your_stripe_secret_key
RAZORPAY_KEY_ID=your_razorpay_key_id
RAZORPAY_KEY_SECRET=your_razorpay_key_secret
ADMIN_EMAIL=admin@example.com
ADMIN_PASSWORD=securepassword
```

Start the server:

```bash
npm start
# or for development
npm run server
```

### 2. Frontend Setup

Navigate to the frontend directory:

```bash
cd frontend
npm install
```

Create a `.env` file in the `frontend` directory if required (e.g., for API base URL):

```env
VITE_BACKEND_URL=http://localhost:4000
```

Start the frontend application:

```bash
npm run dev
```

### 3. Admin Panel Setup

Navigate to the admin directory:

```bash
cd admin
npm install
```

Create a `.env` file in the `admin` directory:

```env
VITE_BACKEND_URL=http://localhost:4000
```

Start the admin dashboard:

```bash
npm run dev
```

## 🛡️ License

This project is licensed under the ISC License.
