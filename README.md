🚀 Real-Time Full-Stack Chat Application

MERN Stack | WebSockets (Socket.io) | Custom UI/UX

🌟 Project Overview

This repository hosts a robust, full-stack real-time chat application built on the MERN (MongoDB, Express, React, Node.js) stack. The goal of this project was to implement persistent, scalable messaging and explore modern client-side performance using Vite and a component-based architecture.

The application allows authenticated users to engage in instant one-on-one conversations, manage their profile, and see online user statuses in real-time.

✨ Core Features

Real-Time Messaging: Implemented using Socket.io for low-latency, bidirectional communication, ensuring messages and status updates are instant.

Full Authentication & Authorization: Secure user sign-up and log-in handled using JWT (JSON Web Tokens) and HTTP-only cookies.

NoSQL Data Persistence: MongoDB is used to store user profiles, encrypted passwords, and conversation history.

Image Uploads: Users can send images directly through the chat, which are handled and hosted using Cloudinary.

Customization: Includes a theme manager built with Zustand and Daisy UI to allow users to personalize their UI color scheme.

Modern Frontend: Built with React and bundled using Vite for optimized development and production speed.

🛠️ Tech Stack

Frontend (Client)

Framework: React.js

Styling: Tailwind CSS + Daisy UI (Component Library)

Build Tool: Vite

State Management: Zustand (Custom Hooks)

Networking: Axios

Backend (Server)

Runtime: Node.js

Framework: Express.js

Database: MongoDB (via Mongoose ODM)

Real-Time: Socket.io

Authentication: JWT, bcryptjs (Password Hashing)

File Hosting: Cloudinary

⚙️ Local Setup Instructions

Follow these steps to get the project running on your local machine.

Prerequisites

You must have Node.js (v18+) and npm installed.

Clone the Repository:

git clone [YOUR REPOSITORY URL]
cd [YOUR REPOSITORY NAME]


Install Dependencies:

cd backend
npm install
cd ../frontend
npm install


Environment Configuration

Create a file named .env inside the backend folder.

Populate it with the necessary keys (use the example file for structure):

# Content of backend/.env

# Database Connection
MONGO_URI=mongodb+srv://<USERNAME>:<PASSWORD>@<CLUSTER_URL>/<DB_NAME>?retryWrites=true&w=majority

# Security Keys
PORT=5001
JWT_SECRET=YOUR_SUPER_SECRET_KEY_HERE

# Image Uploads (REQUIRED for image sending feature)
CLOUDINARY_CLOUD_NAME=YOUR_CLOUD_NAME
CLOUDINARY_API_KEY=YOUR_API_KEY
CLOUDINARY_API_SECRET=YOUR_API_SECRET


Run the Application

You need two separate terminal windows for the frontend and backend.

Start the Backend Server (Terminal 1):

cd backend
npm run dev
# Wait for: "MongoDB connected"


Start the Frontend App (Terminal 2):

cd frontend
npm run dev
# App runs at: http://localhost:5173/


Open your browser, sign up for a new account, and open the app in a second tab (or incognito window) to test the real-time messaging!
