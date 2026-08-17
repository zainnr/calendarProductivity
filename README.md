# Weekly - Calendar App

A full-stack weekly calendar application with task and meeting management.

## Features

- 🔐 JWT-based authentication
- 📅 Weekly calendar view (Monday - Sunday)
- ✅ Task management with completion tracking
- 📞 Meeting management with completion tracking
- 🎨 Clean, modern UI inspired by Google Calendar

## Tech Stack

- **Frontend**: Vite + React
- **Backend**: Node.js + Express
- **Authentication**: JWT (JSON Web Tokens)
- **Storage**: In-memory (no database required)

## Quick Start

### Backend Setup

```bash
cd backend
npm install
npm start
```

The backend server will run on `http://localhost:3000`

### Frontend Setup

In a new terminal:

```bash
cd frontend
npm install
npm run dev
```

The frontend will run on `http://localhost:5173`

Open your browser and navigate to `http://localhost:5173`

## Demo Credentials

- **Username**: `demo`
- **Password**: `demo123`

## API Endpoints

### Authentication
- `POST /auth/login` - Login and get JWT token

### Tasks (Protected)
- `GET /api/tasks` - Get all tasks
- `POST /api/tasks/:id/toggle` - Toggle task completion status

### Meetings (Protected)
- `GET /api/meetings` - Get all meetings
- `POST /api/meetings/:id/toggle` - Toggle meeting completion status

All protected routes require a JWT token in the Authorization header:
```
Authorization: Bearer <token>
```

## Project Structure

```
Weekly/
├── backend/
│   ├── server.js          # Express server
│   ├── data.js            # In-memory data storage
│   ├── middleware/
│   │   └── auth.js        # JWT authentication middleware
│   └── routes/
│       ├── auth.js        # Authentication routes
│       ├── tasks.js       # Task routes
│       └── meetings.js    # Meeting routes
└── frontend/
    ├── src/
    │   ├── components/
    │   │   ├── Login.jsx
    │   │   ├── WeeklyCalendar.jsx
    │   │   └── DayCard.jsx
    │   ├── services/
    │   │   └── api.js     # API service
    │   ├── styles/
    │   │   └── App.css
    │   ├── App.jsx
    │   └── main.jsx
    └── vite.config.js
```

## Usage

1. Start the backend server
2. Start the frontend development server
3. Open `http://localhost:5173` in your browser
4. Login with demo credentials
5. View your weekly calendar with tasks and meetings
6. Click on any day to expand and see details
7. Toggle tasks and meetings to mark them as completed

Vaibhav V Marar
Zainab Riyaz
