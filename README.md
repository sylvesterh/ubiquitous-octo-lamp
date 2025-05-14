# Real-Time Chat Application

A full-stack real-time chat application demonstrating the power of WebSockets for instant messaging functionality.

## Project Overview

This project is designed as a learning tool to understand real-time communication using WebSockets, specifically with Socket.IO. The application consists of:

- **Backend**: Node.js server with Express and Socket.IO
- **Frontend**: React application using modern libraries

## Technology Stack

### Backend
- **Node.js** with **Express** framework
- **Socket.IO** for real-time, bidirectional communication
- **MongoDB** with Mongoose for database operations
- **JWT** and **bcryptjs** for authentication
- **Cloudinary** for media storage and handling

### Frontend
- **React 19** with hooks
- **Socket.IO Client** for WebSocket communication
- **Tailwind CSS** with DaisyUI for styling
- **Zustand** for state management
- **React Hot Toast** for notifications
- **Axios** for HTTP requests

## Features

- Real-time messaging with WebSockets
- User authentication and authorization
- User profiles with avatar support
- Message persistence with MongoDB
- Responsive design with Tailwind CSS

## Getting Started

### Prerequisites
- Node.js (LTS version recommended)
- MongoDB instance (local or Atlas)
- Cloudinary account for media storage

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/real-time-chat-app.git
cd real-time-chat-app
```

2. Install dependencies for both backend and frontend:
```bash
# Install root dependencies
npm install

# Install backend dependencies
cd backend
npm install

# Install frontend dependencies
cd ../frontend
npm install
```

3. Set up environment variables:
   
   Create a `.env` file in the backend directory with the following variables:
   ```
   PORT=8000
   MONGODB_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
   CLOUDINARY_API_KEY=your_cloudinary_api_key
   CLOUDINARY_API_SECRET=your_cloudinary_api_secret
   ```

### Running the Application

1. Start the backend server:
```bash
cd backend
npm run dev
```

2. Start the frontend development server:
```bash
cd frontend
npm run dev
```

3. Open your browser and navigate to `http://localhost:5173` (or the port shown in your terminal)

## Project Structure

```
.
├── backend/
│   ├── src/
│   │   ├── controllers/     # Request handlers
│   │   ├── models/          # Database models
│   │   ├── routes/          # API routes
│   │   ├── middlewares/     # Custom middlewares
│   │   ├── socket/          # Socket.IO setup and event handlers
│   │   └── index.js         # Entry point
│   └── package.json
└── frontend/
    ├── src/
    │   ├── components/      # React components
    │   ├── pages/           # Page components
    │   ├── store/           # Zustand state management
    │   ├── hooks/           # Custom hooks
    │   ├── utils/           # Utility functions
    │   ├── socket/          # Socket.IO client setup
    │   └── App.jsx          # Main application component
    └── package.json
```

## Understanding WebSockets

This project demonstrates several key WebSocket concepts:

- **Real-time Communication**: Messages are delivered instantly without polling
- **Bidirectional Communication**: Both server and client can initiate communication
- **Event-Based Architecture**: The application uses events to handle different types of messages
- **Room-Based Messaging**: Users can join different chat rooms or conversations
- **Presence Awareness**: Users can see who is online/offline

## Learning Resources

To better understand WebSockets and the technologies used:

- [Socket.IO Documentation](https://socket.io/docs/v4/)
- [React Documentation](https://react.dev/)
- [MongoDB Documentation](https://docs.mongodb.com/)
- [Express Documentation](https://expressjs.com/)

## Acknowledgments

- Socket.IO team for their excellent real-time engine
- React team for their powerful frontend library