# Ganga Collection Website

## Overview
Ganga Collection is an e-commerce platform for selling fashion and lifestyle products. This project includes three parts:
- **Frontend:** User-facing website for browsing and purchasing products.
- **Admin Panel:** Dashboard for managing products, orders, and users.
- **Backend:** API and database handling business logic and data management.

## Tech Stack

### Frontend
- React.js (UI framework)
- Redux (State management)
- Axios (API requests)
- React Router (Navigation)
- Tailwind CSS / Material-UI (Styling)

### Admin Panel
- React.js (UI framework)
- Redux Toolkit (State management)
- Chart.js (Analytics & Reports)
- React Toastify (Notifications)

### Backend
- Node.js (Runtime environment)
- Express.js (Web framework)
- MongoDB (Database)
- Mongoose (ODM for MongoDB)
- JWT (Authentication & Authorization)
- Multer (File uploads)
- Cloudinary (Image storage)

## Features

### User Frontend
- Browse and search products
- User authentication (login/register)
- Add to cart and checkout
- Order tracking system
- Responsive design

### Admin Panel
- Dashboard with statistics
- Manage products (CRUD operations)
- Manage users (CRUD operations)
- Order management and status updates
- Sales reports and analytics

### Backend
- RESTful API with CRUD functionality
- Secure authentication with JWT
- Payment integration (Stripe/Razorpay)
- File uploads for product images
- Role-based access control (User/Admin)

## Installation Guide

### Prerequisites
Ensure you have the following installed:
- Node.js (>= 16.x)
- MongoDB (Local or Atlas Cloud)
- Git
- NPM/Yarn

### Setup Instructions

#### Clone the Repository
```sh
git clone https://github.com/arisErrorCoder/GangaCollections.git
cd ganga-collection
```

#### Backend Setup
```sh
cd backend
npm install
```

Create a `.env` file in `backend` directory:
```
PORT=5000
MONGO_URI=your_mongo_connection_string
JWT_SECRET=your_secret_key
CLOUDINARY_CLOUD_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
```

Start the backend server:
```sh
npm run dev
```

#### Frontend Setup
```sh
cd frontend
npm install
npm start
```

#### Admin Panel Setup
```sh
cd admin
npm install
npm start
```

## Deployment

### Backend (Render/Vercel)
1. Push code to GitHub.
2. Deploy using Render/Vercel.
3. Set environment variables in the hosting platform.

### Frontend & Admin Panel (Vercel/Netlify)
1. Build the React app:
   ```sh
   npm run build
   ```
2. Deploy to Vercel/Netlify.

## API Routes

### Authentication
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - User login
- `GET /api/auth/me` - Get user profile

### Products
- `GET /api/products` - Fetch all products
- `POST /api/products` - Add a new product (Admin)
- `PUT /api/products/:id` - Update product details (Admin)
- `DELETE /api/products/:id` - Delete a product (Admin)

### Orders
- `POST /api/orders` - Place an order
- `GET /api/orders/:id` - Get order details
- `PUT /api/orders/:id` - Update order status (Admin)

## Contributors
- **Your Name** - [GitHub](https://github.com/your-profile)

## License
This project is licensed under the MIT License.