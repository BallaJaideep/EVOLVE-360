<h1 align="center">
  <br/>
  ⚡ EVOLVE-360
  <br/>
</h1>

<p align="center">
  <b>AI-Powered Full-Stack Fitness & Performance Platform</b><br/>
  <i>Track. Analyse. Recover. Evolve.</i>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react&logoColor=white"/>
  <img src="https://img.shields.io/badge/Node.js-Express-339933?style=for-the-badge&logo=node.js&logoColor=white"/>
  <img src="https://img.shields.io/badge/MongoDB-Atlas-47A248?style=for-the-badge&logo=mongodb&logoColor=white"/>
  <img src="https://img.shields.io/badge/Gemini%20AI-2.0-4285F4?style=for-the-badge&logo=google&logoColor=white"/>
  <img src="https://img.shields.io/badge/JWT-Auth-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white"/>
  <img src="https://img.shields.io/badge/Vite-5-646CFF?style=for-the-badge&logo=vite&logoColor=white"/>
</p>

---

## 📌 Overview

**EVOLVE-360** is a comprehensive, AI-driven fitness and performance management platform built for athletes, coaches, and everyday fitness enthusiasts. It combines daily readiness tracking, personalised workout planning, nutrition logging, pain analysis, rehabilitation management, and AI equipment analysis into a single, beautifully designed full-stack web application.

---

## ✨ Features

### 🧠 AI-Powered Modules
| Feature | Description |
|---|---|
| **AI Equipment Analyzer** | Upload or capture any gym equipment photo — Gemini Vision returns expert coaching protocols, technique breakdowns, and 3-level workout programs |
| **AI Workout Plan Generator** | Generates personalised weekly training plans based on readiness score, goals, and history |
| **AI Session Coach** | Provides real-time coaching feedback during workout sessions |
| **Pain Analysis Engine** | Analyses pain location, intensity, and history to suggest recovery protocols |
| **Training Analysis** | Deep-dives into training load, volume, and performance trends |

### 📊 Performance Tracking
- **Daily Readiness Score (APS)** — Athlete Performance Score calculated from HRV, sleep, stress, and soreness inputs
- **APS History Dashboard** — Visual trends, graphs, and longitudinal performance tracking
- **Functional Testing** — Standardised fitness benchmarks and mobility assessments
- **Heart Rate Monitoring** — Log and visualise heart rate data over time

### 🏋️ Workout Management
- **Workout Builder** — Browse, customise, and log workouts across all muscle groups
- **Weekly Plan** — AI-generated or manually configured weekly training schedule
- **Workout Session Logging** — Track sets, reps, weight, and RPE per exercise

### 🥗 Nutrition Tracking
- **Food Log** — Daily meal tracking with macro breakdown
- **Nutrition Targets** — Set and monitor personalised calorie/macro goals
- **Daily Nutrition Summary** — Visual daily overview of intake vs. targets
- **Water Tracker** — Hydration logging with smart reminders

### 🩹 Rehabilitation & Recovery
- **Rehab Session Manager** — Track rehabilitation exercises and recovery milestones
- **RRS (Rehabilitation Readiness Score)** — Phased recovery system with session history
- **Smart Reminders** — Automated email notifications for workouts, hydration, and rehab

### 👤 User Management
- **JWT Authentication** — Secure login & registration
- **Onboarding Flow** — Multi-step profile setup (goals, body metrics, training history)
- **Baseline Profile** — Persisted performance baseline for relative progress tracking

---

## 🛠️ Tech Stack

### Frontend
| Technology | Purpose |
|---|---|
| **React 18** + **Vite** | UI framework & lightning-fast build tooling |
| **React Router v6** | Client-side routing |
| **Vanilla CSS** + **Inline Styles** | Premium glass-morphism design system |
| **Google Fonts (Outfit)** | Typography |
| **Gemini Vision API** | Client-side AI image analysis |

### Backend
| Technology | Purpose |
|---|---|
| **Node.js** + **Express** | REST API server |
| **MongoDB Atlas** + **Mongoose** | Cloud database & ODM |
| **JWT** (jsonwebtoken) | Stateless authentication |
| **Bcrypt** | Password hashing |
| **Nodemailer** | Email notifications & reminders |
| **node-cron** | Scheduled reminder jobs |
| **Gemini 2.0 API** | Server-side AI coaching & plan generation |
| **dotenv** | Environment configuration |
| **CORS** | Cross-origin request handling |

---

## 📁 Project Structure

