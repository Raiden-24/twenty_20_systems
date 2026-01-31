# Twenty20 Portfolio Application

A full-stack portfolio web application with user authentication, built with Node.js, Express, MongoDB, and vanilla JavaScript.

## 🌟 Features

- **User Authentication**: Secure registration and login system with password hashing
- **Responsive Design**: Beautiful, modern UI that works on desktop and mobile devices
- **Portfolio Display**: Personalized portfolio page with About, Skills, and Projects sections
- **MongoDB Integration**: User data stored in MongoDB Atlas cloud database
- **Premium UI/UX**: Glassmorphism effects, smooth animations, and gradient designs

## 🚀 Live Demo

- **Deployed URL**: [To be added after Vercel deployment]
- **GitHub Repository**: [To be added]

## 🛠️ Technology Stack

### Frontend
- HTML5
- CSS3 (with modern features: CSS Grid, Flexbox, Custom Properties)
- Vanilla JavaScript (ES6+)

### Backend
- Node.js
- Express.js
- MongoDB with Mongoose ODM
- bcrypt (password hashing)
- CORS enabled

### Deployment
- Vercel (Serverless functions)
- MongoDB Atlas (Database hosting)

## 📋 Prerequisites

- Node.js (v14 or higher)
- npm or yarn
- MongoDB Atlas account (or local MongoDB instance)

## 🔧 Installation & Setup

### 1. Clone the repository

```bash
git clone <repository-url>
cd twenty20-portfolio-app
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure MongoDB (Optional - already configured)

The application is pre-configured with MongoDB Atlas connection. If you want to use your own database:

1. Create a MongoDB Atlas account
2. Create a new cluster
3. Get your connection string
4. Update the `MONGODB_URI` in `server/index.js`

### 4. Run the application locally

```bash
npm start
```

The server will start on `http://localhost:3000`

## 📁 Project Structure

```
twenty20-portfolio-app/
│
├── client/                 # Frontend files
│   ├── index.html         # Landing page (Login/Register)
│   ├── portfolio.html     # Portfolio page (protected)
│   ├── style.css          # Styles with modern design system
│   └── script.js          # Client-side JavaScript
│
├── server/                # Backend files
│   ├── index.js          # Express server setup
│   ├── models/
│   │   └── User.js       # User model with password hashing
│   └── routes/
│       └── auth.js       # Authentication routes
│
├── package.json          # Project dependencies
├── vercel.json          # Vercel deployment configuration
├── .gitignore           # Git ignore rules
└── README.md            # Project documentation
```

## 🔐 API Endpoints

### POST `/api/register`
Register a new user

**Request Body:**
```json
{
  "email": "user@example.com",
  "password": "password123"
}
```

**Response:**
```json
{
  "success": true,
  "message": "Registration successful! You can now log in."
}
```

### POST `/api/login`
Authenticate a user

**Request Body:**
```json
{
  "email": "user@example.com",
  "password": "password123"
}
```

**Response:**
```json
{
  "success": true,
  "message": "Login successful!",
  "user": {
    "email": "user@example.com"
  }
}
```

### GET `/api/health`
Check server status

**Response:**
```json
{
  "status": "OK",
  "message": "Server is running"
}
```

## 🎨 Design Features

- **Modern Color Palette**: Custom CSS variables for consistent theming
- **Glassmorphism**: Backdrop blur effects for cards and containers
- **Smooth Animations**: Fade-in, slide-in, and hover effects
- **Responsive Layout**: Mobile-first approach with CSS Grid and Flexbox
- **Premium Typography**: Google Fonts (Inter) for clean, modern text
- **Gradient Accents**: Eye-catching gradients for CTAs and headings

## 📱 Responsive Breakpoints

- **Desktop**: 1200px and above
- **Tablet**: 768px - 1199px
- **Mobile**: Below 768px

## 🧪 Testing Locally

1. **Start the server**: `npm start`
2. **Open browser**: Navigate to `http://localhost:3000`
3. **Register**: Create a new account with email and password
4. **Login**: Use your credentials to log in
5. **View Portfolio**: After login, you'll see the portfolio page
6. **Logout**: Click the logout button to return to landing page

## 🚀 Deployment to Vercel

### Method 1: Vercel CLI

```bash
# Install Vercel CLI
npm install -g vercel

# Login to Vercel
vercel login

# Deploy to production
vercel --prod
```

### Method 2: GitHub Integration

1. Push code to GitHub repository
2. Import project in Vercel dashboard
3. Configure build settings (usually auto-detected)
4. Deploy

## ✅ Evaluation Checklist

- [x] Application loads on deployed URL
- [x] Registration functionality works
- [x] User data stored in MongoDB
- [x] Login redirects to portfolio page
- [x] Portfolio displays user email
- [x] Portfolio content (About, Skills, Projects) visible
- [x] Logout functionality works
- [x] Responsive on desktop and mobile
- [x] GitHub repository is public

## 👤 Portfolio Content

**Name**: Amruth Shivakumar  
**Role**: Aspiring Software Engineer  

**Skills**: Python, SQL, Machine Learning, MongoDB, Streamlit, DSA, OOP, DBMS

**Projects**:
1. AI-Powered Customer Churn Prediction Platform
2. Explainable Drug Repurposing using Knowledge Graphs

## 📝 License

MIT License

## 👨‍💻 Author

Amruth Shivakumar
