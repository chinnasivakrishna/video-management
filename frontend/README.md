

# Video Management Application

A full-stack video management application that allows users to upload, manage, and stream videos with Google Drive integration.

## Live Demo
- Frontend: [https://video-management-app-front-end.vercel.app/](https://video-management-app-front-end.vercel.app/)
- Backend: [https://video-management-app.onrender.com](https://video-management-app.onrender.com)

Demo Credentials:
- Email: admin@gmail.com
- Password: sivakrishna
- (Or create your own account through registration)

## Features

- User authentication (JWT)
- Video upload (local & Google Drive)
- Video streaming with custom controls
- Search and filter functionality
- Tag-based organization
- Responsive design
- Secure file handling

## Tech Stack

### Frontend
- React.js
- Material-UI (MUI)
- React Router
- Axios
- Google Drive API
- JWT Authentication

### Backend
- Node.js
- Express.js
- MongoDB
- JWT
- Multer (file handling)
- Cookie-parser

## Setup Instructions

### Backend Setup

1. Clone the repository
```bash
git clone <repository-url>
cd video-manager
```

2. Install dependencies
```bash
cd backend
npm install
```

3. Create `.env` file
```env
MONGODB_URI=your_mongodb_uri
JWT_SECRET=your_jwt_secret
PORT=5000
```

4. Start the server
```bash
npm start
```

### Frontend Setup

1. Navigate to frontend directory
```bash
cd frontend
npm install
```

2. Create `.env` file
```env
REACT_APP_GOOGLE_API_KEY=your_google_api_key
REACT_APP_GOOGLE_CLIENT_ID=your_google_client_id
REACT_APP_API_URL=http://localhost:5000
```

3. Start the application
```bash
npm start
```

## Project Structure

### Backend
```
backend/
├── models/
│   ├── User.js
│   └── Video.js
├── routes/
│   ├── authRoutes.js
│   └── videoRoutes.js
├── middleware/
│   └── auth.js
└── server.js
```

### Frontend
```
frontend/
├── src/
│   ├── components/
│   │   ├── auth/
│   │   └── videos/
│   ├── hooks/
│   ├── utils/
│   └── App.js
└── public/
```

## API Endpoints

### Authentication
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - User login
- `POST /api/auth/logout` - User logout

### Videos
- `POST /api/videos/upload` - Upload video
- `GET /api/videos` - Get all videos
- `GET /api/videos/:id` - Get single video
- `DELETE /api/videos/:id` - Delete video

## Security Features

- JWT Authentication
- HTTP-Only Cookies
- Protected Routes
- Input Validation
- File Type Validation
- Secure Password Hashing

## Deployment

The application is deployed using:
- Frontend: Vercel
- Backend: Render
- Database: MongoDB Atlas

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request

## License

This project is licensed under the MIT License.
```

This README provides:
1. Clear project overview
2. Setup instructions
3. Project structure
4. API documentation
5. Security features
6. Deployment information
7. Live demo links and credentials
8. Contributing guidelines

