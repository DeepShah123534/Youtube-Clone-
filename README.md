📺 YouTube Clone – Full Stack (Cloud + Web)

A full-stack YouTube-like clone built in 4 parts:

Video Processing Service (Express + TypeScript + FFmpeg + Docker + Cloud Run)

Google Cloud Setup (Cloud Run, Pub/Sub, Cloud Storage)

Web App & Firebase (Next.js 13 + Firebase Auth + Firestore + Cloud Functions)

Upload & Watch Videos (Signed URLs, Firestore metadata, video listing & playback)



🚀 Features

🔄 Automated video processing pipeline (raw → 360p processed)

☁️ Google Cloud Run + Pub/Sub + Cloud Storage integration

🔑 Firebase Authentication (Google Sign-In)

🗄️ Firestore database for user & video metadata

🎥 Video uploads via signed URLs (secure direct upload to GCS)

📡 Event-driven video transcoding (ffmpeg, containerized)

🌐 Next.js 13 frontend with server & client components

▶️ Watch page with processed video playback

🐳 Dockerized deployment for both backend and frontend



🛠️ Tech Stack

Frontend: Next.js 13, React, Tailwind (optional styling), Firebase SDK

Backend: Express.js (TypeScript), ffmpeg (via fluent-ffmpeg)

Infrastructure: Google Cloud Run, Pub/Sub, Artifact Registry, Cloud Storage

Database & Auth: Firebase Auth, Firestore, Firebase Functions

Containerization: Docker (multi-stage builds)



🧪 Workflow

User logs in with Google

User uploads a video (directly to GCS via signed URL)

Raw bucket triggers Pub/Sub → Cloud Run processing service

Service downloads → ffmpeg → uploads processed video → marks Firestore metadata

Frontend feed fetches videos via callable function

User can watch processed video in /watch



🌐 Deployment

Backend & Frontend: Dockerized, deployed to Cloud Run

Storage: Cloud Storage (raw + processed)

Messaging: Pub/Sub event subscription

Auth & DB: Firebase Auth + Firestore
