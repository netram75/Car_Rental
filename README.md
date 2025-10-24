# Car Rental System - Full Stack Application

A modern full-stack car rental application built with MERN stack (MongoDB, Express.js, React.js, Node.js) that allows users to rent cars and owners to manage their car fleet.

## Features

### User Features
- User authentication and authorization
- Browse available cars with detailed information
- Filter and search functionality
- Book cars for specific dates
- View booking history
- Responsive design for all devices

### Owner Dashboard
- Secure owner portal
- Add and manage cars in the fleet
- View and manage bookings
- Track car availability
- Real-time updates on bookings

## Tech Stack

### Frontend
- React.js
- Vite
- Context API for state management
- Modern UI components
- Responsive design

### Backend
- Node.js
- Express.js
- MongoDB (with Mongoose)
- JWT Authentication
- ImageKit for image management

## Project Structure

```
├── client/                 # Frontend React application
│   ├── src/
│   │   ├── components/    # Reusable UI components
│   │   ├── context/      # Application state management
│   │   ├── pages/        # Application pages
│   │   └── assets/       # Static assets
│   └── public/           # Public assets
│
├── server/                # Backend Node.js application
│   ├── configs/          # Configuration files
│   ├── controllers/      # Request handlers
│   ├── middleware/       # Custom middleware
│   ├── models/          # Database models
│   └── routes/          # API routes
```

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- MongoDB
- npm or yarn

### Installation

1. Clone the repository
```bash
git clone https://github.com/netram75/Car_Rental.git
cd Car_Rental
```

2. Install frontend dependencies
```bash
cd client
npm install
```

3. Install backend dependencies
```bash
cd ../server
npm install
```

4. Set up environment variables
- Create `.env` file in the server directory
- Add necessary environment variables:
  ```
  MONGODB_URI=your_mongodb_uri
  JWT_SECRET=your_jwt_secret
  IMAGEKIT_PUBLIC_KEY=your_imagekit_public_key
  IMAGEKIT_PRIVATE_KEY=your_imagekit_private_key
  IMAGEKIT_URL_ENDPOINT=your_imagekit_url_endpoint
  ```

5. Start the development servers

Backend:
```bash
cd server
npm start
```

Frontend:
```bash
cd client
npm run dev
```

## API Endpoints

### User Routes
- POST /api/users/register - Register new user
- POST /api/users/login - User login
- GET /api/users/profile - Get user profile

### Car Routes
- GET /api/cars - Get all cars
- GET /api/cars/:id - Get car details
- POST /api/owner/cars - Add new car (owner only)
- PUT /api/owner/cars/:id - Update car (owner only)
- DELETE /api/owner/cars/:id - Delete car (owner only)

### Booking Routes
- POST /api/bookings - Create new booking
- GET /api/bookings/user - Get user bookings
- GET /api/owner/bookings - Get all bookings (owner only)

## Deployment

The application is configured for deployment:
- Frontend is configured for Vercel deployment
- Backend includes vercel.json for serverless deployment

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request



## Note
- Don't commit node_modules directory
- Ensure all sensitive information is stored in environment variables
- Follow the coding standards and guidelines
