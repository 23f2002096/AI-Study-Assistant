# AI Study Assistant

A full-stack web application designed to help students with their studies using AI-powered features. Built with React, Node.js, Express, and MongoDB.

## 🚀 Features

- **User Authentication**: Secure registration and login system with JWT tokens
- **Student Profile Management**: Track college, branch, semester information
- **AI-Powered Study Assistance**: Get help with study materials and questions
- **Data Visualization**: Track progress with interactive charts
- **Responsive Design**: Modern UI built with TailwindCSS

## 🛠️ Tech Stack

### Frontend
- **React 19** - UI library
- **Vite** - Build tool and dev server
- **TailwindCSS** - Styling
- **React Router** - Client-side routing
- **Axios** - HTTP client
- **Chart.js** - Data visualization
- **React Hook Form** - Form management
- **React Markdown** - Markdown rendering

### Backend
- **Node.js** - Runtime environment
- **Express** - Web framework
- **MongoDB** - Database
- **Mongoose** - ODM for MongoDB
- **JWT** - Authentication
- **Bcrypt** - Password hashing
- **Helmet** - Security headers
- **CORS** - Cross-origin resource sharing
- **Express Rate Limit** - Rate limiting
- **XSS Clean** - XSS protection

## 📁 Project Structure

```
ai-study-assistant/
├── Backend/
│   ├── config/          # Database configuration
│   ├── controllers/     # Route controllers
│   ├── middleware/      # Custom middleware
│   ├── models/          # Mongoose models
│   ├── routes/          # API routes
│   ├── utils/           # Utility functions
│   ├── server.js        # Entry point
│   └── package.json
├── Frontend/
│   ├── public/          # Static assets
│   ├── src/
│   │   ├── assets/      # Images and icons
│   │   ├── App.jsx      # Main app component
│   │   ├── main.jsx     # React entry point
│   │   └── index.css    # Global styles
│   ├── index.html
│   └── package.json
└── README.md
```

## 🚦 Getting Started

### Prerequisites

- Node.js (v18 or higher)
- MongoDB (local instance or MongoDB Atlas)
- npm or yarn

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/23f2002096/AI-Study-Assistant.git
   cd ai-study-assistant
   ```

2. **Install Backend Dependencies**
   ```bash
   cd Backend
   npm install
   ```

3. **Install Frontend Dependencies**
   ```bash
   cd ../Frontend
   npm install
   ```

4. **Environment Setup**

   Create a `.env` file in the `Backend` directory:
   ```env
   PORT=5000
   MONGODB_URI=mongodb://localhost:27017/ai-study-assistant
   JWT_SECRET=your_jwt_secret_key
   FRONTEND_URL=http://localhost:5173
   ```

   Create a `.env` file in the `Frontend` directory:
   ```env
   VITE_API_URL=http://localhost:5000
   ```

### Running the Application

1. **Start MongoDB**
   - Make sure MongoDB is running on your system

2. **Start Backend Server**
   ```bash
   cd Backend
   npm run dev
   ```
   The backend will run on `http://localhost:5000`

3. **Start Frontend Development Server**
   ```bash
   cd Frontend
   npm run dev
   ```
   The frontend will run on `http://localhost:5173`

## 📡 API Endpoints

### Authentication

- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login user (to be implemented)

### User

- `GET /api/user/profile` - Get user profile (to be implemented)
- `PUT /api/user/profile` - Update user profile (to be implemented)

## 🔐 Security Features

- Password hashing with bcrypt
- JWT token authentication
- Helmet for security headers
- CORS configuration
- Rate limiting to prevent abuse
- XSS protection
- Input validation with express-validator

## 🧑‍💻 Development Scripts

### Backend
- `npm run dev` - Start development server with nodemon
- `npm start` - Start production server

### Frontend
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run linter

##  Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is licensed under the ISC License.

## 👥 Authors

- Your Name - Initial work

##  Acknowledgments

- Built with React and Express
- Styled with TailwindCSS
- Database powered by MongoDB
