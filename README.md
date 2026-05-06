# Voting Poll App

A responsive React application built with Vite and Tailwind CSS. Users can register, log in, add poll options, vote once per account, and see live results — all persisted via a JSON Server backend and Firebase Firestore.

---

## Contributors

- [Keith Kamau](https://github.com/keithkamau)
- [Emmanuel Torris](https://github.com/emmanueltorris-rgb)
- [Emmanuel Munene](https://github.com/nesh069)
- [Favour Kendi](https://github.com/favourkendi-dev)
- [Kiplimo Kiptoo](https://github.com/kiplimokiptoo)

---

## Live Demo

[https://keithkamau.github.io/voting-poll-project/](https://keithkamau.github.io/voting-poll-project/)

---

## Features

- User authentication via Firebase (email/password and Google Sign-In)
- Add poll options
- Vote once per user account — tracked per user via Firebase Firestore
- Live vote counts and percentage progress bars
- Leading option highlighted
- Reset all votes
- Data persists via JSON Server backend hosted on Render
- Responsive on mobile and desktop
- Auto-deployed to GitHub Pages via GitHub Actions

---

## Tech Stack

- React 19
- Vite
- Tailwind CSS
- Firebase Authentication
- Firebase Firestore
- JSON Server (hosted on Render)
- React Router DOM
- GitHub Actions (CI/CD)

---

## Project Structure


src/
├── components/
│   ├── auth/
│   │   ├── login/
│   │   │   └── index.jsx
│   │   └── register/
│   │       └── index.jsx
│   ├── PollForm.jsx
│   ├── PollList.jsx
│   ├── PollOption.jsx
│   └── ProtectedRoute.jsx
├── contexts/
│   └── authContexts/
│       └── index.jsx
├── firebase/
│   ├── auth.js
│   └── firebaseConfig.js
├── App.jsx
├── App.css
├── index.css
├── main.jsx
└── router.jsx

---

## Setup

This project uses Firebase and a hosted JSON Server backend. To run it locally you will need your own Firebase project.

1. Clone the repository

```bash
   git clone https://github.com/keithkamau/voting-poll-project.git
   cd voting-poll-project
```

2.Install dependencies

```bash
   npm install
```

3.Create a Firebase project at [firebase.google.com](https://firebase.google.com), enable Authentication (Email/Password and Google) and Firestore, then replace the config in `src/firebase/firebaseConfig.js` with your own credentials.

4.Start the development server

```bash
   npm run dev
```

5.Open `http://localhost:5173` in your browser

> Poll data is fetched from a live JSON Server backend hosted on Render — no local backend setup needed.

1. Open `http://localhost:5173` in your browser

---

## Build for Production


bash
npm run build
      npm run preview

---

## Deployment

The app is automatically deployed with Github actions on every push to `main` via GitHub Actions. The JSON Server backend is hosted on Render.
EOF
