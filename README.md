# 🧠 EarlyArc — AI-Enabled Multimodal Autism Screening & Care Platform

> **Tata Elxsi TELIPORT Season 3 · Case Study No. 4 · Round 2 Submission**  
> Team: **The Innovators** · Samiksha Mitra & Rupangkan Mazumdar · **IIT Guwahati**

---

## 🚀 Live Demo

**Hosted on Github Pages:** Open the `earlyarc/` live deployed site at [Github](https://samik123mit.github.io/EarlyArc/)  
**Run locally:** Just open `index.html` in any browser — no server, no install needed.

---

## 📋 What is EarlyArc?

EarlyArc is a cloud-based multimodal AI platform that transforms ASD (Autism Spectrum Disorder) screening from a 2.5-year specialist-gated diagnostic ordeal into a **weeks-long, objective, AI-assisted** early identification and adaptive care pathway.

**Core technology:** Computer Vision (CV) + EEG biosignals + Agentic AI fused via attention-based late fusion engine.

---

## 🖥️ Prototype Screens

### 1. 🏠 Landing Page
- Live animated EEG waveform (3 channels)
- Real-time updating risk metrics
- CV feature weight bars
- Tech stack overview

### 2. 🔬 Live Screening Demo (5-Step Flow)

| Step | Module | What it shows |
|------|--------|---------------|
| 1 | Patient Intake | Demographics form + developmental milestone checklist. Screening Agent auto-flags based on ≥3 concerns |
| 2 | CV Analysis | Animated face tracking + scan line + 6 real-time feature metric cards (gaze, affect, gesture, etc.) with color-coded risk levels |
| 3 | EEG Processing | Live 6-channel animated EEG waveform + power spectral density chart + δ θ α β band analysis cards + P300 ERP result |
| 4 | Fusion Engine | Processing animation overlay → attention fusion → **Risk Score 0.74** → SHAP feature contribution waterfall chart |
| 5 | Clinical Report | Full domain deficit profile, specialist referral recommendation, therapy module assignment (6 modules) |

### 3. 📊 Clinician Dashboard
- 5 KPI cards (patients, screenings, flags, AUC, sensitivity)
- Weekly screening volume bar chart (stacked by risk level)
- Risk score distribution histogram
- Live AI agent activity feed (all 4 agents)
- Patient priority queue with risk pills
- Therapy progress tracker with 4-week trend chart

### 4. ⚙️ Platform & Team
- Full technical architecture breakdown (Layers A–D)
- Tech stack tags
- Team profiles
- Clinical evidence base (6 cited papers)
- Deployment & regulatory pathway

---

## 🏗️ Platform Architecture

```
Layer A — Multimodal Ingestion
  ├── Video streams (RGB, 30fps)
  ├── EEG signals (8–32ch, 128–256Hz)
  ├── Behavioral forms (ADOS-2 adapted)
  └── Therapy session logs

Layer B — Feature Extraction
  ├── CV: CNN + LSTM/Transformer → 6 gaze/affect/gesture features
  └── EEG: ICA + STFT + DNN → δ θ α β bands + ERPs

Layer C — Fusion Engine
  ├── Attention-based late fusion (shared latent space)
  ├── Risk score [0–1] + 95% confidence interval
  └── SHAP feature contribution maps (XAI)

Layer D — Agentic AI (4 Autonomous Agents)
  ├── 01 Screening Agent       → threshold-based risk flagging
  ├── 02 Clinical Support      → diagnostic evidence synthesis
  ├── 03 Therapy Planning      → RL-inspired personalized plans
  └── 04 Progress Monitoring   → longitudinal outcome tracking
```

---

## 🔬 Clinical Evidence Base

| Finding | Source | Application |
|---------|--------|-------------|
| EEG θ/α abnormalities in 73% of ASD children 2–5y | Bosl et al., Neuron 2022 | EEG band power features |
| Eye gaze deviation detectable >85% accuracy via CNN | Wang, Nature DM 2023 | CV gaze stability feature |
| Multimodal fusion improves AUC by +12% | IEEE TBME 2023 | Core fusion engine rationale |
| Early Rx (<3yr) → 47% better outcomes | JAMA Pediatrics 2024 | Platform's screening target |
| RL therapy adaptation → 35% skill improvement | J. Child Psychology 2023 | Therapy Planning Agent |
| P300 latency prolonged +100ms avg in ASD | Brain & Cognition 2021 | ERP analysis module |

---

## 💻 Tech Stack

```
Frontend    React / Vanilla JS / Chart.js
CV Model    PyTorch · MediaPipe Holistic · CNN + LSTM
EEG         MNE-Python · ICA · STFT · DNN classifier
XAI         SHAP (SHapley Additive exPlanations)
Backend     FastAPI · PostgreSQL
Standards   FHIR R4 (EHR integration)
Security    AES-256 · DPDP Act 2023 · Consent-driven AA Framework
Deploy      Docker · Edge (Android, offline-capable) · Cloud
Regulatory  FDA De Novo · CE Mark Class IIb · CDSCO Class C
```

---

## 📁 File Structure

```
earlyarc/
└── index.html      ← entire prototype (single file, ~92KB)
└── README.md       ← this file
```

> The entire prototype is self-contained in one HTML file. No npm, no build step, no dependencies to install. Chart.js is loaded from CDN. Google Fonts are loaded from CDN.

---

## 🌐 Hosting Options

### Option 1 — Netlify Drop (Recommended, 2 min)
1. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag the entire `earlyarc/` **folder** (not just the file) onto the drop zone
3. Get a live URL instantly: `https://your-name-123.netlify.app`

> ⚠️ Must drop the **folder**, not the bare `.html` file. The file must be named `index.html`.

### Option 2 — GitHub Pages
```bash
git init
git add .
git commit -m "EarlyArc prototype"
gh repo create earlyarc --public --push --source=.
# Enable Pages in repo Settings → Pages → Deploy from branch: main
```

### Option 3 — Local
Just double-click `index.html` — works in Chrome, Firefox, Safari, Edge.

---

## 📊 Key Metrics

| Metric | Value |
|--------|-------|
| Target AUC | > 0.92 |
| Sensitivity (screening) | > 88% |
| Screening time | < 2 minutes |
| Inter-rater improvement | 40% ↑ vs ADOS alone |
| Therapy outcome delta | 35% ↑ vs standard care |
| Global ASD population | 75M+ |
| Market TAM by 2030 | $8.7B |
| CAGR | 22.4% |

---

## 👥 Team

**Samiksha Mitra** — B.Tech Civil Engineering, IIT Guwahati  
WorldQuant BRAIN Research Consultant · Multyfi Quant Researcher · NISM V-A Certified  
Overall Coordinator, 4i Labs (200+ members) · Top 20%, International Quant Championship

**Rupangkan Mazumdar** — B.Tech, IIT Guwahati  
Co-developer, EarlyArc Platform

---

*Tata Elxsi TELIPORT Season 3 · Case Study No. 4 · Team: The Innovators · IIT Guwahati · 2026*
