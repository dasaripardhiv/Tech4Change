# Tech4Change
#This is an impactful app for rural india
project structure
jeevan-rakshak/
├── client/                           # React PWA Frontend
│   ├── public/
│   │   ├── manifest.json             # PWA Install Manifest
│   │   └── service-worker.js         # Offline Caching Engine (Crucial)
│   ├── src/
│   │   ├── components/
│   │   │   ├── AIHealthAssistant.jsx # NEW: TTS, LLM, Crowd Instruction
│   │   │   ├── AuthForm.jsx          # Login, Register
│   │   │   └── SOSButton.jsx         # Geolocation & Alert
│   │   ├── context/
│   │   │   └── LanguageContext.jsx   # Multi-language logic
│   │   ├── translations/
│   │   │   ├── en.json
│   │   │   └── hi.json (and ta.json, te.json...)
│   │   └── App.jsx                   # Main Router/Layout
│
├── server/                           # Node/Express API Backend
│   ├── config/
│   │   └── db.js                     # MongoDB Connection
│   ├── controllers/
│   │   └── authController.js         # Handles User/NGO/Admin Auth
│   ├── models/
│   │   └── User.js                   # User Schema (Role: user, ngo, admin)
│   ├── routes/
│   │   └── authRoutes.js             # API routes for /api/auth
│   └── server.js                     # Express Entry Point
│
└── README.md
