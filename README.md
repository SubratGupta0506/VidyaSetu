<div align="center">
<img width="1200" height="475" alt="GHBanner" src="https://github.com/user-attachments/assets/0aa67016-6eaf-458a-adb2-6e31a0763ed6" />
</div>

# Run and deploy your AI Studio app

This contains everything you need to run your app locally.

View your app in AI Studio: https://ai.studio/apps/06682214-d7f6-456d-8606-f1e377173e66

## Run Locally

**Prerequisites:**  Node.js


1. Install dependencies:
   `npm install`
2. Set the `GEMINI_API_KEY` in [.env.local](.env.local) to your Gemini API key
3. Run the app:
   `npm run dev`

# 🎓 VidyaSetu — Scalable Platform for Multimedia Educational Content Using Cloud Infrastructure

![HTML](https://img.shields.io/badge/Frontend-HTML%2FCSS%2FJS-orange)
![Tailwind](https://img.shields.io/badge/Styling-TailwindCSS-38B2AC)
![Supabase](https://img.shields.io/badge/Backend-Supabase-3ECF8E)
![AWS S3](https://img.shields.io/badge/Cloud-AWS%20S3-FF9900)
![n8n](https://img.shields.io/badge/Automation-n8n-EA4B71)
![License](https://img.shields.io/badge/License-MIT-green)

> 🌐 **Live Platform:** [https://vidya-setu-kohl.vercel.app/]
> 

An internship project developed at **GITAM (Deemed to be University), Bengaluru** — a full-stack, AI-powered, cloud-based e-learning platform that delivers multimedia educational content to students using modern web technologies and cloud infrastructure.

---

## 📖 About the Project

**VidyaSetu** (meaning "Bridge of Knowledge") is a web-based educational platform designed to provide structured and multimedia-rich learning experiences. The platform integrates **video lectures, podcasts, AI-generated notes, and quizzes** in a single system, backed by **AWS S3 cloud storage** and **automated content generation pipelines**.

This project was developed as part of the internship program (INTN2333) at GITAM School of CSE, Bengaluru, from **January 2026 to April 2026**.

---

## 👥 Team Members

| Name | Registration No |
|---|---|
| Subrat Gupta | 2023001559 |
| K. Yuvan Sankar Raja Reddy | 2023001485 |
| V. Ghayini | 2023003292 |
| Rudraraju Himaja | 2023001137 |
| P. J. Siddharth | 2023001377 |
| Parla Chaithanya | 2023001912 |

**Guide:** Dr. Zameer Ahmed Adhoni, Assistant Professor, Department of AI&DS, GSCE, Bengaluru

---

## 🎯 Features

- 🔐 **Secure Authentication** — User registration, login, and session management via Supabase
- 📋 **Personalized Onboarding** — Questionnaire-based personalization for course recommendations
- 🎥 **Video Lectures** — High-quality educational videos stored and streamed from AWS S3
- 🎙️ **Podcast Learning** — AI-generated audio content for flexible, on-the-go learning
- 📝 **AI-Generated Notes** — Structured notes created using NotebookLM from video transcripts
- ❓ **Auto-Generated Quizzes** — AI-powered quizzes generated from video content via n8n workflows
- 🤖 **Vidya AI Assistant** — Real-time doubt-solving AI assistant for DBMS, OS, DSA, and Python
- 📊 **Student Dashboard** — Progress tracking, quiz scores, weekly activity, and learning analytics
- ☁️ **Cloud Storage** — All multimedia content stored and delivered via AWS S3
- ⚙️ **Automated Content Pipeline** — Fully automated content generation using n8n workflows

---

## 🛠️ Tech Stack

| Category | Technologies |
|---|---|
| **Frontend** | HTML, CSS, JavaScript, Tailwind CSS, Node.js, Stitch UI, Google AI Studio |
| **Backend** | Supabase (Backend-as-a-Service) |
| **Database** | Supabase (PostgreSQL) |
| **Cloud Platform** | Amazon Web Services — AWS S3 |
| **Automation** | n8n (Workflow Automation) |
| **AI Tools** | Lovable AI (Assistant), NotebookLM (Notes Generation), Google AI Studio |
| **APIs** | YouTube Data API |
| **Version Control** | Git, GitHub |

---

## 🏗️ System Architecture

```
User (Browser)
      ↓
Frontend (HTML + Tailwind CSS + Node.js + Stitch UI)
      ↓
Backend (Supabase — Auth + Database + API)
      ↓                          ↓
AWS S3 Cloud Storage      n8n Automation Workflow
(Videos, Podcasts, PDFs)  (YouTube → Transcript → Quiz/Notes/Podcast)
      ↓                          ↓
         Content Delivered to User
                  ↓
      AI Assistant (Lovable AI / Vidya AI)
```

---

## ⚙️ How the Automated Content Pipeline Works

```
📥 Input Topic or YouTube Link
        ↓
🔍 YouTube Data API fetches multiple videos
        ↓
📊 Videos evaluated by views, likes, engagement score
        ↓
✅ Best video selected
        ↓
📜 Transcript extracted and cleaned (JavaScript in n8n)
        ↓
    ┌───────────────────────────────┐
    │                               │
❓ Quizzes generated via AI   📝 Notes via NotebookLM
                                    │
                               🎙️ Podcast audio created
    └───────────────────────────────┘
        ↓
☁️ All content stored in AWS S3
        ↓
🌐 Delivered to users via Platform
```

---

## 📁 AWS S3 Storage Structure

```
my-videos-platform/
├── Data Structures/
│   ├── videos/          ← MP4 video lectures
│   ├── podcast/         ← MP3 audio podcasts
│   └── notes/           ← PDF structured notes
├── DBMS/
│   ├── videos/
│   ├── podcast/
│   └── notes/
└── Python/
    ├── videos/
    ├── podcast/
    └── notes/
```

---

## 🖥️ Platform Interfaces

| Interface | Description |
|---|---|
| **Login Page** | Secure sign-in with email/password, forgot password support |
| **Signup Page** | Account creation with full name, email, password confirmation |
| **Home Page** | Course overview, platform features, team section |
| **Course Learning** | Video + Notes + Quiz + Podcast in a single integrated dashboard |
| **Student Dashboard** | Progress tracking, quiz accuracy, weekly activity charts |
| **Vidya AI** | Real-time AI doubt-solving assistant for DBMS, OS, DSA, Python |

---

## 👤 User Journey

```
1️⃣  Register / Login
2️⃣  Complete Onboarding Questionnaire
3️⃣  Get Personalized Course Recommendations
4️⃣  Select Course (Python / Data Structures / DBMS)
5️⃣  Watch Video Lectures
6️⃣  Listen to Podcasts
7️⃣  Read AI-Generated Notes
8️⃣  Attempt Quizzes
9️⃣  Ask Vidya AI for Doubt Resolution
🔟  Track Progress on Dashboard
```

---

## 🚀 Running the Project Locally

### Prerequisites
- Node.js installed
- Supabase account (for backend)
- AWS S3 bucket (for storage)
- n8n instance (for automation)

### Steps

```bash
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/VidyaSetu.git
cd VidyaSetu

# 2. Install dependencies
npm install

# 3. Set up environment variables
# Create a .env file with your Supabase and AWS credentials:
# SUPABASE_URL=your_supabase_url
# SUPABASE_ANON_KEY=your_supabase_key
# AWS_BUCKET_NAME=your_s3_bucket

# 4. Run the development server
npm start
```

---

## ⚠️ Current Limitations & Honest Disclaimer

- The **Vidya AI assistant** is partially trained and currently handles basic academic queries. Full training and fine-tuning is planned for future versions.
- The platform currently covers **3 subjects**: Python, Data Structures, and DBMS.
- Content is generated and stored manually/semi-automatically via the n8n pipeline.

---

## 🔮 Future Scope

- [ ] Full training and fine-tuning of Vidya AI for accurate, context-aware responses
- [ ] Case Study Learning Section with research paper summaries
- [ ] Expand to more courses — AI/ML, Cloud Computing, Cybersecurity, and non-tech subjects
- [ ] AI-powered personalized course recommendation system
- [ ] Mobile application development (iOS & Android)
- [ ] Collaborative features — discussion forums, peer interaction
- [ ] Gamification — badges, achievements, leaderboards
- [ ] Multilingual content support

---

## 📄 Project Report

This project was submitted as an Internship Report for the partial fulfilment of the degree of **Bachelor of Technology in Computer Science and Engineering** at GITAM (Deemed to be University), Bengaluru, 2026.

**Internship Code:** INTN2333
**Duration:** January 2026 — April 2026

---

## 🏛️ Acknowledgements

- **Director Prof. Y. Vamsidhar** — for providing the opportunity to undertake this project
- **Dr. Smita Sandeep Darandale**, HOD, Department of CSE, GITAM Bengaluru
- **Dr. Zameer Ahmed Adhoni**, Assistant Professor — for guidance and support throughout
- **GITAM School of CSE** — for the resources and infrastructure
- **AWS, Supabase, n8n, NotebookLM, Lovable AI** — for the powerful tools and services

---

## 📄 License

This project is licensed under the **MIT License** — free to use, modify, and distribute!

---

⭐ **If you find this project useful or interesting, please give it a star!** ⭐
