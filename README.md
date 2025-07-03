# Fullstack Image Generator

A full-stack MERN (MongoDB, Express.js, React, Node.js) application that generates AI-powered images using the ClipDrop API.

## Features

- 🎨 AI-powered image generation
- 🔐 User authentication with JWT
- 💳 Credit-based system for image generation
- 📱 Responsive design with modern UI
- 🚀 Fast image processing
- 💾 Image download functionality

## Tech Stack

### Frontend
- **React** - UI framework
- **Vite** - Build tool
- **Tailwind CSS** - Styling
- **React Router** - Client-side routing
- **Axios** - API calls
- **React Toastify** - Notifications

### Backend
- **Node.js** - Runtime environment
- **Express.js** - Web framework
- **MongoDB** - Database
- **Mongoose** - ODM
- **JWT** - Authentication
- **Bcrypt** - Password hashing
- **ClipDrop API** - Image generation

## Prerequisites

Before running this application, make sure you have the following installed:
- Node.js (v14 or higher)
- MongoDB (local or cloud instance)
- ClipDrop API key

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Fullstack-image-generator.git
   cd Fullstack-image-generator
   ```

2. Install dependencies for both client and server:
   ```bash
   # Install server dependencies
   cd server
   npm install

   # Install client dependencies
   cd ../client
   npm install
   ```

3. Set up environment variables:

   Create a `.env` file in the server directory:
   ```env
   MONGODB_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret_key
   CLIPDROP_API=your_clipdrop_api_key
   ```

   Create a `.env` file in the client directory:
   ```env
   VITE_BACKEND_URL=http://localhost:4000
   ```

## Running the Application

1. Start the server:
   ```bash
   cd server
   npm start
   ```

2. Start the client (in a new terminal):
   ```bash
   cd client
   npm run dev
   ```

3. Open your browser and navigate to `http://localhost:5173`

## Project Structure

```
├── client/                 # React frontend
│   ├── src/
│   │   ├── components/     # Reusable components
│   │   ├── pages/          # Page components
│   │   ├── context/        # React context
│   │   └── assets/         # Static assets
│   └── public/             # Public assets
├── server/                 # Node.js backend
│   ├── controllers/        # Request handlers
│   ├── models/             # Database models
│   ├── routes/             # API routes
│   ├── middlewares/        # Custom middlewares
│   └── config/             # Configuration files
└── .gitignore              # Git ignore file
```

## API Endpoints

### Authentication
- `POST /api/user/register` - Register a new user
- `POST /api/user/login` - Login user
- `GET /api/user/profile` - Get user profile

### Image Generation
- `POST /api/image/generate` - Generate image from text
- `GET /api/image/history` - Get user's image history

## Features in Detail

### User Authentication
- Secure user registration and login
- JWT-based authentication
- Password hashing with bcrypt

### Image Generation
- Text-to-image generation using ClipDrop API
- Credit-based system
- Image history tracking

### Payment Integration
- Razorpay integration for credit purchases
- Secure payment processing

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- ClipDrop API for image generation
- React and Node.js communities
- MongoDB for database solutions

## Contact

For any questions or suggestions, please open an issue or contact the maintainers.
