<h1 align="left">Shubhi Tiwari</h1>

<p align="left">
Backend-leaning full-stack developer · AI & ML, CS undergrad (CGPA 8.0) · Building toward SDE / ML Engineer roles<br/>
Selected for <b>GSSoC 2026</b> (AI Agents Track) · Open to remote work & freelance
</p>

<p align="left">
  <img src="https://img.shields.io/badge/-Node.js-339933?style=flat-square&logo=node.js&logoColor=white" />
  <img src="https://img.shields.io/badge/-Express-000000?style=flat-square&logo=express&logoColor=white" />
  <img src="https://img.shields.io/badge/-MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white" />
  <img src="https://img.shields.io/badge/-React-20232A?style=flat-square&logo=react&logoColor=61DAFB" />
  <img src="https://img.shields.io/badge/-Next.js-000000?style=flat-square&logo=next.js&logoColor=white" />
  <img src="https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/-PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" />
</p>

I write backend systems with real auth, real error handling, and real data — not demo-shaped versions of them. Most of what's below started as a hackathon idea or a personal frustration and got rebuilt until it could survive actual use. Currently deep in DSA and system design fundamentals, one topic at a time, spaced-repetition style.

---

## Projects

Each one below includes the design decision that mattered most — not just what the stack is, but why it's shaped that way.

### First-Gen Guidance — AI scholarship & career guidance platform
**Stack:** Next.js · TypeScript · Supabase · Gemini API (`gemini-2.5-flash`) · Tailwind CSS
**What it does:** Matches first-generation students to scholarships and mentorship resources using an AI scoring layer, with a full onboarding and profile system.
**Design decision:** Mentor Q&A was originally a WhatsApp thread. Replaced it with a structured in-app system because group chat doesn't scale past a few dozen students and search inside it was effectively impossible — trading conversational ease for retrievability.
[Live →](https://first-gen-guidance.vercel.app) · [Repo →](https://github.com/shubhitiwariiii/first-gen-guidance)

### ShelfSpace — library & study space discovery
**Stack:** Next.js · TypeScript · Supabase · Tailwind CSS · OpenStreetMap
**What it does:** Surfaces nearby libraries and study spaces with pricing, timings, and amenities on a map.
**Design decision:** Data comes from a decoupled OSM ingestion pipeline with idempotent upserts, not a hardcoded list — so re-running ingestion never duplicates records, and the schema stays provider-agnostic if the data source changes later.
[Repo →](https://github.com/shubhitiwariiii/shelf-space.git)

### HealthLens — medical report analyzer
**Stack:** React 19 · Node.js · Firebase · Gemini API · Tailwind CSS
**What it does:** Turns uploaded medical reports into plain-language explanations.
**Design decision:** Built at HackDays 2026 under time pressure, so the priority was a tight upload → parse → explain pipeline over breadth of report types — narrow scope, but the core flow is solid.
[Repo →](https://github.com/AnubhavGitHub07/HealthLens)

### Daily Wage Tracker — wage & attendance management
**Stack:** React · Node.js · Express · MongoDB · JWT
**What it does:** Tracks attendance and computes wages for contractors and workers, with PDF report export.
**Design decision:** Auth is JWT-based with bcrypt hashing rather than session cookies, since the deployment splits frontend (Vercel) and backend (Render) across origins — token-based auth avoids the cross-origin cookie headache entirely.
[Repo →](https://github.com/shubhitiwariiii/daily-wage-tracker)

### Personalized Voice Assistant
**Stack:** Python · scikit-learn · Ollama (LLaMA 3)
**What it does:** A voice assistant that retains context across sessions and uses it in later responses.
**Design decision:** Intent classification runs on a lightweight Naive Bayes model instead of routing every utterance through the LLM — cheaper and faster for a small, fixed intent set, with the LLM reserved for actual generation.
[Repo →](https://github.com/shubhitiwariiii/personalized-voice-assistant)

---

## Currently working on

- **DSA** — Striver's A2Z sheet, Recursion & Backtracking → Trees → Graphs → DP
- **System design** — self-built 70-topic syllabus, tracked in Notion + Anki + a physical notebook
- **Next build** — a backend-first project centered on auth and rate limiting done properly

---

## GitHub activity

<p align="left">
  <img src="https://streak-stats.demolab.com?user=shubhitiwariiii&theme=tokyo-night&hide_border=true&background=0D1117&ring=0EA5E9&fire=0EA5E9&currStreakLabel=FFFFFF&currStreakNum=FFFFFF&sideLabels=FFFFFF&sideNums=FFFFFF&dates=FFFFFF" />
</p>

---

## Reach me

[LinkedIn](https://linkedin.com/in/shubhi-tiwari-664553329) · [LeetCode](https://leetcode.com/shubhitiwariiii) · [shubhitiwari0132@gmail.com](mailto:shubhitiwari0132@gmail.com)
