# Food Delivery App - SwiftBite

This repository contains the code for a food delivery application, consisting of a frontend, backend, and admin panel.

## Project Structure

The project is divided into three main parts:

* **frontend:** The user-facing application built with React and Vite.  Allows users to browse menus, add items to their cart, place orders, and view their order history.
* **backend:** The server-side application built with Node.js, Express.js, and MongoDB.  Handles user authentication, database interactions, order processing, and payment integration with Stripe.
* **admin:** A React admin panel built with Vite, providing administrative functionalities for managing food items and orders.


## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

* Node.js and npm (or yarn) installed.
* MongoDB instance running.  Ensure you have set the `MONGO_URL` environment variable to point to your database.
* Stripe account for payment processing. Set the `STRIPE_SECRET_KEY` environment variable with your secret key.
* A method of setting environment variables (`.env` files are recommended).


### Installation

1. **Clone the repository:**

```bash
git clone <repository_url>
```

2. **Navigate to each directory and install dependencies:**

```bash
cd frontend
npm install  # or yarn install

cd ../backend
npm install  # or yarn install

cd ../admin
npm install  # or yarn install
```

3. **Set environment variables:** Create `.env` files in the `frontend`, `backend`, and `admin` directories, populating them with the necessary credentials. Example `backend/.env`:

```
MONGO_URL=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
STRIPE_SECRET_KEY=your_stripe_secret_key
```

4. **Run the backend server:**

```bash
cd backend
npm run server
```

5. **Run the frontend development server:**

```bash
cd ../frontend
npm run dev
```

6. **Run the admin panel development server:**

```bash
cd ../admin
npm run dev
```

You should now have the frontend, backend, and admin panel running on separate ports.  The frontend will connect to the backend API, and the admin panel will also interact with the backend.  The default backend port is 4000;  the frontend and admin panel use the default Vite port (3000).


## Technologies Used

* **Frontend:** React, Vite, React Router, Axios, React Toastify
* **Backend:** Node.js, Express.js, Mongoose, MongoDB, Multer, Stripe, JWT, bcrypt, validator
* **Admin Panel:** React, Vite, React Router, Axios, React Toastify
