# 🛡️ OmniGuard XAI
**Real-Time Adaptive Financial Fraud Detection System**

![OmniGuard XAI](https://img.shields.io/badge/Status-Hackathon_Ready-success) ![Tech Stack](https://img.shields.io/badge/Stack-React%20%7C%20Python%20%7C%20FastAPI%20%7C%20XGBoost-blue) 

OmniGuard XAI is an enterprise-grade, real-time fraud detection engine designed to stop financial crimes *before* the money leaves the server. By fusing Machine Learning (XGBoost + Isolation Forest) with eXplainable AI (SHAP) and dynamic Step-Up MFA, OmniGuard provides unparalleled security without compromising the user experience.

Built by **Team Collective**.

---

## ⚠️ The Problem Statement: The Silent Fraud Crisis

Modern financial institutions are losing billions to sophisticated, AI-driven cyber threats. Current legacy systems are failing due to four critical vulnerabilities:

1. **Reactive Defense:** Legacy systems flag fraud *after* funds are stolen. Banks urgently need pre-transaction prevention.
2. **Complex Attacks:** Coordinated, multi-channel threats (e.g., Account Takeovers, Synthetic IDs) easily bypass traditional rule-based engines.
3. **High Latency & Siloed Data:** Fragmented databases prevent the instant fusion of user behavior, device intelligence, and transaction context needed for real-time anomaly detection.
4. **The "Black Box" AI Problem:** Unexplainable AI alerts leave security teams (SOC) guessing *why* a transaction was flagged, causing critical delays in incident response.

---

## 💡 Our Solution: OmniGuard XAI

OmniGuard shifts the paradigm from post-transaction recovery to **pre-transaction prevention** with millisecond latency. 

### Core Features
* **🧠 Blended ML Engine:** Combines XGBoost (supervised) and Isolation Forest (unsupervised) for high-accuracy anomaly detection.
* **🔎 SHAP Explainability (XAI):** Translates complex ML decisions into human-readable insights for SOC analysts instantly.
* **🛡️ Dynamic Step-Up MFA:** Automatically triggers biometric or OTP verification for "medium-risk" transactions (Score 40-69) to block hackers while keeping real users moving.
* **👁️ Insider Threat Detection (UEBA):** Monitors internal employee portal logs to detect rogue admins, privilege escalation, and unauthorized data exports.
* **📱 Dual-Portal Simulation:** Includes a live Customer Mobile App simulator and an Employee Terminal to inject real-time attack vectors.

---

## 🏗️ Project Architecture & File Structure

```text
omniguard-xai/
│
├── backend/                  # Python API & ML Models
│   ├── main.py               # Main FastAPI/Flask application
│   ├── requirements.txt      # Python dependencies
│   ├── models/               # Pre-trained XGBoost & Isolation Forest models
│   ├── utils/                # Helper functions for data processing & SHAP
│   └── data/                 # Sample transaction datasets for evaluation
│
├── frontend/                 # React UI (SOC Dashboard & Mobile App)
│   ├── package.json          # Node modules and scripts
│   ├── vite.config.js        # Vite bundler configuration
│   ├── index.html            # Main HTML entry point
│   ├── public/               # Static assets (images, icons)
│   └── src/
│       ├── main.jsx          # React DOM render
│       ├── App.jsx           # Main SOC Analyst Dashboard Component
│       ├── MobileApp.jsx     # Customer & Employee Simulator (Attack Injector)
│       ├── components/       # Reusable UI widgets (Charts, Alerts, MFA)
│       └── styles/           # CSS modules and dark-theme styling
│
└── README.md                 # Project documentation
