# 🎯 CrewAI HiringScreener
**Multi-Agent AI Candidate Screening**

🌐 **[View Live Application](https://ai-hiring-screener.vercel.app/)**

> **Screen candidates in minutes, not days.** Paste a job description and candidate profile, and get a structured, fair, and actionable scorecard—powered by a crew of specialized AI agents. ⚡

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.11+-blue.svg)](https://www.python.org/downloads/)
[![Next.js](https://img.shields.io/badge/Next.js-15-black.svg)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-19.2-61DAFB.svg)](https://react.dev/)
[![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4.1-412991.svg)](https://openai.com/)
[![Railway](https://img.shields.io/badge/Deploy-Railway-blueviolet.svg)](https://railway.app/)

---

## ✨ What It Does

HiringScreener is an intelligent candidate screening platform that uses a **multi-agent AI crew** to evaluate candidates against job descriptions:

1. **RoleAnalyst** — Extracts job requirements, skills, and success criteria
2. **ProfileReader** — Analyzes candidate experience, achievements, and qualifications
3. **Evaluator** — Computes precise dimension scores using calibrated rubrics
4. **RiskChecker** — Identifies gaps, risks, and areas needing follow-up
5. **SummaryWriter** — Generates recruiter-ready summaries and interview questions

All in a single, beautiful interface with real-time progress visualization.

---

## 🎯 Core Features

### 🤖 **AI-Powered Screening**
- **Multi-Agent Crew** — 5 specialized AI agents work sequentially for thorough analysis
- **Precise Scoring** — Calibrated 0-100% scores for skills, experience, domain, and communication
- **Fair Evaluation** — Built-in bias detection and protected attribute filtering
- **Actionable Insights** — Specific strengths, gaps, and follow-up questions

### 📊 **Structured Scorecards**
- **Overall Match Score** — Weighted composite score with visual indicator
- **Dimension Scores** — Breakdown across 4 key areas with progress bars
- **Strengths & Gaps** — Evidence-based findings, not generic statements
- **Follow-up Questions** — Role-specific interview questions generated per candidate

### 🎨 **Modern Experience**
- **Single-Page App** — Smooth state-driven transitions, no page reloads
- **Dark/Light Mode** — Beautiful themes with system preference support
- **Mobile-First** — Responsive design with touch-optimized navigation
- **Real-time Progress** — Watch each AI agent work in real-time

### 📱 **Full Feature Set**
| Feature | Description |
|---------|-------------|
| 🎯 **Match Score** | Visual percentage showing candidate-job fit |
| 📈 **Dimension Scores** | Skills, Experience, Domain, Communication breakdown |
| ✅ **Strengths** | Evidence-based positive findings |
| ⚠️ **Gaps** | Specific areas where candidate may fall short |
| 💬 **Follow-ups** | Interview questions tailored to this candidate |
| 📝 **Summary** | Recruiter-ready paragraph with recommendation |
| 🛡️ **Fairness Note** | Confirmation of bias-free evaluation |
| 📊 **Analytics** | Track screening patterns over time |
| 📄 **PDF Export** | Professional branded reports |
| 📋 **Copy Results** | One-click clipboard sharing |
| 🔄 **History** | View and compare past screenings |
| ⚖️ **Compare Mode** | Side-by-side candidate comparison |
| 🎚️ **Custom Weights** | Adjust dimension importance per role |
| 📦 **Batch Screening** | Process multiple candidates at once |
| 🔗 **ATS Integration** | Connect to Supabase as ATS |
| ⌨️ **Keyboard Shortcuts** | Power user productivity |

---

## 🏗️ Tech Stack

### **Frontend** ⚛️
| Technology | Purpose |
|------------|---------|
| **Next.js 15** | React 19.2 with App Router |
| **TypeScript** | Type-safe development |
| **Tailwind CSS** | Utility-first styling |
| **shadcn/ui** | Beautiful component library |
| **Framer Motion** | Smooth animations |
| **Recharts** | Analytics visualizations |
| **next-themes** | Dark/light mode |

### **Backend** 🐍
| Technology | Purpose |
|------------|---------|
| **FastAPI** | High-performance Python API |
| **OpenAI GPT-4.1** | Multi-agent crew intelligence |
| **Pydantic v2** | Data validation |
| **Async/Await** | Non-blocking operations |

### **Data & Cache** 💾
| Technology | Purpose |
|------------|---------|
| **Supabase** | PostgreSQL persistence |
| **Upstash Redis** | Job queue & caching |

### **Deployment** 🚀
| Platform | Service |
|----------|---------|
| **Vercel** | Frontend hosting |
| **Railway** | Backend API |

---

## 🔄 How It Works

```
┌─────────────────────────────────────────────────────────────┐
│                      USER INPUT                             │
│         Job Description + Candidate Profile                 │
└─────────────────────┬───────────────────────────────────────┘
                      │
                      ▼
┌─────────────────────────────────────────────────────────────┐
│                 AI CREW WORKFLOW                            │
│                                                             │
│  ┌──────────────┐    ┌──────────────┐    ┌──────────────┐  │
│  │  RoleAnalyst │ ─▶ │ProfileReader │ ─▶ │  Evaluator   │  │
│  │  (Extract    │    │  (Extract    │    │  (Score &    │  │
│  │   Job Reqs)  │    │   Skills)    │    │   Compare)   │  │
│  └──────────────┘    └──────────────┘    └──────┬───────┘  │
│                                                  │          │
│  ┌──────────────┐    ┌──────────────┐           │          │
│  │SummaryWriter │ ◀─ │ RiskChecker  │ ◀─────────┘          │
│  │  (Generate   │    │  (Identify   │                      │
│  │   Summary)   │    │    Gaps)     │                      │
│  └──────────────┘    └──────────────┘                      │
└─────────────────────────────┬───────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│                    STRUCTURED OUTPUT                        │
│                                                             │
│  • Overall Match Score (0-100%)                             │
│  • Dimension Scores (Skills, Experience, Domain, Comms)     │
│  • Strengths (3-5 evidence-based findings)                  │
│  • Gaps (2-4 specific improvement areas)                    │
│  • Follow-up Questions (3-5 interview questions)            │
│  • Summary (Recruiter-ready recommendation)                 │
│  • Fairness Note (Bias-free confirmation)                   │
└─────────────────────────────────────────────────────────────┘
```

---

## 📖 User Guide

### Getting Started

1. **Paste Job Description** — Copy the job posting requirements
2. **Paste Candidate Profile** — Resume, LinkedIn summary, or notes
3. **Click "Run Screening"** — Watch the AI agents analyze
4. **Review Scorecard** — Overall score, dimensions, strengths, gaps
5. **Export or Share** — PDF, clipboard, or email

### Understanding Your Results

| Section | What It Shows |
|---------|---------------|
| **Overall Score** | Weighted match percentage (0-100%) |
| **Skills** | Technical and soft skills alignment |
| **Experience** | Years and relevance of experience |
| **Domain** | Industry/sector knowledge match |
| **Communication** | Evidence of communication abilities |
| **Strengths** | Specific positive findings with evidence |
| **Gaps** | Areas where candidate may need development |
| **Follow-ups** | Questions to ask in the next interview |
| **Summary** | Recruiter-ready recommendation paragraph |

### Pro Tips

- **Be detailed** in job descriptions for better analysis
- **Include achievements** in candidate profiles with metrics
- **Use custom weights** for role-specific priorities
- **Compare candidates** to see relative strengths
- **Check history** to track screening patterns

---

## 🎨 Customization

### Theme Options
- ☀️ **Light Mode** — Clean, professional interface
- 🌙 **Dark Mode** — Easy on the eyes
- 🖥️ **System** — Follows OS preference

### Scoring Weights
Adjust dimension importance via the Weights panel:
- **Balanced** — Equal weight to all dimensions
- **Technical Role** — Skills 40%, Experience 30%, Domain 20%, Communication 10%
- **Senior Position** — Skills 25%, Experience 40%, Domain 20%, Communication 15%
- **Client-Facing** — Skills 20%, Experience 20%, Domain 20%, Communication 40%

---

## 🛡️ Security & Fairness

### Data Privacy
- ✅ No candidate data stored permanently (ephemeral processing)
- ✅ API rate limiting for abuse prevention
- ✅ CORS protection for API endpoints
- ✅ Environment variables for all secrets
- ✅ Input sanitization and validation

### Fairness Guardrails
- ✅ **No protected attributes** — Name, age, gender, race, ethnicity, nationality, location (unless job-relevant), photos are never considered
- ✅ **Evidence-based scoring** — All scores tied to job requirements
- ✅ **Fairness note** — Every screening confirms bias-free evaluation
- ✅ **Transparent reasoning** — Strengths and gaps cite specific evidence

---

## 👨‍💻 Creator

**Derril Filemon**

[![GitHub](https://img.shields.io/badge/GitHub-derril--tech-181717?style=flat&logo=github)](https://github.com/derril-tech)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin)](https://www.linkedin.com/in/derril-filemon-a31715319)

This project demonstrates proficiency in:
- 🤖 **AI/ML Integration** — Multi-agent systems, OpenAI GPT-4, prompt engineering
- ⚛️ **Modern React** — Next.js 15, React 19.2, App Router, Server Components
- 🐍 **Python Backend** — FastAPI, async/await, Pydantic validation
- 🎨 **UI/UX Design** — Responsive design, animations, accessibility, theming
- ☁️ **Cloud Architecture** — Supabase, Redis, Railway, Vercel
- 🔧 **DevOps** — Monorepo structure, CI/CD, environment management

---

## 🙏 Acknowledgments

- **[OpenAI](https://openai.com/)** — GPT-4.1 API powering the AI crew
- **[Supabase](https://supabase.com/)** — Database and authentication
- **[Upstash](https://upstash.com/)** — Redis caching and job queues
- **[Railway](https://railway.app/)** — Backend deployment
- **[Vercel](https://vercel.com/)** — Frontend hosting
- **[shadcn/ui](https://ui.shadcn.com/)** — Beautiful component library
- **[Framer Motion](https://www.framer.com/motion/)** — Smooth animations
- **[Recharts](https://recharts.org/)** — Analytics visualizations

---

## 📄 License

MIT License — see [LICENSE](LICENSE) for details.

---

<div align="center">


[Live Demo](https://ai-hiring-screener.vercel.app/) 

Made with ❤️ and ☕ by [Derril Filemon](https://github.com/derril-tech)

</div>
