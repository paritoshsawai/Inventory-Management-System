# Inventory Management System

A comprehensive web-based inventory management solution built with MERN stack (MongoDB, Express, React, Node.js) for efficient tracking, management, and reporting of inventory.

## Overview

This Inventory Management System provides businesses with a robust platform to track inventory levels, orders, sales, and deliveries. The system is designed to help optimize stock levels, reduce costs, and improve efficiency in inventory operations.

## Features

- **User Authentication & Authorization**: Secure login system with role-based access control
- **Dashboard**: Visual representation of inventory metrics and KPIs
- **Product Management**: Add, edit, delete, and view products with details
- **Stock Tracking**: Real-time monitoring of inventory levels
- **Order Management**: Create and track purchase orders and sales orders
- **Supplier & Customer Management**: Maintain detailed information about suppliers and customers
- **Reports & Analytics**: Generate comprehensive reports for informed decision-making
- **Barcode/QR Code Integration**: Scan products for quick lookup and updates
- **Low Stock Alerts**: Automated notifications for inventory replenishment
- **Multi-location Support**: Manage inventory across different warehouses/locations

## Technologies Used

### Frontend
- **React.js**: Building the user interface with component-based architecture
- **Redux**: State management for the application
- **Material-UI**: React component library for responsive design
- **Chart.js**: Data visualization for inventory analytics
- **Axios**: API requests handling

### Backend
- **Node.js**: JavaScript runtime environment
- **Express.js**: Web application framework
- **MongoDB**: NoSQL database for data storage
- **Mongoose**: MongoDB object modeling for Node.js
- **JWT**: JSON Web Tokens for authentication
- **bcrypt**: Password hashing for security

### DevOps & Tools
- **Git & GitHub**: Version control and code repository
- **ESLint & Prettier**: Code linting and formatting
- **Jest**: Testing framework
- **Heroku/AWS/Azure**: Deployment platforms (select based on your actual deployment)

## Project Structure

```
inventory-management-system/
├── client/                     # Frontend React application
│   ├── public/                 # Public assets
│   ├── src/
│   │   ├── actions/            # Redux actions
│   │   ├── components/         # Reusable UI components
│   │   ├── layouts/            # Page layouts
│   │   ├── pages/              # Main application pages
│   │   ├── reducers/           # Redux reducers
│   │   ├── services/           # API services
│   │   ├── utils/              # Utility functions
│   │   ├── App.js              # Main application component
│   │   └── index.js            # Entry point
│   └── package.json            # Frontend dependencies
│
├── server/                     # Backend Node.js/Express application
│   ├── config/                 # Configuration files
│   ├── controllers/            # Request handlers
│   ├── middleware/             # Express middleware
│   ├── models/                 # MongoDB Mongoose models
│   ├── routes/                 # API routes
│   ├── utils/                  # Utility functions
│   ├── validation/             # Input validation
│   ├── server.js               # Entry point for the server
│   └── package.json            # Backend dependencies
│
├── .env                        # Environment variables (gitignored)
├── .gitignore                  # Specifies intentionally untracked files
├── README.md                   # Project documentation
└── package.json                # Root dependencies and scripts
```

## Installation & Setup

### Prerequisites
- Node.js (v14+)
- MongoDB (local or Atlas)
- npm or yarn

### Steps to Run Locally

1. Clone the repository
   ```bash
   git clone https://github.com/paritoshsawai/Inventory-Management-System.git
   cd Inventory-Management-System
   ```

2. Install dependencies
   ```bash
   # Install server dependencies
   cd server
   npm install

   # Install client dependencies
   cd ../client
   npm install
   ```

3. Configure environment variables
   - Create a `.env` file in the server directory
   - Add the following variables:
     ```
     PORT=5000
     MONGODB_URI=your_mongodb_connection_string
     JWT_SECRET=your_jwt_secret
     ```

4. Run the application
   ```bash
   # Run backend server
   cd server
   npm run dev

   # In a separate terminal, run frontend
   cd client
   npm start
   ```

5. Access the application at https://inventory-management-system-1dxj3x4u4-paritoshsawais-projects.vercel.app/

## API Documentation

The API is organized around REST. All requests and responses use JSON format.

Base URL: `/api/v1`

### Authentication
- `POST /auth/register` - Register a new user
- `POST /auth/login` - Login user
- `GET /auth/me` - Get current user

### Products
- `GET /products` - Get all products
- `GET /products/:id` - Get product by ID
- `POST /products` - Create a new product
- `PUT /products/:id` - Update product
- `DELETE /products/:id` - Delete product

### Documentation for other endpoints follows similar patterns for:
- Inventory
- Orders
- Suppliers
- Customers
- Reports

## Deployment

The application can be deployed using platforms like Heroku, AWS, or Azure with the following steps:

1. Set up appropriate environment variables
2. Configure the MongoDB connection for production
3. Build the React frontend for production
4. Deploy the Node.js backend server

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## Contact

Paritosh Sawai - [GitHub](https://github.com/paritoshsawai)

Project Link: [https://github.com/paritoshsawai/Inventory-Management-System](https://github.com/paritoshsawai/Inventory-Management-System)
