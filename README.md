# 🚀 Business Automation Workflow (n8n)

<p align="center">
  <img src="Logo.png" alt="Business Automation Logo" width="180">
</p>

<p align="center">
  <b>An End-to-End Business Automation Workflow built with n8n, Google Sheets, Groq AI, WhatsApp Cloud API, and Gmail.</b>
</p>

---

## 📌 Project Overview

This project automates the complete customer lead management process from lead capture to follow-up and reporting.

The workflow:

- Captures leads using a Webhook
- Stores lead information in Google Sheets
- Generates AI-powered follow-up messages using Groq AI
- Sends WhatsApp messages automatically
- Updates CRM lead status
- Generates and emails weekly CRM reports

---

# 🏗 Workflow Architecture

```text
Webhook
    │
    ▼
Append Lead to Google Sheets
    │
    ▼
Generate AI Follow-up (Groq AI)
    │
    ▼
Send WhatsApp Message
    │
    ▼
Update Lead Status (Google Sheets)

────────────────────────────

Weekly Schedule Trigger
    │
    ▼
Read CRM Data
    │
    ▼
Generate Weekly Report
    │
    ▼
Send Gmail Report
```

---

# ⚙️ Technologies Used

- n8n
- Google Sheets API
- Groq AI API
- WhatsApp Cloud API
- Gmail API
- JavaScript
- Webhooks
- HTTP Request

---

# 📁 Project Structure

```text
Business-Automation/

├── Architecture.jpg
├── Business-Automation.json
├── Google-Sheet.png
├── LICENSE
├── Logo.png
├── README.md
├── Webhook-Test.png
├── Weekly-CRM-Report-Email.png
├── Whatsapp-Message.jpeg
├── Workflow.png
└── .gitignore
```

---

# ✨ Features

## 🔹 Lead Capture Automation

- Receives new leads using Webhook
- Saves lead information into Google Sheets
- Automatically records:
  - Name
  - Email
  - Phone
  - Requirement
  - Status
  - Created At

---

## 🤖 AI-Powered WhatsApp Follow-up

- Sends customer information to Groq AI
- Generates personalized follow-up messages
- Automatically sends the response through WhatsApp Cloud API

---

## 📋 CRM Status Update

Automatically updates lead status after sending the WhatsApp message.

Example:

```text
New
   ↓
Contacted
```

---

## ⏰ Scheduled Lead Processing

Runs automatically using the Schedule Trigger.

- Reads CRM data
- Processes existing leads
- Updates Google Sheets
- Keeps CRM synchronized

---

## 📧 Weekly CRM Report

Every week the workflow automatically:

- Reads all CRM records
- Calculates:
  - Total Leads
  - New Leads
  - Contacted Leads
  - Follow-up 1
  - Follow-up 2
  - Converted Leads
- Sends an automated report via Gmail

---

# 📊 Sample CRM Sheet

| Name | Email | Phone | Requirement | Status |
|------|-------|-------|------------|--------|
| John Doe | john@gmail.com | 9876543210 | Kitchen Interior Design | New |

---

# ▶️ Getting Started

## 1. Clone Repository

```bash
git clone https://github.com/parmarhemeen05/BUSINESS-AUTOMATION.git
```

---

## 2. Open n8n

Start your local or cloud n8n instance.

---

## 3. Import Workflow

Import:

```text
Business-Automation.json
```

---

## 4. Configure Credentials

Replace the placeholder credentials with your own:

- Google Sheets OAuth2
- Groq API Key
- WhatsApp Cloud API Token
- Gmail OAuth2

> **Important:** Never upload your real API keys or access tokens to GitHub.

---

## 5. Execute Workflow

Run the Webhook or Schedule Trigger to test the automation.

---

# 🔄 Workflow Summary

```
New Lead
     │
     ▼
Webhook Trigger
     │
     ▼
Google Sheets
     │
     ▼
Groq AI
     │
     ▼
WhatsApp Message
     │
     ▼
CRM Updated

Weekly Trigger
     │
     ▼
Read CRM
     │
     ▼
Generate Report
     │
     ▼
Gmail Report
```

---

# 🚀 Future Improvements

- 📊 Interactive CRM Dashboard
- 🤖 AI Lead Scoring
- 💬 Slack Notifications
- 📱 SMS Integration
- 👥 Multi-user CRM
- 📈 Analytics Dashboard
- 🌐 Multi-language Support

---

# 👨‍💻 Author

## Hemeen Parmar

**Computer Science & Engineering Student**

**DevOps • Cloud • Automation • AI Workflows**

GitHub:
https://github.com/parmarhemeen05

---

# 📄 License

This project is licensed under the **MIT License**.

See the **LICENSE** file for more information.

---

## ⭐ Support

If you found this project useful, please consider giving it a ⭐ on GitHub.

It helps others discover the project and motivates future improvements.
