# 🛫 Personal Flight Logging App

This is a personal flight logbook application designed for private pilots to **record**, **manage**, and **track** their flight history and aircraft usage with ease. Built with modern web technologies and a CI/CD-first mindset, this project also serves as a **DevOps showcase**, demonstrating production-ready automation and cloud deployment pipelines.

---

## ✈️ Features

- 📘 **Flight Logging**: Store detailed records of each flight including date, aircraft, duration, and notes.
- 🛩️ **Aircraft Management**: Track different planes used for flights.
- 🧾 **Flight History**: Filter and view past flights with a user-friendly interface.
- 📦 **CI/CD Automation**: GitHub Actions pipeline for build, test, coverage, Dockerization, and deployment.

---

## 🧱 Tech Stack

| Layer     | Technology        |
|-----------|-------------------|
| Backend   | [FastAPI](https://fastapi.tiangolo.com/) |
| Frontend  | [Svelte](https://svelte.dev/) + [shadcn-svelte](https://github.com/shadcn-ui/ui) |
| Database  | SQLite            |
| DevOps    | GitHub Actions + Docker + SonarCloud + Render |

---

## 🧪 GitHub Actions CI/CD Overview

This project includes a comprehensive CI/CD pipeline for the **backend** and **frontend**, triggered on pushes to `develop` and `production` branches.

### ✅ Workflow Includes:

- **Build** with dependency caching
- **Test** with `coverage`
- **SonarCloud** quality analysis
- **Docker** image build and push (dev/prod tags)
- **Deployment** to [Render](https://render.com/)
- **Pages** Deployed pages to giuthub pages

> 📘 _See full pipeline config in `.github/workflows/backend.yml` and `.github/workflows/frontend.yml`_

---

## 🚀 Getting Started

### Prerequisites

- Docker

### Backend Setup

```bash
git clone https://github.com/DavidBalazic/flight-logbook-devops.git
cd flight-logbook-devops/EvidencaLetenjaBackend
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python main.py
```

### Frontend Setup

```bash
cd frontend/flight-logbook-devops 
npm install 
npm run dev 
```
