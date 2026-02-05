# 🛡️ EduGuard AI  
### An AI-Powered Student Risk Prediction & Support Platform

EduGuard AI is a **full-stack web application integrated with Machine Learning** that proactively identifies academically and mentally at-risk students and enables **early intervention** through predictive analytics, counseling insights, and intelligent alerts.

The platform empowers educational institutions to **reduce dropout rates**, **improve academic performance**, and **support student well-being** using data-driven decision-making.

---

## 📌 Problem Statement

Educational institutions often respond **too late** to student struggles due to:

- Limited visibility into student engagement patterns  
- Absence of early-warning and predictive systems  
- Manual and reactive monitoring of academic and behavioral data  

As a result, students at risk of dropping out or facing mental health challenges go unnoticed until it is too late.

**EduGuard AI solves this problem** by predicting risks early and enabling timely, targeted support.

---

## 🚀 Key Features

### 🔮 1. Student Dropout Risk Prediction
- Machine Learning–based classification system  
- Predicts dropout probability: **Low / Medium / High**  
- Uses features such as:
  - Attendance records  
  - Academic scores  
  - Fee payment status  
  - Engagement and behavioral metrics  

---

### 📊 2. Performance Forecasting & Analytics
- Predicts **future exam scores**  
- Subject-wise academic progress tracking  
- Visual dashboards for performance trends  
- Feature importance visualization for **model explainability**

---

### 🧠 3. AI Counseling & Sentiment Monitoring
- Sentiment analysis on student feedback and reflections  
- Emotion detection (stress, anxiety, motivation, disengagement)  
- Early **mental health risk indicators**  
- Counselor-oriented insights (non-diagnostic, assistive only)

---

### 🤖 4. Risk-Aware Academic Support Chatbot
- Context-aware academic chatbot for student support  
- Detects stress or negative sentiment during conversations  
- Automatically escalates **high-risk cases** to mentors or counselors  

---

### 🔔 5. Smart Alert System
- Unified risk scoring engine combining:
  - Academic risk  
  - Behavioral risk  
  - Emotional risk  
- Real-time dashboard alerts  
- Automated email notifications  
- Admin-controlled risk thresholds

---

## 🏗️ System Architecture

EduGuard AI is designed using a **modular and scalable architecture** where the frontend, backend, database, and machine learning services are clearly separated and communicate through secure APIs.

### Architecture Flow Diagram

```
┌─────────────────────────────────────────────────────────────┐
│           Frontend (React + Tailwind CSS)                   │
│         (Web Dashboard & Admin Interface)                   │
└────────────────────┬────────────────────────────────────────┘
                     │ (REST API / WebSocket)
                     ↓
┌─────────────────────────────────────────────────────────────┐
│          Backend API (Node.js + Express)                    │
│         (Authentication, Business Logic)                    │
└────────────────────┬────────────────────────────────────────┘
                     │
        ┌────────────┼────────────┐
        ↓            ↓            ↓
┌──────────────┐ ┌───────────────────┐ ┌──────────────────┐
│   MongoDB    │ │ ML Service API    │ │  Cache (Redis)   │
│  Database    │ │ (FastAPI/Flask)   │ │   (Optional)     │
│  (Data)      │ │ (Predictions)     │ │                  │
└──────────────┘ └───────┬───────────┘ └──────────────────┘
                         │
                         ↓
        ┌────────────────────────────────────┐
        │  ML Models                         │
        │  • Dropout Prediction              │
        │  • Performance Forecasting         │
        │  • Sentiment Analysis              │
        │  • Intent Detection                │
        └────────────────────────────────────┘
```

### Key Components

| **Component** | **Technology** | **Purpose** |
|---|---|---|
| **Frontend** | React + TypeScript + Tailwind CSS | User interface & admin dashboard |
| **Backend** | Node.js + Express.js | API & business logic |
| **Database** | MongoDB + Mongoose | Data persistence |
| **ML Service** | FastAPI / Flask | Model serving & predictions |
| **Models** | Scikit-learn, NLP | ML predictions & analytics |

This architecture allows **independent development, deployment, and scaling** of the machine learning services without impacting the core application.

---

## 🧠 Machine Learning Models

EduGuard AI leverages multiple machine learning and NLP models to assess academic risk, predict performance, and analyze student sentiment.

### Model Overview

| **Model** | **Algorithm** | **Purpose** |
|---|---|---|
| **Dropout Risk Prediction** | Logistic Regression, Random Forest | Predicts dropout probability (Low/Medium/High) |
| **Performance Forecasting** | Linear Regression, Random Forest Regressor | Forecasts future exam scores & trends |
| **Sentiment Analysis** | TF-IDF + Supervised Classifier | Detects stress, anxiety, disengagement |
| **Chatbot Intent Detection** | NLP-based Text Classification | Identifies intent & emotional cues |

---

## 🛠️ Tech Stack

### Frontend
- **React.js** - UI library
- **TypeScript** - Type safety
- **Tailwind CSS** - Styling
- **Recharts / Chart.js** - Data visualization

### Backend
- **Node.js** - Runtime environment
- **Express.js** - Web framework
- **JWT Authentication** - Secure authentication
- **MongoDB + Mongoose** - Database & ODM

### Machine Learning
- **Python** - Core language
- **FastAPI / Flask** - API framework
- **Scikit-learn** - ML algorithms
- **Pandas, NumPy** - Data processing
- **TF-IDF** - NLP (Transformer models optional)

### Deployment
- **Frontend**: Vercel
- **Backend**: Render
- **ML API**: Railway / HuggingFace Spaces

---

## 🔐 User Roles

| **Role** | **Responsibilities** | **Key Features** |
|---|---|---|
| **Admin** | System control, analytics, thresholds | Dashboard control, user management, risk threshold configuration |
| **Mentor/Counselor** | Monitor risks, counseling insights | Track at-risk students, access counseling insights, intervention tools |
| **Student** | Performance tracking, chatbot support | View own performance, access academic chatbot, mental health resources |

---

## 🎯 Vision

EduGuard AI envisions a **future where no student is left behind** due to early warning signs being missed. We aim to:

- **Democratize early intervention** by making predictive analytics accessible to all educational institutions
- **Empower educators** with data-driven insights to provide timely, personalized support
- **Protect student well-being** by integrating mental health monitoring with academic tracking
- **Transform education** from reactive problem-solving to proactive student success
- **Bridge the gap** between technology and human care through AI-assisted counseling and mentorship

Our long-term vision is to create an **intelligent education ecosystem** where every student receives personalized support, timely interventions, and equal opportunity to succeed.

---

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

### MIT License Summary

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limited to the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

- **The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.**

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.

---

**© 2026 EduGuard AI. All rights reserved.**
