<div align="center">

<img src="assets/svg/banner.svg" alt="CapAble: See Capability. Prove Potential. Enable Transition." width="100%">

<a href="https://readme-typing-svg.demolab.com"><img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&pause=1200&color=2354D6&center=true&vCenter=true&width=780&lines=A+r%C3%A9sum%C3%A9+is+a+claim.+A+Capability+Twin+is+a+record.;Verified+skills+%E2%86%92+fair+matching+%E2%86%92+human+decision.;Hire+on+what+people+can+DO%2C+not+where+they+studied." alt="Typing animation"></a>

<br>

[![Live prototype](https://img.shields.io/badge/%F0%9F%9A%80%20Live%20Prototype-capable--alpha.vercel.app-2354d6?style=for-the-badge)](https://capable-alpha.vercel.app)
[![Demo video](https://img.shields.io/badge/%E2%96%B6%20Watch%20Demo-YouTube-c4302b?style=for-the-badge)](https://www.youtube.com/watch?v=InX9qLdTvsY)
[![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97%20Model-accesshire--mpnet--final-FFD21E?style=for-the-badge&labelColor=000)](https://huggingface.co/Devengoyal/accesshire-mpnet-final)

![Next.js](https://img.shields.io/badge/Next.js-16-000000?style=flat-square&logo=nextdotjs)
![React](https://img.shields.io/badge/React-19-61DAFB?style=flat-square&logo=react&logoColor=000)
![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=flat-square&logo=typescript&logoColor=fff)
![Tailwind](https://img.shields.io/badge/Tailwind-4-06B6D4?style=flat-square&logo=tailwindcss&logoColor=fff)
![FastAPI](https://img.shields.io/badge/FastAPI-ML%20service-009688?style=flat-square&logo=fastapi&logoColor=fff)
![PyTorch](https://img.shields.io/badge/PyTorch-CPU-EE4C2C?style=flat-square&logo=pytorch&logoColor=fff)
![scikit-learn](https://img.shields.io/badge/scikit--learn-predictive%20models-F7931E?style=flat-square&logo=scikitlearn&logoColor=fff)
![Gemini](https://img.shields.io/badge/Google%20Gemini-agents-8E75B2?style=flat-square&logo=googlegemini&logoColor=fff)
![Supabase](https://img.shields.io/badge/Supabase-auth-3ECF8E?style=flat-square&logo=supabase&logoColor=fff)
![Vercel](https://img.shields.io/badge/Vercel-deployed-000?style=flat-square&logo=vercel)
![Docker](https://img.shields.io/badge/Docker-ML%20service-2496ED?style=flat-square&logo=docker&logoColor=fff)
![Responsible AI](https://img.shields.io/badge/Responsible%20AI-human%20in%20the%20loop-0f9d8a?style=flat-square)
![Accessibility](https://img.shields.io/badge/Accessibility-OpenDyslexic%20%7C%20high%20contrast-7c3aed?style=flat-square)

# CapAble: Capability Intelligence & Talent Operating System

### Hiring on what people can *do*, not where they studied, what they were titled, or how long their résumé is.

**[Problem](#-the-problem) · [Solution](#-our-solution) · [Demo](#-demo) · [Twin](#-the-capability-twin) · [Features](#-features) · [AI engine](#-the-ai-engine) · [Architecture](#-architecture) · [Status](#-project-status) · [Run locally](#-run-it-locally) · [Roadmap](#-roadmap) · [Contributors](#-contributors)**

</div>

---

## 🔗 Quick links

| | Resource | Link |
|:-:|:--|:--|
| 🚀 | Live prototype | [capable-alpha.vercel.app](https://capable-alpha.vercel.app) |
| 🎬 | Demo video | [youtube.com/watch?v=InX9qLdTvsY](https://www.youtube.com/watch?v=InX9qLdTvsY) |
| 💻 | Frontend repository | [Devengoyal885/Access-Hire](https://github.com/Devengoyal885/Access-Hire) *(copy in [`frontend/`](frontend/))* |
| 🧠 | Machine learning repository | [Devengoyal885/accesshireml](https://github.com/Devengoyal885/accesshireml) *(copy in [`ml-service/`](ml-service/))* |
| 🤗 | Trained model | [accesshire-mpnet-final](https://huggingface.co/Devengoyal/accesshire-mpnet-final) |
| 📦 | Dataset | [Google Drive](https://drive.google.com/drive/folders/17lZrwG7Z14cZZMHHAoW76IvVGWXqVab2) *(you may need to request access)* |
| 📋 | Feature audit | [`docs/FEATURE_AUDIT.md`](docs/FEATURE_AUDIT.md) |

---

## 💥 The problem

> **Talent is not scarce. Capability is hidden.**

Static résumés, degree and employer-name filters, self-declared skills and career gaps push capable people out of the hiring funnel. Employers cannot verify what a candidate can really do, and institutions cannot see the true skill picture of their own students.

| 😟 Candidate | 🏢 Employer | 🏛️ Institution |
|:--|:--|:--|
| Strong work, weak pedigree, so **filtered out** | Keyword-stuffed PDFs with **no proof** | Placement data is **scattered and manual** |
| Career gaps read as **red flags** | Hiring on **brand names**, not skill | NAAC / NIRF reporting is **painful** |
| No clear path from *now* to *target role* | **Bias** creeps into shortlists | No view of **curriculum vs market gap** |

<p align="center"><img src="assets/diagrams/stakeholders.png" alt="One capability record serving candidates, institutions, employers and human reviewers" width="90%"></p>

---

## 💡 Our solution

CapAble replaces the static résumé with a **living Capability Twin** and moves every person through one loop: understand, translate, find the gap, verify, match fairly, and let a human decide.

<img src="assets/svg/journey.svg" alt="Understand, Translate, Find the gap, Verify, Match fairly, Human decides, with a feedback loop to the Capability Twin" width="100%">

```mermaid
flowchart LR
  A[📄 Evidence<br/>resume, projects, GitHub, work] --> B[🧠 Capability Translator]
  B --> C[🧬 Capability Twin]
  C --> D[🎯 Role-specific skill gap]
  D --> E[📚 Shortest learning path]
  D --> F[🛠️ Practical verification]
  F --> G[✅ Verified evidence]
  G --> C
  C --> H[⚖️ Opportunity match + bias audit]
  H --> I[🧑‍⚖️ Human decision]

  style C fill:#2354d6,color:#fff,stroke:#0c1f3d,stroke-width:2px
  style I fill:#0f9d8a,color:#fff,stroke:#0c1f3d,stroke-width:2px
```

### Four pillars

<img src="assets/svg/pillars.svg" alt="Verify, Match, Audit, Decide" width="100%">

### Before vs after

| | ❌ Traditional hiring | ✅ With CapAble |
|:--|:--|:--|
| **Unit of trust** | A résumé claim | A verified capability record |
| **Filter** | College, title, keywords | Verified skill and minimum score |
| **Career gaps** | Red flag | Evidence of what the person can do now |
| **Skill proof** | Self-declared | Projects, repos, assessments, with a confidence score |
| **Shortlist fairness** | Unchecked | Bias-audit agent flags skewed lists |
| **Final call** | Opaque | AI recommends, **a human decides** |

---

## 🎬 Demo

[![Watch the CapAble project demo](assets/illustrations/video-poster.png)](https://www.youtube.com/watch?v=InX9qLdTvsY)

<p align="center"><i>Click the image to watch the demo on YouTube, or try the <a href="https://capable-alpha.vercel.app">live prototype</a>.</i></p>

---

## 📊 At a glance

<img src="assets/svg/stats.svg" alt="469 capabilities, 12,000+ hiring records, 4 portals, 6 dimensions, 4 agent routes, 0 fabricated claims" width="100%">

Also in the platform: **4** job sources aggregated and de-duplicated, and **3** predictive models (salary, hike, seniority).

```mermaid
mindmap
  root((CapAble))
    Candidates
      Capability Twin
      Skill gap and learning path
      Mock interviews
      Tailored resume
    Employers
      Capability based search
      Pipeline Kanban
      Interview scheduler
      Bias audit
    Institutions
      Placement dashboard
      Drive management
      NAAC and NIRF reports
      Curriculum gap analytics
    Faculty
      Student endorsements
      Mentorship
      Research and FDP
    AI and Data
      Capability Translator
      Predictive engine
      Gemini agents
      Voice AI
```

---

## 🧬 The Capability Twin

<table>
<tr>
<td width="55%" align="center"><img src="assets/svg/twin_radar.svg" alt="Radar chart of the six Twin dimensions" width="100%"></td>
<td width="45%" valign="middle">

| Dimension | Answers |
|:--|:--|
| 🎚️ **Proficiency** | How good is the person at it? |
| 🧩 **Context** | Where and how was it used? |
| 📎 **Evidence** | What proves it? |
| 🔒 **Confidence** | How sure are we? |
| ⏱️ **Recency** | How fresh is the skill? |
| 🦅 **Autonomy** | Can they do it independently? |

</td>
</tr>
</table>

<p align="center"><img src="assets/diagrams/capability_loop.png" alt="Closed loop: evidence to Capability Twin to skill gap to practical task to evaluation to verified evidence and back to the Twin" width="90%"></p>

New work becomes new evidence, the Twin updates, and future matching improves.

```mermaid
stateDiagram-v2
  [*] --> Claimed: Résumé or self-declared
  Claimed --> Inferred: Capability Translator
  Inferred --> Evidenced: Project, repo or work sample
  Evidenced --> Verified: Practical task + evaluation
  Verified --> Verified: Recency refresh
  Verified --> Matched: Opportunity match
  Matched --> [*]: Human decision
```

### One platform, four stakeholders

```mermaid
flowchart TB
  T((🧬 Shared<br/>Capability Record))
  S[🎓 Candidate] <--> T
  E[🏢 Employer] <--> T
  I[🏛️ Institution / TPO] <--> T
  F[👨‍🏫 Faculty] <--> T
  T --> AI[🤖 AI agents + ML models]
  AI --> H[🧑‍⚖️ Human review]
  style T fill:#2354d6,color:#fff
  style H fill:#0f9d8a,color:#fff
```

---

## ✨ Features

> Status legend: ✅ working in the deployed prototype · 🧪 prototype / partial · 🗺️ planned. See [Project status](#-project-status).

### 🎓 Candidate

| | Feature | What it does | Status |
|:-:|:--|:--|:-:|
| 🪪 | **3D holographic identity card** | Spring-tilt physics, specular glare, capability-confidence ring, verification watermark | ✅ |
| 📈 | **Capability matrix & readiness score** | Verified skills (0–100%) and a composite career-readiness score | ✅ |
| 🏅 | **Peer benchmarking** | College and branch percentile ranking | ✅ |
| 🔁 | **Skill gap → learn → opportunity loop** | Finds the two weakest skills with 1-click *Learn*, *Assess*, *Roles* | ✅ |
| 🧭 | **AI learning pathways** | Milestone-based curriculum from Gemini, linked to docs, videos and repos | ✅ |
| 📝 | **Resume Studio** | ATS score, job-tailored resume, and a **no-fabrication engine** limited to verified projects | ✅ |
| 🛣️ | **Career roadmap** | Role-transition simulation with exact missing requirements | ✅ |
| 🌍 | **Portfolio & public profile** | GitHub telemetry sync, shareable `/u/:username`, QR-linked certificates | ✅ |
| 🎙️ | **AI voice mock interview** | Speech-to-speech via Vapi + Gemini, with clarity, confidence and filler-word analytics | ✅ |
| 💻 | **Coding IDE, aptitude, case-study & GD arena** | Monaco editor, Piston/Judge0 runner, timed aptitude with history | 🧪 |
| ✉️ | **MailIQ outreach** | Personalised recruiter cold emails with subject-line optimisation | 🧪 |

### 🏢 Employer

| | Feature | What it does | Status |
|:-:|:--|:--|:-:|
| 📡 | **Talent Radar** | Search by verified skill and minimum score (e.g. React ≥ 85%), not keywords | ✅ |
| ⚔️ | **Candidate comparison** | Side-by-side radar-chart comparison | 🧪 |
| 📌 | **Role posting & match matrix** | Post roles and auto-match against enrolled students | ✅ |
| 🗂️ | **Pipeline (ATS)** | Applied → Shortlisted → Round 1 → Technical → Offer → Hired | ✅ |
| 📅 | **Interview scheduler & offer letters** | Slot coordination, invites, offer-letter generation | ✅ |

```mermaid
flowchart LR
  A([Applied]) --> B([Shortlisted]) --> C([Round 1]) --> D([Technical]) --> E([Offer]) --> F([Hired])
  style A fill:#e0e7ff,stroke:#2354d6
  style F fill:#0f9d8a,color:#fff,stroke:#0c1f3d
```

### 🏛️ Institution & Faculty

| | Feature | What it does | Status |
|:-:|:--|:--|:-:|
| 📊 | **Placement dashboard** | Enrolled, placed, placement %, average and highest CTC | ✅ |
| 📥 | **Bulk CSV invite & skill-matrix export** | Onboard cohorts and export skill data | ✅ |
| 🏛️ | **NAAC / NIRF reporting** | Criterion 5 tables with print/PDF export | ✅ |
| 👨‍🏫 | **Faculty dashboard & endorsements** | Cohort progress and institutional skill endorsements | ✅ |
| 🚧 | **Drive management admin, multi-channel comms, curriculum-gap analytics** | Eligibility rules, broadcasts, syllabus insights | 🗺️ |

### ♿ Inclusion & accessibility

| | Feature | What it does | Status |
|:-:|:--|:--|:-:|
| 🔤 | **Synapse UI** | One-tap OpenDyslexic typeface and high-contrast reading modes | ✅ |
| ⚖️ | **Bias-audit agent** | Flags skewed shortlists for human review | 🧪 |
| 🤝 | **Equity-nudge & job-fairness agents** | Proactive fairness checks across the funnel | 🗺️ |

---

## 🤖 The AI engine

```mermaid
flowchart LR
  subgraph Browser
    UI[Next.js UI]
  end
  subgraph Server["Next.js server routes"]
    GW[AI gateway<br/>key rotation + failover]
    R1[translate-capability]
    R2[learning-pathway]
    R3[opportunity-match]
    R4[bias-audit]
  end
  subgraph ML["FastAPI ML service"]
    M[all-mpnet-base-v2<br/>fine-tuned, 469 capabilities]
    A[Predictive sklearn models]
  end
  UI --> GW --> R1 & R2 & R3 & R4
  R1 -.-> M
  UI --> A
  R1 & R2 & R3 & R4 --> G[(Google Gemini Flash)]
  style GW fill:#2354d6,color:#fff
  style M fill:#0f9d8a,color:#fff
```

### 🧠 Capability Translator (ML service)

A FastAPI service built on an `all-mpnet-base-v2` model fine-tuned on a **469-capability taxonomy**, with precomputed embeddings and an explainability breakdown for every inference.

| Method | Path | Purpose |
|:-:|:--|:--|
| `GET` | `/` | Service info |
| `GET` | `/health` | Health check |
| `GET` | `/capabilities` | List known capabilities |
| `POST` | `/infer-capabilities` | Infer capabilities from free text (`text`, optional `top_k` 1–20, default 8) |

```bash
curl -X POST http://localhost:8000/infer-capabilities \
  -H "Content-Type: application/json" \
  -d '{"text": "Led a volunteer team and built a budgeting spreadsheet", "top_k": 5}'
```

```mermaid
sequenceDiagram
  autonumber
  participant U as Candidate
  participant W as Next.js app
  participant ML as FastAPI Translator
  participant G as Gemini agent
  U->>W: Free-text experience
  W->>ML: POST /infer-capabilities
  ML-->>W: Top-k capabilities + explainability
  W->>G: Evidence + target role
  G-->>W: Gap analysis + learning pathway
  W-->>U: Capability Twin update
```

### 🎯 Gemini agent routes

| Route | Role |
|:--|:--|
| `translate-capability` | Turns raw evidence into capabilities |
| `learning-pathway` | Builds a milestone-based learning plan |
| `opportunity-match` | Matches a Twin to roles, with an evidence trail |
| `bias-audit` | Flags skewed shortlists for human review |

All routes run server-side, and each match carries an evidence trail.

### ⚡ Predictive engine (ArcLight models)

Scikit-learn re-implementation of enterprise SAS models over 12,000+ hiring records.

| Model | Predicts |
|:--|:--|
| 💰 **High-salary model** | Probability of a ≥ 15 LPA offer, with skill-boost levers |
| 📈 **Salary-hike predictor** | Appraisal and role-switch increments |
| 🧗 **Senior success potential** | Leadership and complex-delivery readiness |

Plus market-intelligence endpoints for top roles, salary distribution, skill demand and hiring hubs.

### 🔑 AI gateway

A server-side proxy with key rotation and automatic failover on rate limits. Keys never reach the browser.

---

## 🛡️ Proctoring & integrity

| Layer | Capability |
|:--|:--|
| 👁️ **Vision** | In-browser face detection via `@vladmandic/face-api`: multi-face, presence and gaze checks |
| 🔒 **Lockdown** | Fullscreen enforcement, tab-switch and window-blur counters, auto-termination at threshold |

---

## 🏗️ Architecture

<p align="center"><img src="assets/diagrams/architecture.png" alt="Layered system architecture: users, Next.js web app, AI and data services, inclusive-workforce layer, outputs" width="100%"></p>

Solid boxes exist in the repositories. Dashed boxes are planned.

| Layer | Technology | Source |
|:--|:--|:--|
| 🖥️ Web app | Next.js 16.3.1, React 19, TypeScript, Tailwind CSS 4, Framer Motion, Recharts, Zustand, lucide-react | `Access-Hire/package.json` |
| 🔌 Server API routes | `translate-capability`, `learning-pathway`, `opportunity-match`, `bias-audit` | `Access-Hire/app/api/agents/` |
| 🧠 ML inference | FastAPI, sentence-transformers, PyTorch 2.3.1 (CPU), scikit-learn, pandas | `accesshireml/requirements.txt`, `Dockerfile` |
| ✨ Generative agents | Google Gemini Flash | `Access-Hire/lib/gemini.ts` |
| 🔐 Authentication | Supabase | `Access-Hire/.env.example` |
| ♿ Accessibility | Synapse context (OpenDyslexic, high contrast) | `Access-Hire/lib/synapse-context.tsx` |
| ☁️ Deployment | Frontend on Vercel; ML service ships with a Dockerfile | live prototype, `accesshireml/Dockerfile` |

The deployed prototype also uses Firestore, a Vapi voice interview and Firebase email triggers; check its own code for those.

---

## 📏 Project status

> We would rather be exact than impressive.

<img src="assets/svg/status_bar.svg" alt="Stacked bar: 40 fully built, 13 partial, 84 not built of 137 audited features" width="100%">

```mermaid
pie showData title Deployed prototype: 137 audited features (audit dated 2026-09-25)
  "Fully built" : 40
  "Partial / new" : 13
  "Not built yet" : 84
```

<p align="center"><img src="assets/diagrams/feature_audit.png" alt="Stacked bar chart of fully built, partial and not-built features across nine areas, 40 of 137 fully built" width="90%"></p>

| Area | Working today |
|:--|:--|
| 🎓 Candidate career | AI career-path mapping, skill-gap analysis, personalised learning paths, QR-linked certificates, public profile, portfolio with GitHub sync, resume tailoring, ATS score |
| 🎙️ Interview prep | AI voice mock interview, session history and statistics, filler-word counter |
| 🏛️ Institution | Placement dashboard, bulk CSV invite, NAAC/NIRF report, faculty dashboard, skill-matrix export |
| 🏢 Employer | Role posting, candidate pipeline, offer-letter generation, interview scheduling |
| ⚙️ Platform | Role-based security rules, in-app notifications, dark mode |

**Not built yet:** equity-nudge and job-fairness agents, automated bias-audit reports in the deployed app, auto-scored practical tasks, WCAG compliance, mobile app.

---

## ⚙️ Run it locally

### 🖥️ Frontend

Requires Node.js 20+ and npm. Code is in [`frontend/`](frontend/).

```bash
cd frontend
npm install
cp .env.example .env.local
npm run dev   # http://localhost:3000
```

### 🧠 ML service

Code is in [`ml-service/`](ml-service/).

```bash
cd ml-service
pip install -r requirements.txt
# or: docker build -t accesshire-ml .
uvicorn app.main:app --host 0.0.0.0 --port 8000
```

### Environment variables

| Variable | Used for |
|:--|:--|
| `GOOGLE_GEMINI_API_KEY` | Server-side Gemini calls |
| `NEXT_PUBLIC_GEMINI_API_KEY` | Exposed to the browser. Avoid in production; use the server-side key |
| `NEXT_PUBLIC_SUPABASE_URL`, `NEXT_PUBLIC_SUPABASE_ANON_KEY` | Supabase authentication |
| `ACCESSHIRE_ML_API_URL` | URL of the running ML service |

Never commit real keys. Other scripts: `npm run build`, `npm run start`, `npm run lint`. The repository's `AGENTS.md` warns that Next.js 16 has breaking changes, so read `node_modules/next/dist/docs/` before framework-level changes.

---

## 🖼️ Gallery

These are illustrations, not screenshots. Add real screenshots in [`assets/screenshots/`](assets/screenshots/README.md).

<table>
  <tr>
    <td align="center"><img src="assets/illustrations/training.png" alt="Learners in a classroom facing a bar chart" width="320"><br><sub>Learning and upskilling</sub></td>
    <td align="center"><img src="assets/illustrations/placement-drive.png" alt="Students outside a campus building with a placement banner" width="320"><br><sub>Institutions and placements</sub></td>
  </tr>
  <tr>
    <td align="center"><img src="assets/illustrations/employer-verification.png" alt="Candidate and employer across a desk with a check mark" width="320"><br><sub>Verified capability</sub></td>
    <td align="center"><img src="assets/illustrations/impact-analytics.png" alt="Reviewer beside a screen with a rising line chart" width="320"><br><sub>Workforce insight</sub></td>
  </tr>
</table>

---

## 🗺️ Roadmap

```mermaid
timeline
  title CapAble roadmap
  Near term : Move Gemini key behind a backend
            : One clean end-to-end demo flow
  Next : Auto-generated and auto-scored practical tasks
       : Equity-nudge and job-fairness agents
       : Bias-audit reports in the deployed app
  Then : Institution drive-management admin UI
       : Job recommendations in opportunities
       : Employer funnel analytics
  Later : PWA and notifications
        : WCAG accessibility work
        : Multilingual support
        : Enterprise HR integrations
```

```mermaid
quadrantChart
  title Roadmap priority
  x-axis Low effort --> High effort
  y-axis Low impact --> High impact
  quadrant-1 Plan carefully
  quadrant-2 Do first
  quadrant-3 Fill gaps
  quadrant-4 Later
  Gemini key behind backend: [0.2, 0.9]
  Equity-nudge agents: [0.55, 0.8]
  Auto-scored tasks: [0.75, 0.9]
  Drive management UI: [0.5, 0.55]
  WCAG work: [0.7, 0.65]
  Multilingual support: [0.8, 0.45]
```

*Quadrant positions are rough planning estimates.*

---

## ⚖️ Responsible AI & privacy

| | Principle | In practice |
|:-:|:--|:--|
| 🧑‍⚖️ | **AI recommends, a human decides** | Match and bias-audit outputs are for human review |
| 🔎 | **Explainable by design** | Every capability carries evidence and an explanation |
| 🚫 | **No fabrication** | Resume generation is restricted to verified projects and capabilities |
| 🔐 | **Role-based security** | Rules protect data in the deployed prototype |
| 📝 | **No compliance claims** | Keep real personal data out of demos; share datasets only with permission |

---

## 👥 Contributors

| | Name | Role | Links |
|:-:|:--|:--|:--|
| <img src="assets/svg/team_deven.svg" width="120" alt="Deven"> | **Deven** | ML and research | [GitHub](https://github.com/Devengoyal885) · [LinkedIn](https://www.linkedin.com/in/deven-goyal) |
| <img src="assets/svg/team_aditya.svg" width="120" alt="Aditya Singh"> | **Aditya Singh** | Backend | [GitHub](https://github.com/aditya511-GH) · [LinkedIn](https://www.linkedin.com/in/adityas511) |
| <img src="assets/svg/team_rishabh.svg" width="120" alt="Rishabh Verma"> | **Rishabh Verma** | Frontend and backend | [GitHub](https://github.com/rishabhv16) · [LinkedIn](https://www.linkedin.com/in/rishabhverma1916) |
| <img src="assets/svg/team_divya.svg" width="120" alt="Divya Verma"> | **Divya Verma** | Testing | [GitHub](https://github.com/Divyav19) · [LinkedIn](https://www.linkedin.com/in/dviyaverma16) |

---

## 🔎 Topics

<details>
<summary><b>Topics this project covers</b></summary>

`capability-intelligence` · `skills-based-hiring` · `talent-operating-system` · `capability-twin` · `verified-skills` · `skill-gap-analysis` · `learning-pathways` · `explainable-ai` · `responsible-ai` · `bias-audit` · `fair-hiring` · `human-in-the-loop` · `resume-parser` · `ats` · `semantic-search` · `sentence-transformers` · `mpnet` · `nlp` · `fastapi` · `nextjs` · `react` · `typescript` · `tailwindcss` · `google-gemini` · `generative-ai` · `ai-agents` · `voice-ai` · `mock-interview` · `proctoring` · `placement-analytics` · `naac` · `nirf` · `edtech` · `hrtech` · `inclusive-hiring` · `accessibility` · `dyslexia`

</details>

## 🤝 Contributing

Read [CONTRIBUTING.md](CONTRIBUTING.md) and the [Code of Conduct](CODE_OF_CONDUCT.md). Issues and ideas are welcome. Open an issue first for larger changes, keep real keys out of commits, and keep the **human-in-the-loop** and **no-fabrication** principles intact.

## 📄 License

No license file has been added yet. Add one (for example MIT or Apache-2.0) before inviting outside contributions.

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&height=120&color=0:0f9d8a,50:2354d6,100:0c1f3d&section=footer" alt="footer" width="100%">
</p>
