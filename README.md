# docontips - Online Doctor Appointment Booking System

This is a full-stack MERN (MongoDB, Express.js, React, Node.js) application designed for booking and managing doctor appointments online. It features a user-facing frontend, a doctor panel, and an admin panel to handle all operations.

-----

### 🚀 Live Demo

This project is currently live on Vercel.

**Frontend:**
https://docontips-frontend.vercel.app/

**Admin Panel:**
https://docontips-admin.vercel.app/

-----

### ✨ Features

  * **User Authentication**: Secure user registration and login.
  * **Doctor and Admin Panels**: Separate interfaces for doctors to manage their appointments and for administrators to oversee the entire platform.
  * **Appointment Booking**: Users can browse doctors by specialty and book available time slots.
  * **Online Payments**: Integrated payment gateways using **Stripe** and **Razorpay** for seamless transactions.
  * **Profile Management**: Users and doctors can update their profiles.
  * **Data Management**: Admins can add new doctors, view all appointments, and manage doctor availability.

-----

### 💻 Tech Stack

  * **Frontend**: React, Vite, Tailwind CSS, React Router DOM
  * **Backend**: Node.js, Express.js
  * **Database**: MongoDB
  * **Cloud Services**: Cloudinary for image hosting
  * **Payments**: Stripe and Razorpay
  * **Authentication**: JSON Web Tokens (JWT)
  * **Other Dependencies**: `bcrypt`, `multer`, `validator`

-----

### ▶️ How to Run Locally

Follow these simple steps to set up and run the project on your local machine.

#### Prerequisites

  * Node.js (v14 or higher)
  * npm (v6 or higher)
  * MongoDB (local or cloud instance)
  * Cloudinary, Stripe, and Razorpay accounts to get API keys

#### 1\. Clone the repository

```bash
git clone https://github.com/Leepakshi78/docontips.git
cd docontips
```

#### 2\. Backend Setup

1.  Navigate to the `backend` directory.
    ```bash
    cd backend
    ```
2.  Install the required dependencies.
    ```bash
    npm install
    ```
3.  Create a `.env` file and add your environment variables based on the `backend/.env` file provided.
      - `CURRENCY`
      - `JWT_SECRET`
      - `ADMIN_EMAIL`
      - `ADMIN_PASSWORD`
      - `MONGODB_URI`
      - `CLOUDINARY_NAME`
      - `CLOUDINARY_API_KEY`
      - `CLOUDINARY_SECRET_KEY`
      - `RAZORPAY_KEY_ID`
      - `RAZORPAY_KEY_SECRET`
      - `STRIPE_SECRET_KEY`
4.  Run the backend server.
    ```bash
    npm run server
    ```
    The server will run on port `4000`.

#### 3\. Frontend Setup

1.  Open a new terminal and navigate to the `frontend` directory.
    ```bash
    cd frontend
    ```
2.  Install the required dependencies.
    ```bash
    npm install
    ```
3.  Create a `.env` file and add the following variables based on the `frontend/.env` file provided.
      - `VITE_RAZORPAY_KEY_ID`
      - `VITE_BACKEND_URL=http://localhost:4000`
4.  Run the frontend development server.
    ```bash
    npm run dev
    ```
    The frontend will run on port `5173`.

#### 4\. Admin Panel Setup

1.  Open another new terminal and navigate to the `admin` directory.
    ```bash
    cd admin
    ```
2.  Install the required dependencies.
    ```bash
    npm install
    ```
3.  Create a `.env` file and add the following variables based on the `admin/.env` file provided.
      - `VITE_CURRENCY`
      - `VITE_BACKEND_URL=http://localhost:4000`
4.  Run the admin panel development server.
    ```bash
    npm run dev
    ```
    The admin panel will run on port `5174`.
