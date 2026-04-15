# Mocksy Frontend

This directory contains the React frontend for the Mocksy Mock Interview Platform. It is built with React and Vite, featuring a responsive, dark-mode design with real-time websocket connections to the backend.

## Prerequisites

Make sure you have [Node.js](https://nodejs.org/) installed on your machine.

## How to Run the Frontend

1. **Navigate to the frontend directory**
   If you aren't already here, change to the `frontend` directory:
   ```bash
   cd frontend
   ```

2. **Install dependencies**
   Run the following command to install all the required node modules:
   ```bash
   npm install
   ```

3. **Start the development server**
   You can start the frontend development server using:
   ```bash
   npm run dev
   ```
   Or if you want it to be accessible on your local network (so you can test it on your phone or other devices):
   ```bash
   npm run dev -- --host 0.0.0.0
   ```

4. **Access the application**
   Once the server starts, open your browser and navigate to:
   [http://localhost:5173/](http://localhost:5173/) or the port specified in your terminal output (e.g., `5174`).

> **Note**: For the application to function correctly (user registration, login, file uploads, and initiating mock interviews), make sure the Mocksy backend is also running concurrently on port `8000`.

## Architecture Details
- **Routing**: `react-router-dom`
- **Design System**: Vanilla CSS with glassmorphism styles (`src/index.css`)
- **Authentication**: JWT tokens stored in `localStorage` managed via `AuthContext.jsx`
- **Real-Time Features**: WebSockets to connect directly to the FastAPI server for the live interview loop.


## Backend REPO Link: https://github.com/itxmuhammadwaqarali/Mocksy