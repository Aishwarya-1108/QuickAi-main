# QuickAI

QuickAI is a full-stack AI-powered utility platform that provides users with a collection of intelligent tools for content generation, image processing, and resume analysis. Built with React, Node.js, Express.js, and PostgreSQL, the platform supports secure authentication, cloud media storage, and subscription-based access to premium features.

## Features

### Free Tools

* **Dashboard** – Centralized access to all AI tools and user activities.
* **Write Article** – Generate detailed, AI-powered articles from user prompts.
* **Blog Title Generator** – Create SEO-friendly and engaging blog titles.
* **Community Feed** – Browse and interact with content shared by other users.

### Premium Tools *(Currently Available for Free)*

* **Generate Images** – Create AI-generated images from text prompts.
* **Remove Background** – Automatically remove image backgrounds.
* **Remove Objects** – Erase unwanted objects from images.
* **Resume Review** – Receive AI-powered resume analysis and improvement suggestions.

### Security & Access Control

* Secure user authentication using Clerk.
* Role-based access to premium features.
* Protected API routes and user-specific data management.

## Tech Stack

### Frontend

* React.js
* React Router DOM
* Tailwind CSS

### Backend

* Node.js
* Express.js

### Database

* PostgreSQL

### Authentication

* Clerk Authentication

### Media Storage

* Cloudinary

### AI & External APIs

* Google Gemini 2.0 Flash
* Clipdrop API

### Deployment

* Frontend: Vercel
* Backend: Vercel

## Live Demo

Frontend: https://quick-ai-frontend.vercel.app/

## APIs Used

### Google Gemini 2.0 Flash

Used for:

* Article generation
* Blog title generation
* Resume analysis
* General AI-powered text generation

### Clipdrop API

Used for:

* AI image generation
* Background removal
* Object removal

## Project Architecture

```text
QuickAI
│
├── client/                 # React Frontend
│   ├── src/
│   ├── components/
│   ├── pages/
│   └── assets/
│
├── server/                 # Node.js Backend
│   ├── controllers/
│   ├── routes/
│   ├── middleware/
│   ├── configs/
│   └── database/
│
└── PostgreSQL Database
```

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Jagg2611/QuickAI.git
cd QuickAI
```

### 2. Configure Environment Variables

#### Backend (server/.env)

```env
DATABASE_URL=postgresql://your-user:your-password@your-host/neondb?sslmode=require&channel_binding=require

CLERK_SECRET_KEY=your-clerk-secret-key

GEMINI_API_KEY=your-gemini-api-key

CLIPDROP_API_KEY=your-clipdrop-api-key

CLOUDINARY_CLOUD_NAME=your-cloud-name
CLOUDINARY_API_KEY=your-cloudinary-api-key
CLOUDINARY_API_SECRET=your-cloudinary-api-secret
```

#### Frontend (client/.env)

```env
VITE_BASE_URL=http://localhost:3000

VITE_CLERK_PUBLISHABLE_KEY=your-clerk-publishable-key
```

### 3. Install Dependencies

#### Backend

```bash
cd server
npm install
```

#### Frontend

```bash
cd client
npm install
```

### 4. Run the Application

#### Start Backend

```bash
npm run server
```

#### Start Frontend

```bash
npm run dev
```

### 5. Open in Browser

```text
Frontend: http://localhost:5173
Backend: http://localhost:3000
```

## Key Highlights

* Built a full-stack AI SaaS platform integrating multiple AI services.
* Implemented secure authentication and role-based access using Clerk.
* Integrated Gemini AI and Clipdrop APIs for text and image generation capabilities.
* Developed scalable REST APIs with Express.js and PostgreSQL.
* Leveraged Cloudinary for efficient media storage and management.
* Deployed frontend and backend applications on Vercel.

## Future Improvements

* Subscription payment integration (Stripe/Razorpay)
* User usage analytics dashboard
* AI chat assistant
* Team collaboration features
* AI content history and bookmarking

## Author

**Aishwarya Panuganti**

GitHub: https://github.com/yourusername

LinkedIn: https://linkedin.com/in/yourprofile

