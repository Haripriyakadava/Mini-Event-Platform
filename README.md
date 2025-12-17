# Mini Event Platform (MERN)

A full-stack MERN application that allows users to create, view, and RSVP to events.

## Tech Stack
- MongoDB
- Express.js
- React.js
- Node.js

## Features
- User authentication using JWT
- Create, view, edit, and delete events
- Only event creators can edit or delete events
- Image upload for events
- RSVP system with capacity enforcement
- Prevents duplicate RSVPs and overbooking

## RSVP Concurrency Handling
RSVP logic is implemented using atomic MongoDB `findOneAndUpdate` operations to ensure:
- Capacity is never exceeded
- A user cannot RSVP multiple times
- Race conditions are avoided

## Deployment
- Backend deployed on Render
- Frontend deployed on Vercel

## Live URLs
- Backend: https://mini-event-platform-cz20.onrender.com
- Frontend: https://mini-event-platform-three.vercel.app
  
## How to Run Locally

### Backend
```bash
npm install
npm start
