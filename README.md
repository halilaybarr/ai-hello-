# SE Playground

**Halil Aybar** — *APIs, customers, and the chaos in between.*

A portfolio site built with real APIs. Search Spotify live, debug a broken integration with an AI-powered customer, and poke at a mock monitoring dashboard.

---

## What's in it

| Section | What it does |
|---------|-------------|
| 🔍 **Live API Explorer** | Real Spotify API search — results as cards + raw JSON toggle |
| 🤖 **SE Scenario Simulator** | AI roleplay: debug a broken webhook with a fictional enterprise customer |
| 📊 **Integration Health Dashboard** | Mock monitoring — KPIs, charts, event log, incident simulation |

---

## ✨ Features

### 🔍 Live API Explorer
Hits the real Spotify API. Search any artist or track, get results as cards, toggle the raw JSON if you want to see what's actually coming back.

### 🤖 SE Scenario Simulator
You're the SE. Chat with "Melodia Inc." — a fictional customer whose Spotify webhooks stopped working. The AI plays the customer and drops clues as you ask the right questions.

**Root cause:** expired OAuth token from the November 2025 Spotify API migration.

### 📊 Integration Health Dashboard
Uptime, latency, error rate, a Chart.js webhook timeline, and a live event log. Hit **Trigger Incident** to simulate a 500 spike and watch the dashboard react.

---

## 🛠️ Tech Stack

- **Frontend:** Vanilla HTML, CSS, JavaScript
- **Backend:** Node.js + Express (proxy server to protect API credentials)
- **APIs:** Spotify Web API (Client Credentials flow), OpenAI GPT-4o-mini
- **Visualizations:** Chart.js
- **Auth pattern:** OAuth 2.0 Client Credentials, server-side secret management

---

## 🚀 Setup

### 1. Install dependencies
```bash
npm install
```

### 2. Configure environment variables
```bash
cp .env.example .env
```

Open `.env` and fill in your credentials:

```env
SPOTIFY_CLIENT_ID=your_spotify_client_id
SPOTIFY_CLIENT_SECRET=your_spotify_client_secret
OPENAI_API_KEY=your_openai_api_key
PORT=3000
```

**Get credentials:**
- Spotify: [developer.spotify.com/dashboard](https://developer.spotify.com/dashboard)
- OpenAI: [platform.openai.com/api-keys](https://platform.openai.com/api-keys)

### 3. Start the server
```bash
npm start
```

### 4. Open in browser
```
http://localhost:3000
```

---

## 📁 Project Structure

```
se-playground/
├── server.js           # Express proxy — keeps API secrets off the frontend
├── public/
│   ├── index.html      # Single-page layout
│   ├── styles.css      # Spotify-inspired dark UI
│   └── app.js          # Frontend logic — API calls, chat loop, dashboard
├── .env.example        # Credential template
└── package.json
```

---

## 👨‍💻 About

**Halil Aybar** — Full-stack engineer, former ops manager (Starbucks, 4 years). Looking for SE / Forward Deployed Engineer roles.

- React + Node.js, deployed in production
- Managed teams of 15+, $38K/week in operations
- Comfortable talking to engineers and non-engineers alike

