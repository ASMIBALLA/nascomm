# nascomm
ClaimBridge is a smart, voice-enabled AI agent tailored for insurance claim management, specifically in the health and travel sectors, signifying the  connection between the user and their insurer/support team. It streamlines the end-to-end claims journey: from capturing user information for a new claim, to retrieving real-time claim statuses, estimating resolution timelines, and delivering updates via SMS or email. The agent acts as a digital claims guide, integrated seamlessly with Zoho CRM for lead capture, Google Sheets for live status lookups, and communication channels for proactive notifications.

# ClaimBridge – Backend Logic (AuroraWave)

This repository contains backend logic and workflow scripts for **SureClaim**, an AI-powered Claims Assistant agent built for the Inya.ai Buildathon 2025.

## 🧠 Purpose

SureClaim simplifies insurance claim management by allowing users to:
- Submit new claims via a guided flow
- Check existing claim statuses
- Receive SMS/email updates with estimated resolution times

Backend workflows are implemented using **Pipedream** and integrated with **Google Sheets** and **Zoho CRM**.

---

## 📁 Contents

| Folder | Purpose |
|--------|---------|
| `pipedream/` | Backend scripts used in Pipedream workflows |
| `docs/` | Logic breakdown and flow diagrams |
| `assets/` | Screenshots and visual aids |

---

## 🔁 Key Workflows

### 1. `fetchClaimStatus.js`
Retrieves claim data from Google Sheets and estimates resolution time.

- Input: Claim ID or phone/email
- Output: Claim summary + dynamic ETA
- Optional: Sends summary via SMS or Email

---

## 🔌 Integrations

| Tool         | Purpose                        |
|--------------|--------------------------------|
| Inya.ai      | Frontend conversational agent  |
| Zoho CRM     | Stores submitted claims        |
| Google Sheets| Claim status storage & lookup  |
| Pipedream    | Executes backend workflows     |
| SMS/Email API| Sends user notifications       |

---

## 🚀 How to Use

1. Clone this repo
2. Set up a Google Sheet with claim records
3. Deploy Pipedream workflows using `/pipedream/fetchClaimStatus.js`
4. Link Pipedream endpoints to Inya.ai agent actions

---

## 🧾 Authors
**Team AuroraWave**
- Asmi Balla (Agent & Workflow Architect)

