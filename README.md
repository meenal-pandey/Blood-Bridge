<<<<<<< HEAD
# BloodBridge — Full-Stack Final Prototype

This package connects the existing BloodBridge prototype UI to a real Node.js HTTP API and a persistent SQLite database. It is intentionally dependency-free at runtime: Node.js built-in modules provide the web server, SQLite database, SSE events, routing, and crypto utilities.

## Requirements
- Node.js 22.5+ (22 LTS recommended)

## Run locally
```powershell
cd BloodBridge_Final_FullStack
npm start
```
No `npm install` is required.

Open:
- http://localhost:3000
- http://localhost:3000/api/health

The first run automatically creates `data/bloodbridge.db` and seeds demo inventory, donors, requests, notifications and audit data.

## Full-stack flows implemented
- Persistent donor registration
- Persistent emergency request creation
- Emergency request filtering
- Broadcast pending requests
- Persistent notifications + mark-all-read
- Persistent audit trail
- Backend AI matching endpoint
- Inventory filtering + CSV export
- Global search endpoint
- Demo OTP authentication with backend session token
- Server-Sent Events for live UI refresh after backend changes

## Important production notes
- The OTP endpoint is demo authentication. For production, integrate an approved OTP provider and never expose an OTP in an API response.
- The AI engine is decision support only and must not independently authorize transfusion. Clinical compatibility, laboratory testing, donor eligibility and clinician approval remain mandatory.
- Keep Google Maps keys in environment variables and restrict them by API and application/domain.
- SQLite is excellent for this prototype/local demo. For a multi-instance production deployment, use PostgreSQL/Supabase or another managed database.
=======
# 🩸 BloodBridge

### Real-Time Blood Network & Intelligent Matching Dashboard

BloodBridge is a prototype command-center dashboard designed to connect **hospitals, blood banks, donors and patients** through a centralized blood management and emergency response workflow.

The platform provides real-time visibility into blood availability, emergency requests, inventory, donor networks, AI-assisted compatibility matching, analytics and healthcare network operations.

## 🚀 Features

- 🩸 Real-time blood inventory dashboard
- 🚨 Emergency blood request management
- 🤖 AI-assisted blood compatibility matching
- 🏥 Hospital network management
- 🩸 Blood bank management
- 👤 Donor network
- 🗺️ Live healthcare network map
- 🔔 Notification center
- 📊 Analytics & reports
- 📋 Audit trail
- 📦 Expiry-aware inventory management
- 📱 Responsive interface for different screen sizes

## 🧠 Blood Matching Workflow

```text
Emergency Request
        ↓
AI Analysis
        ↓
Compatibility Check
        ↓
Inventory Analysis
        ↓
Distance & Response Time
        ↓
Best Match
        ↓
Confirmation
        ↓
Tracking
```

## 🛠️ Technologies Used

- HTML5
- CSS3
- JavaScript
- Responsive Web Design
- CSS Grid & Flexbox
- Browser APIs

## ⚠️ Disclaimer

BloodBridge is a **prototype and decision-support demonstration**.

The blood compatibility workflow shown in the application must not be used as a substitute for qualified healthcare professionals, laboratory testing, crossmatching procedures or clinical decision-making.

## 🌐 Live Demo

Coming soon — GitHub Pages deployment.

## 📸 Screenshots

Screenshots of the dashboard can be added here.

## 👨‍💻 Project Status

Prototype / Hackathon Project

---

Made with ❤️ for improving emergency blood coordination.
>>>>>>> 7a2c887232889e3ce672642a6ad927f3b8c987d0
