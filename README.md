# StudyBuddy

<p align="center">
  <strong>A collaborative learning prototype built for Hack4Impact</strong><br />
  Study forums, accountability goals, peer discovery, profile gamification, and real-time collaboration experiments in one student-first interface.
</p>

<p align="center">
  <img alt="React" src="https://img.shields.io/badge/Frontend-React%2018-20232a?style=for-the-badge&logo=react" />
  <img alt="Express" src="https://img.shields.io/badge/Backend-Express-111111?style=for-the-badge&logo=express" />
  <img alt="Socket.IO" src="https://img.shields.io/badge/Realtime-Socket.IO-0b0b0b?style=for-the-badge&logo=socketdotio" />
  <img alt="MongoDB" src="https://img.shields.io/badge/Database-MongoDB-0f5d3f?style=for-the-badge&logo=mongodb" />
</p>

## Overview

StudyBuddy was built as part of **Hack4Impact**, organized by the **IEEE Computer Society VIT**, where the project won **Runner-Up**.

The idea behind the project is simple: studying gets easier when it becomes social, visible, and collaborative. Instead of learning in isolation, StudyBuddy brings together:

- subject-based discussion spaces
- study-goal and commitment tracking
- peer discovery and accountability
- profile-driven motivation through progress and badges
- real-time communication experiments for collaboration

This repository captures the hackathon prototype and the product direction behind it.

## What The Project Includes

### 1. Forum and buddy discovery
The landing experience introduces StudyBuddy as a collaborative learning platform and highlights top forums and top study buddies across subjects like DBMS, OS, VLSI, and InfoSec.

### 2. Study goal tracking
Users can browse active commitments, check progress percentages, and navigate to an add-goal flow for creating new study targets.

### 3. Social accountability feed
The social page surfaces other learners, their subjects, and countdown-style commitment windows to create a sense of momentum and public accountability.

### 4. Profile and gamification
The profile view showcases:

- commitments completed
- badges earned
- average response time
- a direct path into chat

### 5. Real-time collaboration experiments
The project also includes a backend and collaboration-oriented pieces for:

- Socket.IO-powered whiteboard synchronization
- real-time chat events
- a `react-chat-engine` based chat view

## Tech Stack

### Frontend

- React 18
- React Router
- Axios
- React Chat Engine
- CSS-based UI screens

### Backend

- Node.js
- Express
- Socket.IO
- MongoDB with Mongoose

## Project Structure

```text
study-buddy/
├── src/                 # React app and screens
├── public/              # Static assets used by the UI
├── backend/             # Express + Socket.IO backend scaffold
└── README.md
```

## Running Locally

### Prerequisites

- Node.js and npm

### Frontend

```bash
npm install
npm start
```

The React app runs on `http://localhost:3000`.

### Backend

```bash
cd backend
npm install
npm start
```

The backend starts on `http://localhost:3009` unless `PORT` is overridden.

### Optional environment variable

If you want to use the MongoDB connection scaffold in the backend, create a `.env` file inside `backend/` with:

```env
MONGODB_URI=your_mongodb_connection_string
```

## Current Prototype Notes

This repository reflects a hackathon build, so a few parts are best understood as prototype-stage work:

- the frontend is largely a polished UI prototype with seeded content
- the backend contains Socket.IO chat and whiteboard logic plus Mongo CRUD scaffolding
- some backend/database pieces are present but not fully wired into the current frontend flows
- the chat view includes demo credentials in code and should be replaced before any real deployment

## Why This Project Matters

StudyBuddy was designed around a practical student problem: staying consistent is hard when studying feels solitary. By combining community, visibility, and lightweight accountability, the project explores how software can make learning feel more shared and more motivating.

## Status

Hackathon prototype with strong product direction, UI coverage across key flows, and foundational real-time collaboration work.
