# 🎬 BookMyShow Clone — Movie Booking System

A full-stack **Movie Ticket Booking System** inspired by BookMyShow, built using **Django REST Framework** for the backend and a modern frontend.

The platform allows users to browse movies, theaters and shows, select seats, make bookings, complete payments, and manage their bookings.

---

## 🚀 Features

### 👤 User Features

* User Registration & Login
* Secure Authentication
* Browse Movies
* Search Movies
* Filter Movies by:

  * Genre
  * Language
  * Release Date
* View Movie Details
* View Movie Posters
* View Cast & Crew
* Browse Theaters
* View Available Shows
* Select Show Time
* Interactive Seat Selection
* Book Movie Tickets
* Booking Confirmation
* Unique Booking Reference
* Payment Transaction Management
* View Booking History
* Booking Details
* Ticket Information
* Movie Reviews & Ratings

---

## 🎥 Movie Management

The system supports:

* Movie Name
* Description
* Genre
* Language
* Duration
* Release Date
* Movie Poster
* Cast Members
* Trailer / Movie Information
* Movie Ratings

---

 live link :- https://bookshow-kyfwjknb.manus.space

 
## 🏢 Theater Management

Admin can manage:

* Theaters
* Screens
* Screen Capacity
* Seats
* Show Timings
* Movie Shows
* Ticket Prices

---

## 💺 Seat Booking

The booking system includes:

* Seat Layout
* Available Seats
* Selected Seats
* Booked Seats
* Multiple Seat Selection
* Real-time Seat Availability
* Prevention of duplicate seat booking
* Automatic booking amount calculation

---

## 💳 Payment System

The project includes a payment transaction system for movie bookings.

Payment records contain:

* Transaction ID
* Booking Reference
* Amount
* Payment Status
* Payment Date
* Payment Method

> Payment gateway integration can be connected with services such as Razorpay or Stripe for production use.

---

## 🎟️ Booking System

Each successful booking generates a unique booking reference.

Example:

```text
BMS-DEEPALI-001
```

Booking information includes:

* Booking Reference
* User
* Movie
* Theater
* Screen
* Show
* Selected Seats
* Total Amount
* Booking Status
* Payment Status

---

## 🛠️ Technology Stack

### Backend

* Python
* Django
* Django REST Framework
* Django ORM
* SQLite / PostgreSQL
* Django Admin

### Frontend

* React
* Vite
* JavaScript
* HTML5
* CSS3
* Tailwind CSS

### Development Tools

* Git
* GitHub
* VS Code
* Postman

---

## 📁 Project Structure

```text
BookMyShow/
│
├── backend/
│   ├── config/
│   ├── movies/
│   ├── theaters/
│   ├── bookings/
│   ├── payments/
│   ├── reviews/
│   ├── manage.py
│   └── requirements.txt
│
├── frontend/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── vite.config.js
│
├── .gitignore
└── README.md
```

---

## ⚙️ Backend Installation

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd BookMyShow
```

### 2. Create Virtual Environment

```bash
python -m venv venv
```

### 3. Activate Virtual Environment

### Windows

```bash
venv\Scripts\activate
```

### macOS / Linux

```bash
source venv/bin/activate
```

### 4. Install Dependencies

```bash
pip install -r backend/requirements.txt
```

### 5. Run Migrations

```bash
cd backend
python manage.py makemigrations
python manage.py migrate
```

### 6. Create Admin User

```bash
python manage.py createsuperuser
```

### 7. Start Django Server

```bash
python manage.py runserver
```

Backend will run at:

```text
http://127.0.0.1:8000/
```

---

## 💻 Frontend Installation

Open a new terminal:

```bash
cd frontend
npm install
```

Start the development server:

```bash
npm run dev
```

Frontend will normally run at:

```text
http://localhost:5173/
```

---

## 🔐 Django Admin

The project includes Django Admin for managing the complete movie booking system.

Admin can manage:

* Movies
* Genres
* Languages
* Cast Members
* Movie Posters
* Theaters
* Screens
* Seats
* Shows
* Bookings
* Payments
* Reviews
* Users

Admin URL:

```text
http://127.0.0.1:8000/admin/
```

---

## 🗄️ Database Models

The backend contains the following major models:

```text
User
│
├── Booking
│   ├── Show
│   ├── Seat
│   └── PaymentTransaction
│
Movie
├── Genre
├── Language
├── CastMember
└── MoviePoster
│
Theater
└── Screen
    └── Seat
        │
        └── Show
