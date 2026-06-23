# MediBook - Doctor Appointment Booking System

MediBook is a full-stack doctor appointment booking web application built using the **MERN Stack** (MongoDB, Express.js, React.js, Node.js). It features three levels of login — **Patient**, **Doctor**, and **Admin** — each with distinct features tailored to their roles.

## 🌐 Live Demo
- **Frontend**: [MediBook](https://medi-book-gamma-seven.vercel.app)
- **Admin Panel**: [MediBook Admin](https://medi-book-pq2s.vercel.app)

## 🛠️ Tech Stack

- **Frontend**: React.js, Tailwind CSS
- **Backend**: Node.js, Express.js
- **Database**: MongoDB Atlas
- **Image Storage**: Cloudinary
- **Authentication**: JSON Web Token (JWT)
- **Payment**: Simulated Payment Flow

## 🔑 Key Features

### Patient
- Create account and login securely with JWT
- Browse and search doctors by specialty name
- Book appointments with available time slots
- View and cancel booked appointments
- Update profile with photo upload

### Doctor
- Login and manage appointments
- View earnings and patient details
- Update profile, fees, and availability status

### Admin
- Add and manage doctor profiles with image upload
- View and manage all appointments
- Dashboard with total doctors, patients, appointments analytics

## 🚀 Project Setup

### Prerequisites
- Node.js installed
- MongoDB Atlas account
- Cloudinary account

### Clone the Repository
```bash
git clone https://github.com/Ankita-2006-gore/MediBook.git
cd MediBook
```

### Install Dependencies
```bash
# Install backend dependencies
cd backend
npm install

# Install frontend dependencies
cd ../frontend
npm install

# Install admin dependencies
cd ../admin
npm install
```

### Environment Variables

Create `.env` file in **backend** folder:
```env
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
CLOUDINARY_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_SECRET_KEY=your_cloudinary_secret_key
ADMIN_EMAIL=your_admin_email
ADMIN_PASSWORD=your_admin_password
PORT=4000
```

Create `.env` file in **frontend** folder:
```env
VITE_BACKEND_URL=http://localhost:4000
```

Create `.env` file in **admin** folder:
```env
VITE_BACKEND_URL=http://localhost:4000
```

### Run the Application

```bash
# Run backend (Terminal 1)
cd backend
npm start

# Run frontend (Terminal 2)
cd frontend
npm run dev

# Run admin panel (Terminal 3)
cd admin
npm run dev
```

## 📁 Folder Structure
MediBook/

├── admin/           # Admin Panel (React.js)
├── backend/         # Backend (Node.js, Express.js)
│   ├── config/      # Database and Cloudinary config
│   ├── controllers/ # API Controllers
│   ├── middlewares/ # Auth middlewares
│   ├── models/      # MongoDB Schemas
│   └── routes/      # API Routes
└── frontend/        # Patient Frontend (React.js)
└── src/
├── assets/
├── components/
├── context/
└── pages/

## 👩‍💻 Developed By

**Ankita Gore**
- GitHub: [Ankita-2006-gore](https://github.com/Ankita-2006-gore)