# 📱 Contact Management System

A modern, full-stack contact management application built with **Express.js**, **MongoDB**, **React**, and **Tailwind CSS**. Features a beautiful, responsive UI with complete CRUD operations and user authentication.

## 🌟 Features

### 🔐 Authentication
- User registration and login
- JWT-based authentication
- Protected routes
- Secure password handling

### 👥 Contact Management
- **Create** new contacts with name, email, and phone
- **Read** and view all contacts with search functionality
- **Update** existing contact information
- **Delete** contacts with confirmation modal
- **Search** contacts by name, email, or phone number

### 🎨 UI/UX
- Modern, dark-themed design with glassmorphism effects
- Fully responsive layout (mobile-first design)
- Beautiful gradient backgrounds and animations
- Toast notifications for user feedback
- Loading states and error handling
- Intuitive navigation with React Router

## 🛠️ Tech Stack

### Backend
- **Node.js** - Runtime environment
- **Express.js** - Web framework
- **MongoDB** - Database
- **Mongoose** - ODM for MongoDB
- **JWT** - Authentication tokens
- **bcrypt** - Password hashing
- **CORS** - Cross-origin resource sharing
- **Express Async Handler** - Error handling

### Frontend
- **React 18** - UI library
- **Vite** - Build tool and dev server
- **React Router DOM** - Client-side routing
- **Tailwind CSS** - Utility-first CSS framework
- **Axios** - HTTP client
- **Lucide React** - Icon library
- **React Hot Toast** - Notifications

## 🚀 Live Demo

- **Frontend**: [https://my-contact-cyan.vercel.app](https://my-contact-cyan.vercel.app)
- **Backend API**: [https://mycontact-rltg.onrender.com](https://mycontact-rltg.onrender.com)

## 📦 Installation & Setup

### Prerequisites
- Node.js (v16 or higher)
- MongoDB Atlas account or local MongoDB
- Git

### Clone Repository
```bash
git clone <your-repo-url>
cd express-project
```

### Backend Setup
```bash
cd backend
npm install
```

Create `.env` file in the backend directory:
```env
PORT=5001
CONNECTION_STRING=mongodb+srv://username:password@cluster.mongodb.net/mycontacts-backend?retryWrites=true&w=majority
ACCESS_TOKEN_SECRET=your-secret-key
FRONTEND_URL=http://localhost:5173
```

Start the backend server:
```bash
npm start
# or for development
npm run dev
```

### Frontend Setup
```bash
cd ../frontend
npm install
```

Create `.env` file in the frontend directory:
```env
VITE_API_URL=http://localhost:5001
```

Start the frontend development server:
```bash
npm run dev
```

## 📁 Project Structure

```
MyContact/
├── backend/
│   ├── config/
│   │   └── dbConnection.js
│   ├── controllers/
│   │   ├── contactController.js
│   │   └── userController.js
│   ├── middleware/
│   │   ├── errorHandler.js
│   │   └── validateTokenHandler.js
│   ├── models/
│   │   ├── contactModel.js
│   │   └── userModel.js
│   ├── routes/
│   │   ├── contactRoutes.js
│   │   └── userRoutes.js
│   ├── constants.js
│   ├── server.js
│   ├── package.json
│   └── .env
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── LoadingSpinner.jsx
│   │   │   ├── Navbar.jsx
│   │   │   └── ProtectedRoute.jsx
│   │   ├── context/
│   │   │   └── AuthContext.jsx
│   │   ├── pages/
│   │   │   ├── ContactDetails.jsx
│   │   │   ├── ContactForm.jsx
│   │   │   ├── Contacts.jsx
│   │   │   ├── Dashboard.jsx
│   │   │   ├── Login.jsx
│   │   │   └── Register.jsx
│   │   ├── services/
│   │   │   └── api.js
│   │   ├── App.jsx
│   │   ├── index.css
│   │   └── main.jsx
│   ├── index.html
│   ├── package.json
│   ├── tailwind.config.js
│   ├── vite.config.js
│   └── .env
└── README.md
```

## 🔧 API Endpoints

### Authentication
- `POST /api/users/register` - Register new user
- `POST /api/users/login` - User login
- `GET /api/users/current` - Get current user info

### Contacts
- `GET /api/contacts` - Get all contacts
- `POST /api/contacts` - Create new contact
- `GET /api/contacts/:id` - Get contact by ID
- `PUT /api/contacts/:id` - Update contact
- `DELETE /api/contacts/:id` - Delete contact

## 🎯 Key Features Explained

### Responsive Design
- **Desktop**: Full layout with sidebar navigation and detailed views
- **Tablet**: Optimized spacing and button sizes
- **Mobile**: Compact design with collapsible elements and touch-friendly interface

### Search Functionality
- Real-time search across contact names, emails, and phone numbers
- Debounced input for optimal performance
- Clear visual feedback for search results

### Authentication Flow
- JWT tokens stored in localStorage
- Automatic token validation and refresh
- Protected routes redirect to login when unauthenticated
- Context-based user state management

### Modern UI Elements
- Glassmorphism design with backdrop blur effects
- Smooth animations and transitions
- Consistent color scheme and typography
- Interactive hover states and micro-animations


## 🔒 Security Features

- Password hashing with bcrypt
- JWT token-based authentication
- CORS configuration for secure cross-origin requests
- Input validation and sanitization
- Protected API routes with middleware
- Environment variable usage for sensitive data

## 🛡️ Error Handling

- Global error handler middleware
- Try-catch blocks for async operations
- User-friendly error messages
- Toast notifications for user feedback
- Loading states for better UX

## 📱 Mobile Optimization

- Touch-friendly interface design
- Responsive grid layouts
- Optimized button sizes for mobile
- Collapsible navigation elements
- Fast loading and smooth scrolling

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


Made with ❤️ by Aaron Kurian Abraham