```

---

## 🎬 Sample Movies

The project can be populated with sample movies such as:

* Pathaan
* Jawan
* 3 Idiots
* Stree 2
* Kalki 2898 AD

---

## 🔄 Booking Flow

```text
User
  ↓
Browse Movies
  ↓
Select Movie
  ↓
Select Theater
  ↓
Select Show
  ↓
Select Seats
  ↓
Confirm Booking
  ↓
Payment
  ↓
Booking Confirmation
  ↓
Generate Ticket
```

---

## 🔒 Security

The project follows Django security practices including:

* CSRF Protection
* Password Hashing
* Authentication
* Permission Management
* Secure Database Queries
* Environment Variables for Sensitive Configuration
* API Authentication

Sensitive information such as:

```text
SECRET_KEY
DATABASE_PASSWORD
API_KEYS
PAYMENT_KEYS
```

should be stored in environment variables and should **never be committed to GitHub**.

---

## 🌐 API

The Django backend provides API endpoints for frontend integration.

Typical API categories include:

```text
/api/movies/
/api/theaters/
/api/shows/
/api/bookings/
/api/payments/
/api/reviews/
```

Exact endpoints may vary depending on the implementation.

---

## 🧪 Testing

Run Django tests using:

```bash
python manage.py test
```

For API testing, tools such as Postman can be used.

---

## 📦 Production Deployment

For production deployment, the application can be deployed using:

* Render
* Railway
* AWS
* DigitalOcean
* VPS
* Vercel / Netlify for frontend

Recommended production database:

```text
PostgreSQL
```

---

## 🔧 Environment Variables

Create a `.env` file:

```env
DEBUG=True

SECRET_KEY=your-secret-key

DATABASE_URL=your-database-url

RAZORPAY_KEY_ID=your-key
RAZORPAY_KEY_SECRET=your-secret

CORS_ALLOWED_ORIGINS=http://localhost:5173
```

Never upload `.env` to GitHub.

---

## 📌 Current Project Status

### Backend

* ✅ Django project setup
* ✅ Movie management
* ✅ Theater management
* ✅ Screen management
* ✅ Seat management
* ✅ Show management
* ✅ Booking management
* ✅ Payment transaction model
* ✅ Review system
* ✅ Django Admin

### Frontend

* ✅ Movie browsing
* ✅ Movie details
* ✅ Theater/show selection
* ✅ Seat selection
* ✅ Booking interface
* 🔄 Payment gateway integration
* 🔄 Production deployment

---

## 🚀 Future Improvements

Possible future features:

* Razorpay payment integration
* QR Code ticket generation
* PDF ticket generation
* Email booking confirmation
* SMS notifications
* WhatsApp notifications
* Google / social login
* Location-based theaters
* Movie trailers
* Advanced movie search
* Offers & coupons
* Cashback system
* Multiple cities
* Food & beverage booking
* Real-time seat locking
* Recommendation system
* Mobile responsive improvements

---

## ⚠️ Disclaimer

This project is an **educational / portfolio project inspired by online movie-ticket booking platforms**.

It is not affiliated with or officially connected to BookMyShow.

BookMyShow and its branding are trademarks of their respective owners.

---

## 👩‍💻 Author

**Deepali Dabaria**

Full Stack Developer

### Technologies

```text
Python
Django
Django REST Framework
React
JavaScript
PostgreSQL
HTML
CSS
Git
GitHub
```

---

## ⭐ Support

If you find this project useful, consider giving the repository a ⭐ on GitHub.

---

## 📄 License

This project is intended for educational and portfolio purposes.
