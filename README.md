# 🎥 ChatBridge - Video Calling & Chat Application

🌐 **Live Demo**: [https://chatbridge-language-exchange-platform.onrender.com](https://chatbridge-language-exchange-platform.onrender.com)



A modern, full-stack video calling and chat application built with React and Node.js. ChatBridge provides seamless real-time communication with video calls, messaging, and friend management features.

## ✨ Key Features

- 📹 **High-quality video calls** with screen sharing capabilities
- 💬 **Real-time messaging** with instant notifications
- 👥 **Friend management system** with friend requests
- 🔐 **Secure authentication** with JWT tokens
- 🎨 **Modern UI** with responsive design and dark/light themes
- ⚡ **Real-time updates** using Socket.io and Stream Chat
- 🚀 **Scalable architecture** with MongoDB and Express.js

## 🛠️ Tech Stack

### Frontend

- **React 19** with Vite
- **TailwindCSS** for styling
- **Zustand** for state management
- **React Router** for navigation
- **Stream Chat SDK** for real-time messaging
- **Stream Video SDK** for video calling

### Backend

- **Node.js** with Express
- **MongoDB** with Mongoose
- **JWT** for authentication
- **bcryptjs** for password hashing
- **Socket.io** for real-time features

## 🚀 Quick Start

### Prerequisites

- Node.js (v16 or higher)
- MongoDB
- Stream Chat & Video API keys

### Installation

1. **Clone the repository**

```bash
git clone <repository-url>
cd streamify-video-calls-master
```

2. **Install dependencies**

```bash
# Install root dependencies
npm install

# Install backend dependencies
cd backend && npm install

# Install frontend dependencies
cd ../frontend && npm install
```

3. **Environment Setup**

Create `.env` files in both backend and frontend directories:

**Backend `.env` (in `/backend`)**

```env
PORT=5001
MONGO_URI=mongodb://localhost:27017/streamify
JWT_SECRET_KEY=your-secret-key-here
NODE_ENV=development
```

**Frontend `.env` (in `/frontend`)**

```env
VITE_STREAM_API_KEY=your-stream-api-key
```

4. **Start the development servers**

**Backend**

```bash
cd backend
npm run dev
```

**Frontend**

```bash
cd frontend
npm run dev
```

The application will be available at:

- Frontend: http://localhost:5173
- Backend: http://localhost:5001

## 📁 Project Structure

```
streamify-video-calls-master/
├── backend/
│   ├── src/
│   │   ├── controllers/     # API controllers
│   │   ├── middleware/      # Authentication & validation
│   │   ├── models/          # MongoDB schemas
│   │   ├── routes/          # API routes
│   │   └── server.js        # Express server
├── frontend/
│   ├── src/
│   │   ├── components/      # Reusable components
│   │   ├── pages/          # Page components
│   │   ├── hooks/          # Custom React hooks
│   │   ├── store/          # Zustand stores
│   │   └── lib/            # Utilities & API client
├── README.md
└── package.json
```

## 🔧 Available Scripts

### Root directory

- `npm run build` - Build both frontend and backend
- `npm start` - Start production server

### Backend

- `npm run dev` - Start development server with nodemon
- `npm start` - Start production server

### Frontend

- `npm run dev` - Start Vite development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build

## 🎯 Features Overview

### Authentication

- User registration and login
- JWT-based authentication
- Protected routes

### Video Calling

- 1-on-1 video calls
- Screen sharing
- High-quality video streaming

### Messaging

- Real-time chat
- Message notifications
- Chat history

### Friend System

- Send/accept friend requests
- Friend list management
- Online status indicators

## 🌐 API Endpoints

### Authentication

- `POST /api/auth/signup` - User registration
- `POST /api/auth/login` - User login
- `POST /api/auth/logout` - User logout

### Users

- `GET /api/users` - Get all users
- `GET /api/users/:id` - Get user by ID
- `PUT /api/users/:id` - Update user

### Friends

- `POST /api/friends/request` - Send friend request
- `PUT /api/friends/accept` - Accept friend request
- `GET /api/friends/list` - Get friend list

### Chat

- `GET /api/chat/conversations` - Get user conversations
- `POST /api/chat/message` - Send message
- `GET /api/chat/messages/:conversationId` - Get messages

## 📝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the ISC License.

## 👥 Support

For support, please open an issue in the GitHub repository.
