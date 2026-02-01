# AI-Powered Project & Productivity Platform

[![Tech Stack](https://img.shields.io/badge/Tech-Next.js%20|%20Node.js%20|%20PostgreSQL%20|%20AWS-blue)](https://github.com/vinitavictushvi/AI-Powered-Project-Productivity-Platform)

A **full-stack, enterprise-ready project and productivity management platform powered by AI-driven analytics**. This platform helps teams plan projects, manage tasks, predict delays, and gain actionable productivity insights using modern web technologies, cloud infrastructure, and machine learning.

---

## Table of Contents
- [Project Overview](#project-overview)  
- [Tech Stack](#tech-stack)  
- [Core Features](#core-features)  
- [Architecture & Workflow](#architecture--workflow)  
- [Installation & Setup](#installation--setup)  
- [Usage](#usage)  
- [Portfolio Value](#portfolio-value)  
- [Future Enhancements](#future-enhancements)  

---

## Project Overview

**Project Name:** AI-Powered Project & Productivity Platform  

**Purpose:**  
A scalable full-stack platform designed for teams and organizations to efficiently manage projects and tasks. The system leverages AI to predict task delays, suggest task prioritization, and analyze team productivity—demonstrating **real-world, enterprise-level development skills**.

This project highlights expertise in **Next.js, Node.js, AWS, PostgreSQL, and AI/ML integration**.

---

## Tech Stack

**Frontend**
- **Next.js** – Modern React framework with SSR/SSG  
- **Tailwind CSS** – Utility-first responsive UI design  
- **Charts.js / Recharts** – Interactive dashboards & analytics  

**Backend**
- **Node.js + Express.js** – REST APIs for modular, scalable architecture  

**Database**
- **PostgreSQL (AWS RDS)** – Structured relational database for users, projects, and tasks  

**Authentication**
- **AWS Cognito** – Enterprise-ready authentication with role-based access control (Admin / Manager / Developer)  

**Cloud & Deployment**
- **AWS EC2** – Backend deployment  
- **AWS S3** – Static assets & reports  
- **AWS CloudFront** – CDN for fast content delivery  

**AI / Analytics**
- **Python (sklearn / lightweight transformers)**  
  - Task delay prediction  
  - Task prioritization suggestions  
  - Sentiment analysis on comments/feedback  

---

## Core Features

### 1️⃣ User & Role Management
- **Roles:** Admin, Manager, Developer  
- **Capabilities:**  
  - **Admin:** Full access to users, projects, and tasks  
  - **Manager:** Assign tasks, monitor team performance  
  - **Developer:** Update task progress, add comments  
- **Implementation:**  
  - AWS Cognito authentication & MFA  
  - Role-based access control (RBAC)  
  - Conditional UI rendering based on role  

**Portfolio Value:** Enterprise-grade security and access control  

---

### 2️⃣ Projects & Tasks CRUD
- Create, read, update, delete projects and tasks  
- Assign tasks to developers  
- Track task status: Todo / In Progress / Completed  

**Implementation:**  
- REST API endpoints: `/projects`, `/tasks`  
- PostgreSQL relational schema  
- Optional Kanban-style task board  

**Portfolio Value:** Real-world project management logic with full CRUD  

---

### 3️⃣ AI-Powered Insights
- **Predict delayed tasks** using ML  
- **Suggest task prioritization**  
- **Sentiment analysis** on comments/feedback  

**AI Workflow:**  
1. Collect task data (deadlines, progress, dependencies)  
2. Run ML model to calculate delay probability  
3. Send predictions to frontend for visualization  

**Frontend Indicators:**  
- 🔴 High-risk tasks  
- 🟠 Medium-risk tasks  
- 🟢 Healthy tasks  

**Portfolio Value:** Strong AI + full-stack integration (high interview wow factor)  

---

### 4️⃣ Dashboard & Analytics
- KPIs: Completion %, overdue tasks, productivity score  
- Visual analytics using bar, line, and pie charts  
- Team & project performance tracking  

**Implementation:**  
- Next.js + Tailwind CSS  
- Charts.js / Recharts  
- Aggregated data via REST APIs  

**Portfolio Value:** Professional data visualization & analytics skills  

---

### 5️⃣ Notifications
- **Email reminders** for upcoming deadlines  
- **Alerts** for delayed or high-risk tasks  

**Implementation:**  
- AWS SES for email notifications  
- Cron jobs / AWS Lambda for scheduling  

**Portfolio Value:** Production-ready notification system with cloud services  

---

### 6️⃣ Realtime Updates (Optional)
- Live task updates and comments  
- Auto-refresh dashboards without page reload  

**Implementation:**  
- WebSocket / Socket.io  
- Frontend subscribes to live events  

---

## Architecture & Workflow

```text
Frontend (Next.js + Tailwind)  <-->  REST APIs (Node.js + Express)  <-->  PostgreSQL (AWS RDS)
                                   |                          
                                   v                          
                           AI Services (Python / ML)          
                                   |                          
                                   v                          
                             Notifications (AWS SES + Lambda)
