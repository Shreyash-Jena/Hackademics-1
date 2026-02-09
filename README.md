<div align="center">

# Hackademics — AI-Powered Career Intelligence Platform

**Bridging the gap between talent and opportunity through intelligent diagnostics, personalized upskilling, and AI-driven career guidance.**

[![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Django](https://img.shields.io/badge/Django-5.2-092E20?logo=django&logoColor=white)](https://www.djangoproject.com/)
[![Gemini AI](https://img.shields.io/badge/Google%20Gemini-AI%20Powered-4285F4?logo=google&logoColor=white)](https://ai.google.dev/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-3.x-06B6D4?logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

</div>

---

## Table of Contents

- [Vision](#vision)
- [Problem Statement](#problem-statement)
- [Our Solution](#our-solution)
- [Key Features](#key-features)
  - [AI-Powered Competency Assessment](#1-ai-powered-competency-assessment)
  - [Intelligent Resume Builder](#2-intelligent-resume-builder)
  - [Smart Skill Extraction & Analysis](#3-smart-skill-extraction--analysis)
  - [Personalized Job Recommendations](#4-personalized-job-recommendations)
  - [Adaptive Learning Roadmaps](#5-adaptive-learning-roadmaps)
  - [Performance Analytics Dashboard](#6-performance-analytics-dashboard)
- [Architecture Overview](#architecture-overview)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Module Deep Dive](#module-deep-dive)
- [API Integrations](#api-integrations)
- [Team](#team)

---

## Vision

The modern job market moves at an unprecedented pace. New technologies emerge, roles evolve, and the skills required to stay competitive shift constantly. Yet, candidates are often left navigating this landscape alone — armed with generic job boards that offer no real insight into their readiness, their gaps, or a clear path forward.

**Hackademics envisions a world where every candidate — regardless of background — has access to an intelligent career companion** that understands their unique skill profile, honestly evaluates their competencies, recommends the right opportunities, and builds a concrete roadmap to get them where they want to be.

We are not building just another job portal. We are building a **Career Intelligence Platform** — a unified ecosystem where diagnostics, learning, and employment converge, all powered by the latest advances in Generative AI.

---

## Problem Statement

> **ED01 — AI-Powered Employment Portal** *(Education Domain)*

Current employment platforms suffer from critical shortcomings:

| Challenge | Impact |
|---|---|
| **No personalized diagnostics** | Candidates apply blindly without understanding their readiness for a role |
| **No adaptive learning** | Generic courses flood the market but none are tailored to individual skill gaps |
| **Disconnected workflows** | Resumes, skill assessments, job searches, and upskilling exist on separate platforms |
| **No AI-driven feedback** | Subjective answers go unevaluated; candidates receive no actionable feedback |
| **Static resumes** | Resumes don't evolve with the candidate's growing skill set |

There is a pressing need for an **intelligent, unified system** that evaluates user competencies, recommends matching jobs, suggests targeted learning paths to address skill gaps, and streamlines professional presentation — all in one place.

---

## Our Solution

Hackademics is a **full-stack AI-powered employment portal** that acts as a one-stop career intelligence platform combining:

- **Competency Diagnostics** — AI-generated role-specific assessments with real-time answer evaluation
- **Adaptive Learning** — Personalized upskilling roadmaps generated from the candidate's actual skill profile
- **Resume Intelligence** — AI-enhanced resume generation with multiple professional templates
- **Job Matching** — Live job recommendations powered by skill extraction and market data
- **Performance Analytics** — Visual dashboards tracking competency growth over time

All AI capabilities are powered by **Google Gemini (Generative AI)**, enabling natural language question generation, subjective answer evaluation, skill extraction, resume enhancement, and learning path creation.

---

## Key Features

### 1. AI-Powered Competency Assessment

The heart of Hackademics. The platform generates **role-specific subjective questions** using Gemini AI, tailored to whatever job role the user selects.

- **Dynamic Question Generation** — Enter any job role (e.g., "Machine Learning Engineer," "Full Stack Developer") and the AI generates technically rigorous, relevant competency questions on the fly.
- **AI Answer Evaluation** — Unlike MCQ-based platforms, Hackademics evaluates **free-form, subjective answers** using Gemini. Each answer is scored on a 0–1 scale for correctness.
- **Session-Based Testing** — Each test is tracked as a session with individual answers stored, enabling detailed review and historical comparison.
- **Difficulty Awareness** — Questions are generated with Easy, Medium, and Hard difficulty classifications.

### 2. Intelligent Resume Builder

Hackademics doesn't just store your resume — it **enhances** it.

- **AI-Enhanced Content** — Projects and achievements are automatically polished by Gemini AI to be concise, impactful, and resume-worthy using strong action verbs and professional language.
- **Multiple Professional Templates** — Choose from three curated templates:
  - `Professional` — Clean, corporate-ready layout
  - `Creative` — Modern design with visual flair
  - `Minimalistic` — Elegant, distraction-free format
- **DOCX Export** — Download your enhanced resume as a fully formatted Word document, ready for submission.
- **Resume History** — View, manage, and delete previously generated resumes. Each version is timestamped and stored.

### 3. Smart Skill Extraction & Analysis

The platform reads your complete professional profile and uses AI to **extract a structured list of technical and soft skills**.

- **Profile-Aware Extraction** — Analyzes education, experience, projects, achievements, and declared skills to build a comprehensive skill inventory.
- **Stored Skill Profiles** — Extracted skills are persisted in the user profile as structured JSON, enabling downstream features like job matching and roadmap generation.
- **Dual AI Engines** — Supports both Google Gemini (cloud) and Ollama/Mistral (local) for skill extraction, providing flexibility in deployment.

### 4. Personalized Job Recommendations

Hackademics connects extracted skills with **real-world job market data** to surface the most relevant opportunities.

- **Live Job Search** — Integrates with the **Jooble API** to fetch real-time job listings based on AI-refined search keywords.
- **AI-Curated Matching** — Gemini refines raw skills into optimal search keywords, and results are filtered by location and relevance.
- **Remote Job Matching** — Queries the **Remotive API** for remote opportunities, with AI-powered ranking that explains *why* each job is a good fit.
- **Match Explanations** — Each recommended job comes with a human-readable reason for the match (e.g., "Strong match with backend Python skills and database experience").

### 5. Adaptive Learning Roadmaps

Once skills and target roles are identified, the platform generates **personalized, week-by-week learning roadmaps**.

- **Gap Analysis** — AI compares the user's current skills against the requirements of their target role and identifies exactly what's missing.
- **Structured Roadmap** — A detailed 3–4 month learning plan broken into actionable steps with recommended resources (documentation, courses, articles).
- **Interactive Checklist** — Roadmaps are parsed into structured JSON steps with completion tracking, enabling users to check off progress.
- **Resume-Informed** — Roadmaps are generated from the user's latest resume data, ensuring recommendations are grounded in reality.

### 6. Performance Analytics Dashboard

Track your career growth with **visual analytics**.

- **Test History** — Review all past competency test sessions with scores, dates, and job roles.
- **Accuracy Graphs** — Chart.js-powered visualizations showing performance trends, accuracy rates, and correct/incorrect breakdowns across sessions.
- **Aggregate Statistics** — Overall accuracy, total questions attempted, and performance summaries at a glance.

---

## Architecture Overview

```
┌─────────────────────────────────────────────────────────────────┐
│                        CLIENT (Browser)                        │
│              Tailwind CSS · Chart.js · Django Templates         │
└──────────────────────────────┬──────────────────────────────────┘
                               │
┌──────────────────────────────▼──────────────────────────────────┐
│                      DJANGO APPLICATION                         │
│                                                                 │
│  ┌──────────┐  ┌──────────────┐  ┌─────────────┐  ┌─────────┐ │
│  │  Users    │  │  Competency  │  │Recommendations│  │ Resume  │ │
│  │  Module   │  │   Module     │  │   Module     │  │ Builder │ │
│  └────┬─────┘  └──────┬───────┘  └──────┬───────┘  └────┬────┘ │
│       │               │                 │                │      │
│  ┌────▼───────────────▼─────────────────▼────────────────▼────┐ │
│  │                    SHARED DATA LAYER                        │ │
│  │               SQLite · Django ORM · Models                  │ │
│  └─────────────────────────┬──────────────────────────────────┘ │
└────────────────────────────┼────────────────────────────────────┘
                             │
┌────────────────────────────▼────────────────────────────────────┐
│                      EXTERNAL SERVICES                          │
│                                                                 │
│  ┌───────────────┐  ┌────────────┐  ┌───────────────────────┐  │
│  │  Google Gemini │  │  Jooble API │  │  Remotive API         │  │
│  │  (Gen AI)      │  │  (Jobs)     │  │  (Remote Jobs)        │  │
│  └───────────────┘  └────────────┘  └───────────────────────┘  │
│                                                                 │
│  ┌───────────────┐                                              │
│  │  Ollama/Mistral│ (Optional — Local AI)                       │
│  └───────────────┘                                              │
└─────────────────────────────────────────────────────────────────┘
```

---

## Tech Stack

| Layer | Technology |
|---|---|
| **Backend Framework** | Django 5.2 (Python) |
| **AI / LLM** | Google Gemini 2.5 Flash (Primary), Ollama + Mistral (Optional Local) |
| **Frontend** | Django Templates, Tailwind CSS, Chart.js |
| **Database** | SQLite (Development) |
| **Job APIs** | Jooble REST API, Remotive REST API |
| **Document Generation** | python-docx (DOCX export) |
| **Authentication** | Django Auth (Custom User Model) |

---

## Project Structure

```
Hackademics/
├── config/                     # Django project configuration
│   ├── settings.py             # Project settings & installed apps
│   ├── urls.py                 # Root URL routing
│   └── wsgi.py / asgi.py       # Server entry points
│
├── users/                      # User management module
│   ├── models.py               # Custom User & UserProfile models
│   ├── views.py                # Register, Login, Dashboard, Profile CRUD
│   ├── forms.py                # Custom user & profile forms
│   └── urls.py                 # Auth & profile routes
│
├── competency/                 # AI competency assessment module
│   ├── models.py               # Question, TestSession, Answer models
│   ├── views.py                # Test generation, question flow, results, analytics
│   ├── utils.py                # Gemini question generation & answer evaluation
│   └── urls.py                 # Assessment routes
│
├── recommendations/            # Job matching & learning roadmap module
│   ├── models.py               # JobRecommendation, LearningPath, Roadmap models
│   ├── views.py                # Skill extraction, job matching, roadmap generation
│   ├── utils.py                # Gemini roadmap generation, Jooble integration
│   ├── ollama_utils.py         # Local AI (Ollama/Mistral) skill extraction
│   └── urls.py                 # Recommendation routes
│
├── resume_builder/             # AI-enhanced resume module
│   ├── models.py               # Resume model
│   ├── views.py                # Resume generation, DOCX download, history
│   ├── utils.py                # Gemini content enhancement
│   └── urls.py                 # Resume routes
│
├── templates/                  # All HTML templates
│   ├── base.html               # Master layout (dark theme, navigation)
│   ├── users/                  # Auth & profile templates
│   ├── competency/             # Assessment & analytics templates
│   ├── recommendations/        # Job matching & roadmap templates
│   └── resume_templates/       # Resume preview & template variants
│
├── manage.py                   # Django management CLI
└── db.sqlite3                  # SQLite database
```

---

## Getting Started

### Prerequisites

- Python 3.10 or higher
- pip (Python package manager)
- Git
- A Google Gemini API key ([Get one here](https://ai.google.dev/))
- *(Optional)* Ollama installed locally for offline AI features

### Installation

```bash

# 2. Create and activate a virtual environment
python -m venv venv
# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate

# 3. Install dependencies
pip install django google-generativeai ollama python-docx xhtml2pdf requests djangorestframework pypandoc

# 4. Apply database migrations
python manage.py migrate

# 5. Create a superuser (optional, for admin access)
python manage.py createsuperuser

# 6. Start the development server
python manage.py runserver
```

### Configuration

1. **Gemini API Key** — Replace the API key placeholders in the following files with your own key:
   - `competency/utils.py`
   - `recommendations/utils.py`
   - `recommendations/views.py`
   - `resume_builder/utils.py`

2. **Jooble API Key** — Replace the Jooble API key in `recommendations/utils.py` with your own key from [Jooble](https://jooble.org/api/about).

3. Visit `http://127.0.0.1:8000/` to access the platform.

---

## Module Deep Dive

### Users Module (`/users`)

The foundation of the platform. Manages authentication, user profiles, and the central data store that feeds all other modules.

| Endpoint | Description |
|---|---|
| `/register/` | New user registration |
| `/login/` | User authentication |
| `/logout/` | Session termination |
| `/` | Main dashboard |
| `/profile/edit/` | Create or update professional profile |
| `/profile/` | View profile summary |

The `UserProfile` model stores comprehensive career data: full name, contact details, location, skills, education, experience, projects, achievements, preferred resume template, and AI-extracted skills (JSON).

### Competency Module (`/competency`)

Delivers the AI-driven assessment engine.

| Endpoint | Description |
|---|---|
| `/competency/generate/` | Generate questions for a job role |
| `/competency/questions/<role>/` | View generated questions |
| `/competency/test/start/<role>/` | Begin a timed test session |
| `/competency/test/<id>/question/<id>/` | Answer individual questions |
| `/competency/test/<id>/result/` | View test results and scores |
| `/competency/test/history/` | Browse all past test sessions |
| `/competency/test/historygraph/` | Visual performance analytics |

### Recommendations Module (`/recommendations`)

Powers job discovery and personalized learning.

| Endpoint | Description |
|---|---|
| `/recommendations/extract-skills/` | AI skill extraction from profile |
| `/recommendations/match-live-jobs/` | Match skills to remote job listings |
| `/recommendations/job-recommendation/` | Fetch live job recommendations |
| `/recommendations/targetjob/` | Set target job role for roadmap |
| `/recommendations/roadmap/<target>/` | Generate personalized learning roadmap |

### Resume Builder Module (`/resume`)

Handles AI-enhanced resume creation and management.

| Endpoint | Description |
|---|---|
| `/resume/generate/` | Generate AI-enhanced resume |
| `/resume/download/` | Download resume as DOCX |
| `/resume/view-resume/` | View all saved resumes |
| `/resume/resume-details/<id>/` | View a specific resume with template |
| `/resume/delete-resume/<id>/` | Delete a saved resume |

---

## API Integrations

| Service | Purpose | Type |
|---|---|---|
| **Google Gemini 2.5 Flash** | Question generation, answer evaluation, skill extraction, resume enhancement, roadmap creation | Generative AI |
| **Jooble API** | Real-time job listings by keywords and location | REST API |
| **Remotive API** | Remote job listings for skill-based matching | REST API |
| **Ollama (Mistral)** | Local/offline skill extraction and job matching | Local LLM |

---



**Domain:** Education  
**Problem Statement:** ED01 — AI-Powered Employment Portal

---

<div align="center">

*Built with purpose. Powered by AI. Designed for your career.*

**Hackademics** © 2026

</div>
