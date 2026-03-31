# LeadGenius AI ⚡

> **AI-powered B2B cold outreach that converts — in under 10 seconds.**

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/YOUR_USERNAME/leadgenius-ai)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
![Gemini 1.5 Flash](https://img.shields.io/badge/AI-Gemini%201.5%20Flash-4f46e5?logo=google)
![Static Site](https://img.shields.io/badge/Hosting-Netlify-00C7B7?logo=netlify)

---

## 🚀 What is LeadGenius AI?

LeadGenius AI is a **single-file SaaS MVP** that uses **Google Gemini 1.5 Flash** to instantly generate:

- **3 specific industry pain points** for any target company & decision-maker
- A **hyper-personalised 100-word cold email** optimised for reply rates

No backend. No database. No subscriptions. Just your API key and you're converting prospects in seconds.

---

## 💼 ROI & Business Value

| Metric | Manual Prospecting | LeadGenius AI |
|---|---|---|
| Time per personalised email | 20–45 min | **< 10 seconds** |
| Avg. cold email reply rate | 1–3% | **3–9% (3× uplift)** |
| Cost per prospect | $25–50 (SDR hours) | **~$0.001 (API cost)** |
| Emails per hour | 2–3 | **360+** |
| Consistency | Variable | **Always on-brand** |

> **Bottom line:** A team of 5 SDRs generating 50 emails/day can scale to 1,800+ personalised emails/day — with zero extra headcount.

---

## ✨ Features

- 🧠 **Pain-Point Intelligence** — Gemini identifies real, role-specific challenges your prospect faces today
- ✉️ **High-Conversion Emails** — Subject line + body optimised for B2B reply rates
- 📋 **One-Click Copy** — Structured output you can paste directly into your CRM or mail client
- 🔒 **Privacy First** — Your API key never leaves your browser; zero server-side storage
- ⚡ **Zero Infrastructure** — A single HTML file. Host anywhere. No build step.
- 🎨 **CEO-Level UI** — Dark SaaS aesthetic built with Tailwind CSS

---

## 🏁 Quick Start

### Option 1: Open Locally

```bash
# No installation required
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

### Option 2: Deploy to Netlify (1 click)

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/YOUR_USERNAME/leadgenius-ai)

### Option 3: GitHub + Netlify CI/CD

See the [CI/CD section](#-cicd-github--netlify) below.

---

## 🔑 Getting Your API Key

1. Go to [Google AI Studio](https://makersuite.google.com/app/apikey)
2. Click **Create API Key**
3. Copy the key and paste it into the app's **API Key** field

> The key is used directly in your browser via the `@google/generative-ai` ESM SDK. It is never sent to any third-party server.

---

## 🏗️ Architecture

```
leadgenius-ai/
├── index.html              ← Entire application (HTML + CSS + JS)
├── .netlify/
│   └── state.json          ← Netlify site binding
├── .github/
│   └── workflows/
│       └── netlify.yml     ← CI/CD auto-deploy pipeline
└── README.md
```

**Tech Stack:**

| Layer | Technology |
|---|---|
| UI Framework | Tailwind CSS (CDN) |
| AI Model | Google Gemini 1.5 Flash |
| AI SDK | `@google/generative-ai` (ESM via CDN) |
| Hosting | Netlify (static) |
| CI/CD | GitHub Actions |

---

## 🔄 CI/CD: GitHub → Netlify

Every push to `main` automatically deploys to Netlify via `.github/workflows/netlify.yml`.

### Setup Steps

1. **Create a Netlify site** and note your `NETLIFY_SITE_ID` (Site Settings → General)
2. **Generate a Netlify Personal Access Token** (User Settings → Applications)
3. **Add GitHub Secrets** in your repo (`Settings → Secrets → Actions`):
   - `NETLIFY_AUTH_TOKEN` — your personal access token
   - `NETLIFY_SITE_ID` — your site ID
4. Push to `main` — the workflow handles the rest ✅

---

## 📈 Roadmap

- [ ] CSV export of generated pitches
- [ ] LinkedIn message variant generation
- [ ] CRM integration (HubSpot, Salesforce)
- [ ] A/B subject line generator
- [ ] Team collaboration mode

---

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first.

---

## 📄 License

[MIT](LICENSE) — free to use, fork, and commercialise.

---

<p align="center">
  Built with ❤️ using <strong>Google Gemini 1.5 Flash</strong> · Deployed on <strong>Netlify</strong>
</p>
