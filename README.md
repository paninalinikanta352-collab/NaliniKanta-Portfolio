# Nalinikanta Pani — Portfolio

Personal portfolio of **Nalinikanta Pani** — Full Stack Dev, Applied AI & Data Science @ IIT Jodhpur.

**Live:** https://paninalinikanta352-collab.github.io/NaliniKanta-Portfolio/

## Built with
- Pure HTML + CSS + JavaScript — single file, zero frameworks
- Vanilla animations: typewriter, 3D tilt, scramble text, canvas constellation, nav wipe
- Live GitHub stats via GitHub Public API

## Projects
- **StudentVault** — Notes sharing backend (FastAPI, JWT auth)
- **LinkBolt API** — URL shortener with click analytics (FastAPI)
- **CivicFix** — Civic issue reporting platform (FastAPI + Next.js) → [Live app](https://civicfix-web.onrender.com) · [API docs](https://civicfix-bl4k.onrender.com/docs)
- **Expense Tracker** — Browser-only tracker, localStorage + canvas chart ([live](https://paninalinikanta352-collab.github.io/expense-tracker/))
- **Weather Board** — Open-Meteo dashboard, no API key ([live](https://paninalinikanta352-collab.github.io/weather-board/))
- **MyShop** — Full-stack e-commerce MVP (Next.js + FastAPI + PostgreSQL + Razorpay)

### 🏛️ CivicFix — [GitHub repo](https://github.com/paninalinikanta352-collab/CivicFix)
Full stack. Citizen → worker → resolved, with every step visible.

Citizens report potholes, water leaks, garbage or broken streetlights with a **photo + GPS/location**. A **0–100 explainable risk engine** ranks every issue on urgency and age, so admins fix the dangerous ones first, not the oldest first. Admins create worker accounts and assign issues; workers push live status updates — `reported → assigned → in_progress → resolved` — and citizens track the whole timeline end to end.

**Inside the build**
- **JWT auth with 3 roles** — user / admin / worker, plus email OTP verification (SMTP, dev mode returns the code)
- **AI category suggestion** — Gemini suggests a category from title + description; strictly optional, never overrides the citizen's own pick, and fails open (blocked key = no suggestion, never a blocked report)
- **AI photo detection** — offline zero-shot CLIP (ONNX) flags likely fake uploads
- **Deployed on Render free tier** — Next.js web frontend + FastAPI backend, separate services
- **Live VLOBL battle-testing** — the CORS-origins-as-config lesson came from the real deploy, not theory

`FastAPI` · `Next.js 15` · `React` · `SQLite` · `JWT Auth` · `Gemini` · `CLIP (ONNX)` · `Render`

## Run locally
Clone and open `index.html` in any browser.
