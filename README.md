# NEXUS

NEXUS is a lightweight real-time chat application (frontend + backend) built with React, Vite, Express, Socket.IO, and MongoDB. It provides user authentication, messaging, and media sharing with a modern, responsive UI.

## Tech stack
- Frontend: React, Vite, Tailwind CSS, DaisyUI, Zustand
- Backend: Node.js, Express, Mongoose, Socket.IO
- Database: MongoDB (self-hosted or Atlas)

## Features
- User sign up / sign in (JWT)
- Real-time messaging with Socket.IO
- File/image sharing support
- Responsive UI with animated components

## Repo layout
```
backend/        # Express API, socket server, env and DB config
frontend/       # React + Vite app
package.json    # root metadata (optional)
README.MD       # this file
```

## Prerequisites
- Node.js (>= 18 recommended)
- npm or yarn
- MongoDB: either local MongoDB server or a MongoDB Atlas cluster

## Environment variables
The backend loads environment variables from `backend/.env`. Create that file (or set env vars) with the following keys:

```
PORT=3000
MONGO_URI=your_mongo_uri_here         
NODE_ENV=development
JWT_SECRET=your_jwt_secret
RESEND_API_KEY=your_resend_api_key
EMAIL_FROM=your_email_from_address
EMAIL_FROM_NAME=your_email_from_name
CLIENT_URL=http://localhost:5173
CLOUDINARY_CLOUD_NAME=...
CLOUDINARY_API_KEY=...
CLOUDINARY_API_SECRET=...
ARCJET_KEY=...
ARCJET_ENV=development
```