```
EVOLVE-360/
├── backend/
│   └── src/
│       ├── app.js                  # Express app, CORS, route mounting
│       ├── server.js               # Entry point, DB connection
│       ├── config/
│       │   └── db.js               # MongoDB Atlas connection
│       ├── controllers/            # Route handler logic
│       ├── models/                 # Mongoose schemas
│       │   ├── User.model.js
│       │   ├── DailyReadiness.model.js
│       │   ├── WeeklyPlan.model.js
│       │   ├── WorkoutSession.model.js
│       │   ├── Nutrition*.model.js
│       │   ├── PainAnalysis.model.js
│       │   ├── rehabSession.model.js
│       │   └── ...
│       ├── routes/                 # Express routers
│       │   ├── auth.routes.js
│       │   ├── workout.routes.js
│       │   ├── nutrition.routes.js
│       │   ├── readiness.routes.js
│       │   ├── rehab.routes.js
│       │   ├── pain.routes.js
│       │   └── ...
│       ├── services/               # Business logic & AI integrations
│       │   ├── ai/
│       │   ├── workout/
│       │   ├── nutrition/
│       │   ├── readiness/
│       │   ├── plan/
│       │   └── recovery/
│       ├── cron/                   # Scheduled jobs (reminders)
│       └── utils/                  # Shared helpers
│
└── frontend/
    └── src/
        ├── App.jsx                 # Router configuration
        ├── main.jsx                # React entry point
        ├── index.css               # Global design tokens
        ├── api/                    # Axios API layer
        ├── components/             # Reusable UI components
        ├── context/                # React Context (Auth, etc.)
        ├── pages/
        │   ├── Login.jsx
        │   ├── Register.jsx
        │   ├── Onboarding.jsx
        │   ├── Dashboard.jsx
        │   ├── Workout.jsx
        │   ├── Readiness.jsx
        │   ├── Nutrition.jsx
        │   ├── Watertracker.jsx
        │   ├── APS.jsx
        │   ├── APSHistory.jsx
        │   ├── Analyzer.jsx        # AI Equipment Analyzer
        │   ├── Rehab.jsx
        │   ├── Painanalysis.jsx
        │   ├── TrainingAnalysis.jsx
        │   ├── Functionaltest.jsx
        │   ├── HearRate.jsx
        │   └── Model.jsx
        └── utils/
```

---

## 🚀 Getting Started

### Prerequisites
- **Node.js** v18+
- **npm** v9+
- A **MongoDB Atlas** cluster
- A **Google Gemini API Key** ([Get one here](https://aistudio.google.com/app/apikey))
- A **Gmail App Password** (for email reminders)

---

### 1. Clone the Repository

```bash
git clone https://github.com/BallaJaideep/EVOLVE-360.git
cd EVOLVE-360
```

---

### 2. Backend Setup

```bash
cd backend
npm install
```

Create a `.env` file in the `backend/` directory:

```env
PORT=5000
MONGO_URI=your_mongodb_atlas_connection_string
JWT_SECRET=your_super_secret_jwt_key
GEMINI_API_KEY=your_gemini_api_key
BASE_URL=http://localhost:5000
EMAIL_USER=your_gmail@gmail.com
EMAIL_PASS=your_gmail_app_password
```

Start the backend dev server:

```bash
npm run dev
```

The API will be live at **http://localhost:5000**

---

### 3. Frontend Setup

```bash
cd ../frontend
npm install
npm run dev
```

The app will be available at **http://localhost:5173** (or `5174` if 5173 is in use).

---

## 🔑 Environment Variables Reference

| Variable | Description | Required |
|---|---|---|
| `PORT` | Backend server port (default: `5000`) | ✅ |
| `MONGO_URI` | MongoDB Atlas connection string | ✅ |
| `JWT_SECRET` | Secret key for signing JWT tokens | ✅ |
| `GEMINI_API_KEY` | Google Gemini AI API key | ✅ |
| `BASE_URL` | Backend base URL (used in email links) | ✅ |
| `EMAIL_USER` | Gmail address for sending reminders | Optional |
| `EMAIL_PASS` | Gmail App Password (not your main password) | Optional |

> ⚠️ **Never commit your `.env` file.** It is already excluded by `.gitignore`.

---

## 📡 API Endpoints (Overview)

| Method | Endpoint | Description |
|---|---|---|
| `POST` | `/api/auth/register` | Register a new user |
| `POST` | `/api/auth/login` | Login & receive JWT |
| `GET/POST` | `/api/profile` | Get / update user profile |
| `POST` | `/api/readiness` | Log daily readiness |
| `GET/POST` | `/api/workout` | Workout sessions |
| `GET/POST` | `/api/plan` | Weekly training plans |
| `GET/POST` | `/api/nutrition` | Nutrition targets |
| `GET/POST` | `/api/food` | Daily food logs |
| `GET/POST` | `/api/nutrition-summary` | Daily nutrition summary |
| `POST` | `/api/aps` | Log APS score |
| `GET/POST` | `/api/rehab/rrs/*` | Rehab sessions & RRS |
| `POST` | `/api/pain-analysis` | Log pain data |
| `POST` | `/api/training-analysis` | Training load analysis |
| `POST` | `/api/functional-test` | Functional assessment |
| `POST` | `/api/ai-session` | AI coaching session |
| `GET/POST` | `/reminders` | Workout reminders |
| `GET/POST` | `/water-reminders` | Hydration reminders |

---

## 🎨 Design System

EVOLVE-360 uses a custom **light glass-morphism** design language:

- **Primary accent:** Indigo-Violet `#6366f1` → `#8b5cf6`
- **CTA gradient:** `linear-gradient(135deg, #2563eb, #6366f1, #7c3aed)`
- **Glass cards:** `rgba(255,255,255,0.85)` + `backdrop-filter: blur(16px)`
- **Background:** Animated tri-colour blobs on `#f8fafc → #eff6ff → #eef2ff`
- **Typography:** [Outfit](https://fonts.google.com/specimen/Outfit) (Google Fonts)
- **Micro-animations:** `fadeUp`, `blob`, `spin` keyframes throughout

---

## 🔒 Security Notes

- All passwords are hashed with **bcrypt** before storage
- JWTs are signed with a secret key and validated on every protected route
- The `.env` file is excluded from version control via `.gitignore`
- CORS is restricted to known frontend origins

---

## 📜 License

This project is for personal and educational use. All rights reserved © 2026 **Balla Jaideep**.

---

<p align="center">Built by <b>Balla Jaideep</b></p>
