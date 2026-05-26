# OctoFit Tracker

A modern multi-tier application for tracking fitness activities and octopi encounters.

## Project Structure

```
octofit-tracker/
├── frontend/          # React 19 + Vite application
│   ├── src/
│   ├── package.json
│   └── vite.config.js
├── backend/           # Express + TypeScript backend
│   ├── src/
│   ├── package.json
│   └── tsconfig.json
└── .gitignore
```

## Tech Stack

### Frontend
- **React**: 19.2.6
- **Vite**: 8.0.14
- **Port**: 5173

### Backend
- **Express**: 4.22.2
- **TypeScript**: 5.9.3
- **Mongoose**: 8.24.0
- **Port**: 8000

### Database
- **MongoDB**: 27017

## Installation

### Frontend Setup
```bash
cd octofit-tracker/frontend
npm install
```

### Backend Setup
```bash
cd octofit-tracker/backend
npm install
```

## Running the Application

### Development Mode

**Frontend** (in `octofit-tracker/frontend`):
```bash
npm run dev
```
Runs on http://localhost:5173

**Backend** (in `octofit-tracker/backend`):
```bash
npm run dev
```
Runs on http://localhost:8000

### Production Mode

**Frontend Build**:
```bash
cd octofit-tracker/frontend
npm run build
```

**Backend Build & Start**:
```bash
cd octofit-tracker/backend
npm run build
npm start
```

## API Endpoints

- `GET /api/health` - Health check endpoint

## MongoDB Connection

The backend automatically connects to MongoDB at:
```
mongodb://localhost:27017/octofit-tracker
```

Ensure MongoDB is running on your system before starting the backend.

## Available Scripts

### Frontend
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm preview` - Preview production build

### Backend
- `npm run dev` - Start development server with auto-reload
- `npm run build` - Compile TypeScript to JavaScript
- `npm start` - Start production server
- `npm run lint` - Run ESLint

## Environment Variables

Create a `.env` file in the backend directory if needed:
```
MONGODB_URI=mongodb://localhost:27017/octofit-tracker
PORT=8000
```

## Notes

- The frontend uses Vite for fast development and optimized builds
- The backend uses Express with TypeScript for type safety
- Mongoose provides MongoDB object modeling
- Both applications run independently but communicate via REST APIs
