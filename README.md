# EczeMate+ 🩺

AI-Powered Eczema Management Platform built with React, Vite, Firebase, and OpenAI.

## Tech Stack

- **Frontend:** React 18 + Vite 7
- **Styling:** Tailwind CSS v4
- **Backend/Auth:** Firebase (Authentication + Firestore)
- **AI:** OpenAI API
- **Charts:** Chart.js / Recharts
- **Routing:** React Router v6
- **Deployment:** Vercel

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or higher)
- A Firebase project with **Email/Password Auth** and **Firestore** enabled

### Installation

```bash
git clone https://github.com/Mikaaroni/fyp.git
cd fyp
npm install
```

### Environment Variables

Create a `.env` file in the root directory with the following configuration:

```env
VITE_FIREBASE_API_KEY=AIzaSyA9dcYIBsVorIzZb9fMP7EqfELMO71sqQI
VITE_FIREBASE_AUTH_DOMAIN=eczemate-c2083.firebaseapp.com
VITE_FIREBASE_PROJECT_ID=eczemate-c2083
VITE_FIREBASE_STORAGE_BUCKET=eczemate-c2083.firebasestorage.app
VITE_FIREBASE_MESSAGING_SENDER_ID=463741774944
VITE_FIREBASE_APP_ID=1:463741774944:web:a31cea6d0577776ec1e705
VITE_FIREBASE_MEASUREMENT_ID=G-FV9RD6RTMB
```

### Run the App

```bash
npm run dev
```

The app will be available at `http://localhost:5173/`

### Build for Production

```bash
npm run build
npm run preview
```

## Firebase Setup

1. Go to the [Firebase Console](https://console.firebase.google.com/)
2. Select the **eczemate-c2083** project
3. Enable **Authentication** → **Sign-in method** → **Email/Password**
4. Create a **Firestore Database** (start in test mode)

## Project Structure

```
src/
├── auth/           # Login & Signup pages
├── assets/         # Static assets
├── components/     # Reusable UI components
├── features/       # Feature modules
├── firebase/       # Firebase config & helpers
├── pages/          # App pages (Patient, Doctor, Admin dashboards)
├── styles/         # Global styles
├── App.jsx         # Root component with routing
└── main.jsx        # Entry point
api/
├── chat.js         # OpenAI chat endpoint
└── analyze-triggers.js  # Trigger analysis endpoint
```

## Roles

- **Patient** — Track symptoms, log triggers, view insights
- **Doctor** — Monitor patients, provide recommendations
- **Admin** — Manage users, approve doctor registrations
