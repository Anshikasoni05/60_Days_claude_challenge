# Day 8 — 60-Day Claude Challenge 🌍

## Task
Build a **Personal Environmental Health Analyzer** — a fully interactive Claude Artifact that turns live AQI and water-quality data into a personal environmental health report.

## What I Did
- Prompted Claude to act as a Senior Data Analyst, Environmental Researcher, UX Designer, and Frontend Dashboard Developer in one.
- Claude web-searched live AQI, PM2.5, and PM10 readings for 10 major Indian cities (Delhi, Mumbai, Bengaluru, Chennai, Kolkata, Hyderabad, Pune, Ahmedabad, Jaipur, Agra) plus published water-quality studies (CPCB, BIS tap-water survey, Urban Water Journal groundwater study).
- It cleaned and structured the data, computed an Environmental Health Score per city (Air Score + Water Score), and generated a complete single-file HTML dashboard — no code snippets, a fully working downloadable `index.html`.

## Key Features Built
- 📊 Key metrics strip (avg AQI, highest/lowest AQI city, cities analyzed, health score)
- 📈 5 live charts: AQI, PM2.5, PM10 comparison, city ranking, AQI category distribution
- 🎛 Interactive filters: pollutant selector, AQI range slider, health-risk tier, city chips, two-city comparison mode
- 📋 Clickable city cards → detailed health impact breakdown (lungs, sleep, energy, exercise, long-term health + hair/skin impact from water quality)
- 🚦 Colour-coded AQI categories (Good → Severe) with 🟢🟡🔴 risk indicators
- 🧾 Personal Report Card with A–F grades for Air, Water, Hair Risk, Skin Risk
- 💡 Auto-generated insights: top cleanest/most polluted cities, anomalies, surprising observations, recommended actions
- 🧴 Personalized recommendations across 6 tabs: daily actions, indoor air, outdoor activity, hair care, skin care, water improvement
- 🎨 Dark, glassmorphism, mobile-responsive UI with an animated "breathing ring" health-score gauge as the signature visual

## Learnings
- Prompt engineering for multi-persona tasks (analyst + researcher + designer + developer) works best when the output contract is spelled out explicitly (no code snippets, full working artifact only).
- Grounding a dashboard in **real, cited, live-searched data** — instead of placeholder numbers — makes the analysis section (anomalies, trends, surprising observations) genuinely meaningful instead of generic filler text.
- Turning raw pollution numbers into embodied, personal impact statements (sleep, skin, hair) makes environmental data far more relatable than a plain AQI chart.

## Artifact
`index.html` — complete, downloadable, interactive dashboard (screenshots attached in this folder).

---
#60DayClaudeChallenge
