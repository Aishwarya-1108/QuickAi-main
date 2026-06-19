QuickAI
QuickAI is a full-stack AI utility platform built with a React frontend (Vite) and a Node.js + Express backend, using PostgreSQL as the primary database.

It provides users with access to AI powered tools such as content generation, image processing, and resume analysis etc. with support for both free and premium subscriptions.

Features
Free Tools
Dashboard: Centralized navigation and access to all tools

Write Article: Generate detailed AI-based articles from prompts

Blog Titles: Generate optimized titles for blog posts

Community: View and engage with other users’ content

Premium Tools (Enabled free as of now)
Generate Images: AI-based image generation from textual prompts

Remove Background: Automatically removes background from uploaded images

Remove Object: Erase selected objects from images

Review Resume: Get AI-powered resume feedback

User access is determined by subscription level and enforced via role-based authentication.

Tech Stack
Frontend: React, React Router, Tailwind CSS
Backend: Node.js, Express.js
Database: Postgres SQL
Authentication: Clerk Auth
Media Storage: Cloudinary
Deployment: Vercel (Frontend), and Vercel (backend) deployment.
Live Site
Deployed at: https://quick-ai-frontend.vercel.app/

API's Used
Google gemini-2.0-flash - Text generation related Queries
Clipdrop API - Image related Queries
Getting Started (Local Setup)
1. Clone the repository
git clone https://github.com/Jagg2611/QuickAI.gi
cd QuickAI
2. Environment Variables
Create a .env file in both frontend/ and backend/ folders.

for backend/server add the following keys

DATABASE_URL=postgresql://your-user:your-password@your-host/neondb?sslmode=require&channel_binding=require

CLERK_SECRET_KEY=your-clerk-secret-key
GEMINI_API_KEY=your-gemini-api-key
CLICKDROP_API_KEY=your-clickdrop-api-key

CLOUDINARY_CLOUD_NAME=your-cloud-name
CLOUDINARY_API_KEY=your-cloudinary-api-key
CLOUDINARY_API_SECRET=your-cloudinary-api-secret
for frontend/client add the following keys

VITE_BASE_URL=http://localhost:3000
VITE_CLERK_PUBLISHABLE_KEY=your-publishable-key
3. Install the required dependencies
#Backend

cd server
npm install
#Frontend
cd client 
npm install
4. Run the app locally
Backend/server
npm run server
Frontend/client
npm run dev
