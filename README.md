10gpa.in

A centralized platform for B.Tech CSAM & Cyber Security students to access syllabus, lab experiments, previous year papers, and video resources.
Built using Next.js (App Router) and MongoDB, with a clean UI and fast server-rendered pages.

Overview

10gpa.in consolidates academic resources into a single platform.
Each subject page includes:

Syllabus (unit-wise)

Lab experiments

Previous year question papers

Video lectures and reference material

Credits, codes, and branch/semester details

Everything is stored in MongoDB and served through Next.js API routes.

Features

Centralized academic resource hub

Dynamic subject pages (generated from database)

MongoDB-backed syllabus, labs, videos, and question bank

Next.js App Router with server components for fast load times

Fully responsive UI

Simple, scalable monolithic architecture

Bulk subject upload support (via POST request)

Tech Stack

Frontend:

Next.js (App Router)

React

Tailwind CSS

Backend:

Next.js API Routes

Node.js

Mongoose (ODM)

Database:

MongoDB Atlas

Deployment:

Vercel

Project Structure
10gpa/
│── app/
│   ├── subjects/          # Dynamic subject routes
│   ├── api/subjects/      # CRUD API
│   ├── components/        # Reusable UI
│   └── layout.tsx
│
│── lib/
│   └── dbConnect.ts       # MongoDB connection logic
│
│── models/
│   └── Subject.ts         # Mongoose Schema
│
└── public/

Running Locally

Clone the repo:

git clone <repo-url>
cd 10gpa


Install dependencies:

npm install


Create .env.local:

MONGODB_URI=your_mongodb_connection_string
NEXT_PUBLIC_SITE_URL=http://localhost:3000


Start development server:

npm run dev

API Routes
GET /api/subjects

Fetch all subjects.

POST /api/subjects

Add a single subject or an array of subjects (bulk insert supported).

Example bulk insert:

[
  { "name": "Subject 1", "code": "...", ... },
  { "name": "Subject 2", "code": "...", ... }
]

Deployment

This project is optimized for Vercel.
Deploy by connecting your GitHub repo to Vercel.
Environment variables must be configured in Vercel dashboard.

Future Improvements

Admin panel for adding subjects

Search and filtering

Bookmarking features

User dashboard

Notes upload system

PDF viewer integration

Contributing

Issues, suggestions, and pull requests are welcome.
