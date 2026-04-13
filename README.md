# SE Playground

A single-page portfolio website with a Spotify-inspired dark UI showcasing Solutions Engineering skills.

## Features

- **Hero Section**: Personal introduction with call-to-action buttons
- **Live API Explorer**: Real-time Spotify API search with visual results and raw JSON viewer
- **SE Scenario Simulator**: AI-powered chat interface simulating a customer debugging scenario
- **Integration Health Dashboard**: Mock monitoring dashboard with KPIs, charts, and incident simulation

## Tech Stack

- Vanilla HTML, CSS, JavaScript
- Express.js proxy server
- Spotify Web API
- OpenAI GPT-4o-mini
- Chart.js for visualizations

## Setup

1. **Install dependencies**:
   ```bash
   npm install
   ```

2. **Configure environment variables**:
   - Copy `.env.example` to `.env`
   - Add your Spotify API credentials from [Spotify Developer Dashboard](https://developer.spotify.com/dashboard)
   - Add your OpenAI API key from [OpenAI Platform](https://platform.openai.com/api-keys)

3. **Start the server**:
   ```bash
   npm start
   ```

4. **Open in browser**:
   Navigate to `http://localhost:3000`

## Environment Variables

```
SPOTIFY_CLIENT_ID=your_spotify_client_id
SPOTIFY_CLIENT_SECRET=your_spotify_client_secret
OPENAI_API_KEY=your_openai_api_key
PORT=3000
```

## Project Structure

```
.
├── server.js           # Express proxy server
├── public/
│   ├── index.html     # Main HTML structure
│   ├── styles.css     # Spotify-inspired styling
│   └── app.js         # Frontend JavaScript
├── .env.example       # Environment template
└── package.json       # Dependencies
```

## Features Walkthrough

### Live API Explorer
Search for Spotify tracks and artists. Results display as cards with album art, and you can toggle raw JSON response.

### SE Scenario Simulator
Debug a fictional integration issue with "Melodia Inc." The AI stays in character and reveals that their webhook failures stem from an expired OAuth token after the November 2025 Spotify migration.

### Integration Health Dashboard
Monitor mock integration metrics. Click "Trigger Incident" to simulate a 500 error and watch the error rate spike.

---

Built by **Halil Aybar** | *"I bridge code and customer reality."*
