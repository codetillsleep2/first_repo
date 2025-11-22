## 🚀 10gpa.in — CSAM & CYBER Study Hub

A centralized platform for B.Tech CSAM & Cyber Security students to access syllabus, lab manuals, previous year questions, video resources, and consolidated study material — all in one place.

Built with Next.js App Router + MongoDB, it delivers instant loading, server-rendered pages, and a clean structured UI optimized for academic needs.

##📸 Preview
<img width="1919" height="864" alt="image" src="https://github.com/user-attachments/assets/6814d65f-3c89-4117-94da-86ceb0a02bf0" />
##✨ Features
🎯 Academic Resources

Full syllabus breakdown for each subject

Lab experiments with step-by-step explanations

Previous year papers (PDF access)

Video resources for quick revision

End-to-end subject pages with theory + lab + external resources

##⚙️ Backend Functionality

Fully integrated MongoDB database for storing syllabus, questions, videos, and lab content

Optimized API routes using Next.js server functions

Flexible schema design supporting:

Multiple branches

Multiple semesters

Dynamic syllabus formats

Expandable content sections (videos, notes, PYQs)

##⚡ Performance & UX

Next.js server components for fast page loads

Built-in caching & data fetching

Clean responsive UI for mobile and desktop

Centralized architecture (no separate backend repo needed)

## 🛠️ Tech Stack
# Layer	Technologies
-Frontend	Next.js (App Router), React, Tailwind CSS
-Backend	Next.js Server Actions & API Routes
-Database	MongoDB Atlas (Mongoose ODM)
-Deployment	Vercel
-Auth / Security	Environment-secured API keys, server-side rendering
## 📂 Project Architecture
10gpa/
│── app/
│   ├── subjects/         # Dynamic subject pages
│   ├── api/              # Server-side API routes
│   ├── components/       # Reusable UI components
│   └── layout.tsx
│
│── lib/
│   └── dbConnect.ts      # MongoDB connection handler
│
│── models/
│   └── Subject.ts        # Mongoose schema
│
└── public/

## ▶️ Running Locally
1. Clone the repository
git clone <repo-url>
cd 10gpa

2. Install dependencies
npm install

3. Set environment variables

Create a .env.local file:

MONGODB_URI=your_mongodb_connection_string
NEXT_PUBLIC_SITE_URL=http://localhost:3000

4. Start local dev server
npm run dev

## 🧪 API Routes Overview
GET /api/subjects

Returns all subjects from MongoDB.

POST /api/subjects

Adds a single or multiple subjects (bulk upload supported).

Dynamic Route: /subjects/[code]

Auto-renders subject pages based on URL.

##📌 Roadmap

Add user login & bookmarks

Add student dashboard

Add search / filtering

Admin panel for adding subjects easily

Semester-wise module progress tracker

##🤝 Contributions

Pull requests, issues, and suggestions are welcome!

⭐ Support

If you find this useful, consider giving the repo a star ⭐ — it motivates further development!
