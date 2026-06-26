# Prescripto Hospital Management System

Prescripto is a full-stack hospital management web application that connects patients, doctors, and administrators in a single platform. It allows users to browse doctors, book appointments, manage profiles, and handle doctor/admin operations through dedicated dashboards.

## 🌐 Live Demo
🔗 patient dashboard : https://prescripto-frontend-nine-alpha.vercel.app/
🔗 admin dashboard   :   https://prescripto-1vef1u48r-gaurav252003.vercel.app/

---
## Features

- Patient-friendly frontend for browsing doctors and booking appointments
- Secure authentication for users, doctors, and admins
- Doctor dashboard for managing appointments and profile
- Admin dashboard for doctor management and appointment oversight
- Payment integration support with Razorpay and Stripe
- Cloudinary-based media handling
- Responsive UI built with React, Tailwind CSS, and Vite

## Tech Stack

### Frontend
- React
- Vite
- Tailwind CSS
- React Router
- Axios
- React Toastify

### Backend
- Node.js
- Express.js
- MongoDB with Mongoose
- JWT Authentication
- Cloudinary
- Razorpay
- Stripe

## Project Structure

```text
Prescripto/
├── frontend/         # Patient-facing website
├── admin/            # Admin/doctor management panel
├── backend/          # REST API and database logic
├── README.md
```

## Prerequisites

Make sure you have the following installed:

- Node.js (v18 or higher)
- npm or yarn
- MongoDB running locally or a MongoDB Atlas connection string

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/Prescripto.git
cd Prescripto
```

### 2. Backend setup

```bash
cd backend
npm install
cp .env.example .env
```

Update the values in `backend/.env`:

- `PORT`
- `MONGODB_URI`
- `JWT_SECRET`
- `ADMIN_EMAIL`
- `ADMIN_PASSWORD`
- `CURRENCY`
- `STRIPE_SECRET_KEY`
- `RAZORPAY_KEY_ID`
- `RAZORPAY_KEY_SECRET`
- `CLOUDINARY_NAME`
- `CLOUDINARY_API_KEY`
- `CLOUDINARY_SECRET_KEY`

Start the backend server:

```bash
npm run dev
```

The backend will run on `http://localhost:4000`.

### 3. Frontend setup

```bash
cd ../frontend
npm install
cp .env.example .env
```

Update the frontend environment file if required:

```env
VITE_BACKEND_URL=http://localhost:4000
VITE_CURRENCY=INR
VITE_RAZORPAY_KEY_ID=your_razorpay_key_id
```

Start the frontend:

```bash
npm run dev
```

The frontend will run on `http://localhost:5173`.

### 4. Admin panel setup

```bash
cd ../admin
npm install
npm run dev
```

The admin panel will also run with Vite, typically on `http://localhost:5173` (or another port if already in use).

## Environment Notes

- Keep your real secrets in `.env` files.
- Example environment variables are provided in:
  - `backend/.env.example`
  - `frontend/.env.example`

## Usage

- Open the frontend to browse doctors and book appointments.
- Use the admin panel to manage doctors and appointments.
- Doctors can log in and manage their assigned booking schedule.

## Contributing

Contributions are welcome. If you want to improve the project:

1. Fork the repository
2. Create a new branch
3. Make your changes
4. Submit a pull request

## License

This project is intended for educational and personal use. Please check the repository license before commercial deployment.
