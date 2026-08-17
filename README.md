# AIMS-AI-Receptionist
Bilingual AI front desk system with voice and WhatsApp automation.
https://aims-frontend-ten.vercel.app/](https://aims-frontend-ten.vercel.app/



#  AIMS — AI Front Desk & Omnichannel Operations Platform

[![Live Demo](https://img.shields.io/badge/Demo-Live%20App-blue?style=for-the-badge&logo=vercel)](https://aims-frontend-ten.vercel.app/)
[![Stack](https://img.shields.io/badge/Stack-Python%20%7C%20React%20%7C%20FastAPI%20%7C%20Vapi%20%7C%20Twilio-green?style=for-the-badge)](#tech-stack)

AIMS (Artificial Intelligence Management System) is an enterprise-grade, bilingual (English/Spanish) front desk receptionist and workflow engine. It automates real-time voice calls, WhatsApp messaging, appointment scheduling, and patient/client intake processing from a unified real-time dashboard.

---

##  Live Interactive Demo
 **[Try the Live Web Application](https://aims-frontend-ten.vercel.app/)**

---

##  Tech Stack & Infrastructure

- **Frontend:** React, Tailwind CSS, React Query, Lucide Icons (Vercel deployment)
- **Backend / APIs:** Python (FastAPI/Django), RESTful endpoints, Webhooks pipeline
- **Voice & Telephony:** Vapi AI (Real-time voice streaming), Twilio API, OpenAI TTS
- **Messaging:** WhatsApp Business API integration
- **Data Engineering & Cloud:** Automated pipelines, Azure & Databricks ecosystem readiness for enterprise analytics
- **Database & State:** Real-time sync for calendar scheduling and tablet intake forms

---

## ⚙️ Core Architecture & Features

### 1.  Real-Time Voice Engine (Low-Latency)
- Bi-directional voice streaming over WebSockets/SIP.
- Context-aware natural voice conversational agent with dynamic context switching (English ↔ Spanish).

### 2.  Omnichannel WhatsApp Automation
- Direct sync with backend database.
- Handles FAQs, appointment requests, and client validation seamlessly.

### 3.  Operational Core & Scheduling
- Real-time availability checks.
- Direct creation and update of appointments, patient records, and invoices.

### 4.  Digital Tablet Intake System (`/ficha`)
- Standalone full-screen digital form designed for tablet interaction at physical clinics or front desks.
- Instant submission to the core database without requiring admin layout overhead.

---

##  API Reference & Core Webhooks

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `POST` | `/api/v1/voice/webhook` | Handles incoming Vapi/Twilio real-time audio streams & intent classification |
| `POST` | `/api/v1/whatsapp/message` | Processes incoming WhatsApp messages and triggers AI reply pipeline |
| `GET` | `/api/v1/appointments` | Retrieves real-time calendar availability & booked slots |
| `POST` | `/api/v1/appointments` | Creates a new confirmed appointment in the database |
| `POST` | `/api/v1/patients/intake` | Receives digital intake form submissions from the tablet interface |

---

##  Local Setup & Installation

```bash
# Clone repository
git clone [https://github.com/tu-usuario/AIMS-Frontend.git](https://github.com/tu-usuario/AIMS-Frontend.git)

# Install dependencies
npm install

# Run development server
npm run dev
