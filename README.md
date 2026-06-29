# 🦸 TogetherFix — Hyperlocal Problem Solver

> An AI-powered civic issue reporting platform that enables citizens to identify, report, verify, track, and resolve community problems through collaboration, data, and intelligent automation.

![TogetherFix](https://img.shields.io/badge/Status-Active-green) ![Gemini](https://img.shields.io/badge/AI-Gemini%201.5%20Flash-blue) ![Google](https://img.shields.io/badge/Platform-Google%20AI%20Studio-orange)

---

## 🌐 Live Demo
👉 **[togetherfix.run.app](https://togetherfix-603635732280.asia-southeast1.run.app)** 

---

## 📌 Problem Statement
Communities in India face a fragmented, opaque process for reporting and resolving civic issues like potholes, water leakages, broken streetlights, and garbage overflow. Citizens have no easy way to:
- Report issues with evidence
- Track resolution progress
- Hold authorities accountable
- Collaborate with neighbours

**TogetherFix** solves this end-to-end — from reporting to resolution — using AI and community participation.

---

## 🚀 Key Features

### 🤖 AI-Powered (Gemini 1.5 Flash)
| Feature | Description |
|---|---|
| **Image Categorization** | Upload a photo → Gemini Vision auto-identifies issue type, severity, and responsible department |
| **Complaint Drafter** | Gemini writes a formal complaint letter to the correct authority automatically |
| **Predictive Insights** | AI detects patterns across reports and surfaces proactive alerts (e.g. pothole hotspots before monsoon) |
| **Duplicate Detection** | AI flags if a similar issue has already been reported nearby |
| **Resolution ETA** | AI estimates how long resolution will take based on category and historical data |
| **Department Routing** | Automatically routes issues to PWD, Jal Board, Municipal Corp, or Electricity Dept |

### 🗺️ Core Platform
- **Geo-tagged Reporting** — GPS location capture with interactive map view
- **Photo/Video Upload** — Visual evidence attached to every report
- **Community Verification** — Citizens confirm issues they see ("I see this too")
- **Real-Time Status Tracking** — Reported → Verified → In Progress → Resolved
- **Admin / Municipality Panel** — Officials update issue status, view workload by department
- **Impact Dashboard** — Resolution rates, category breakdowns, trend charts

### 🎮 Gamification
- **XP Points** — Earn points for reporting (+10), verifying (+5), resolving (+20)
- **Badges** — Street Guardian, First Responder, Verifier, Area Champion
- **Leaderboard** — Top contributors ranked by XP monthly and all-time

---

## 🛠️ Technologies Used

### Google Technologies
| Technology | Usage |
|---|---|
| **Gemini 1.5 Flash API** | Image analysis, complaint drafting, predictive insights |
| **Google AI Studio** | Development environment + deployment |
| **Google Cloud Run** | Hosting and scalable deployment |
| **Google Maps JavaScript API** | Geo-tagging, map display, location pinning |
| **Firebase Firestore** | Real-time database for issues and users |
| **Firebase Auth** | Google Sign-In for citizens |
| **Firebase Storage** | Photo and video uploads |
| **Firebase Cloud Messaging** | Push notifications on status updates |

### Other Technologies
| Technology | Usage |
|---|---|
| HTML5 / CSS3 / JavaScript | Frontend (single-file, no framework required) |
| Geolocation API | GPS location capture |
| Web Share API | Native share on mobile |
| LocalStorage | XP and session persistence |

---

## 🤖 Agentic Pipeline (Multi-Step AI)

The core AI agent follows a multi-step autonomous pipeline:

```
📸 Image Upload
     ↓
🔍 Gemini Vision — categorize issue, detect severity, identify department
     ↓
🔄 Duplicate Check — geo + category query against existing reports
     ↓
📄 Complaint Drafter — Gemini generates formal letter to right authority
     ↓
🏛️ Auto-Route — issue assigned to PWD / Jal Board / Muni Corp / Electricity
     ↓
📊 Pattern Analysis — AI aggregates reports, surfaces predictive insights
     ↓
🔔 Notification — citizen and authority notified on status changes
```

This is not a single API call — it's a chain of AI reasoning steps that perceive, classify, act, and monitor.

---

## 📁 Project Structure

```
togetherfix/
├── index.html          # Complete single-file frontend application
├── README.md           # This file
└── docs/
    └── project.md      # Project description (Google Doc mirror)
```

---

## ⚡ Getting Started Locally

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/togetherfix.git
   cd togetherfix
   ```

2. Open `index.html` in any browser — no build step needed.

3. Enter your Gemini API key in the app header (get one free at [aistudio.google.com/apikey](https://aistudio.google.com/apikey))

4. All AI features activate instantly.

---

## 🚀 Deployment (Google AI Studio)

1. Go to [aistudio.google.com](https://aistudio.google.com) → Build Mode
2. Paste the contents of `index.html`
3. Click **Deploy** → Google Cloud Run deploys automatically
4. Get your public `*.run.app` URL

Full deployment docs: [ai.google.dev/gemini-api/docs/aistudio-deploying](https://ai.google.dev/gemini-api/docs/aistudio-deploying)

---

## 📊 Evaluation Criteria Coverage

| Criteria | How We Address It |
|---|---|
| **Problem Solving & Impact (20%)** | End-to-end civic issue lifecycle — report → verify → track → resolve |
| **Agentic Depth (20%)** | Multi-step Gemini pipeline: vision → categorize → route → draft → monitor |
| **Innovation & Creativity (20%)** | Predictive insights, auto-complaint drafter, duplicate detection, gamification |
| **Google Technologies (15%)** | Gemini API, AI Studio, Cloud Run, Maps, Firebase |
| **Product Experience (10%)** | Dark-mode UI, mobile-responsive, real-time updates, smooth UX |
| **Technical Implementation (10%)** | Gemini Vision integration, geo-queries, live status pipeline |
| **Completeness & Usability (5%)** | 7 fully working views, admin panel, citizen panel |

---


