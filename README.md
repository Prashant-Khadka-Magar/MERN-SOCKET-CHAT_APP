# MERN Socket Chat App

A real-time chat application built with the MERN stack and Socket.io, featuring instant messaging, user authentication, and modern UI design.

## 🚀 Features

- **Real-Time Messaging**
  - Instant message delivery with Socket.io
  - Live typing indicators
  - Online/offline user status
  - Message timestamps

- **User Authentication & Authorization**
  - Secure user registration and login
  - JWT-based authentication
  - Protected routes and sessions
  - Password encryption with bcrypt

- **Modern Chat Interface**
  - Clean and intuitive design with DaisyUI
  - Responsive layout for all devices
  - Dark/light theme support
  - Emoji and rich text support

- **User Management**
  - User profiles with avatars
  - Online user list
  - User search functionality
  - Profile image uploads with Cloudinary

- **Real-Time Features**
  - Instant message notifications
  - Live user presence indicators
  - Real-time chat updates
  - Message delivery confirmation

## 🛠️ Tech Stack

### Frontend
- **React 18** - Modern UI library with hooks
- **Vite** - Fast build tool and development server
- **Socket.io Client** - Real-time bidirectional communication
- **Zustand** - Lightweight state management
- **React Router DOM** - Client-side routing
- **Axios** - HTTP client for API requests
- **Tailwind CSS** - Utility-first CSS framework
- **DaisyUI** - Tailwind CSS component library
- **Lucide React** - Beautiful icon library
- **React Hot Toast** - Toast notifications

### Backend
- **Node.js** - JavaScript runtime environment
- **Express.js** - Web application framework
- **Socket.io** - Real-time WebSocket communication
- **MongoDB** - NoSQL database with Mongoose ODM
- **JWT** - JSON Web Tokens for authentication
- **bcryptjs** - Password hashing and encryption
- **Cloudinary** - Cloud-based image storage
- **CORS** - Cross-origin resource sharing

## 📦 Installation

### Prerequisites
- Node.js (v16 or higher)
- MongoDB (local or MongoDB Atlas)
- npm or yarn
- Cloudinary account (for image uploads)

### Clone the repository
```bash
git clone https://github.com/Prashant-Khadka-Magar/MERN-SOCKET-CHAT_APP.git
cd MERN-SOCKET-CHAT_APP
```

### Backend Setup
```bash
# Navigate to backend directory
cd backend

# Install dependencies
npm install

# Create .env file with required variables
touch .env
```

### Frontend Setup
```bash
# Navigate to frontend directory
cd frontend

# Install dependencies
npm install
```

### Environment Variables
Create a `.env` file in the backend directory:
```env
NODE_ENV=development
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
```

## 🚀 Usage

### Development Mode

**Start Backend Server:**
```bash
cd backend
npm run dev
```

**Start Frontend Development Server:**
```bash
cd frontend
npm run dev
```

The application will be available at:
- Frontend: `http://localhost:5173`
- Backend: `http://localhost:5000`

### Production Mode

**Build Frontend:**
```bash
cd frontend
npm run build
```

**Start Production Server:**
```bash
cd backend
npm start
```

## 📁 Project Structure

```
├── backend/
│   ├── src/
│   │   ├── controllers/    # Route controllers
│   │   ├── middleware/     # Custom middleware
│   │   ├── models/         # Database models
│   │   ├── routes/         # API routes
│   │   ├── socket/         # Socket.io handlers
│   │   └── index.js        # Server entry point
│   └── package.json
├── frontend/
│   ├── src/
│   │   ├── components/     # React components
│   │   ├── pages/          # Page components
│   │   ├── store/          # Zustand store
│   │   ├── hooks/          # Custom hooks
│   │   ├── utils/          # Utility functions
│   │   └── App.jsx         # Main App component
│   ├── public/             # Static assets
│   └── package.json
└── README.md
```

## 🔧 API Endpoints

### Authentication
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - Login user
- `POST /api/auth/logout` - Logout user
- `GET /api/auth/check` - Check authentication status

### Messages
- `GET /api/messages/:conversationId` - Get conversation messages
- `POST /api/messages/send` - Send new message
- `GET /api/messages/conversations` - Get user conversations

### Users
- `GET /api/users` - Get all users
- `GET /api/users/profile` - Get user profile
- `PUT /api/users/profile` - Update user profile

## 🌐 Socket Events

### Client to Server
- `join_room` - Join chat room
- `send_message` - Send message
- `typing` - Typing indicator
- `stop_typing` - Stop typing

### Server to Client
- `receive_message` - Receive new message
- `user_online` - User came online
- `user_offline` - User went offline
- `typing_indicator` - Show typing indicator

## 🎨 UI Components

- **Chat Interface** - Main chat window with message history
- **User List** - Online users sidebar
- **Message Input** - Rich text message composer
- **Profile Modal** - User profile management
- **Authentication Forms** - Login and registration
- **Toast Notifications** - Real-time feedback

## 🔐 Security Features

- JWT token-based authentication
- Password hashing with bcrypt
- CORS protection
- Input validation and sanitization
- Protected API routes
- Secure file uploads

## 🤝 Contributing

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the ISC License.

## 👨‍💻 Author

**Prashant Magar**
- GitHub: [@Prashant-Khadka-Magar](https://github.com/Prashant-Khadka-Magar)

## 🙏 Acknowledgments

- Socket.io for real-time communication
- Cloudinary for image management
- DaisyUI for beautiful UI components
- MongoDB for database services
- All the amazing open-source libraries that made this project possible


## 🚀 Deployment

This application can be deployed on platforms like:
- **Heroku** - For the backend
- **Vercel/Netlify** - For the frontend
- **MongoDB Atlas** - For the database
- **Cloudinary** - For image storage

## 🔮 Future Enhancements

- [ ] Group chat functionality
- [ ] File sharing capabilities
- [ ] Voice messages
- [ ] Video calling integration
- [ ] Message encryption
- [ ] Push notifications
- [ ] Message search functionality
