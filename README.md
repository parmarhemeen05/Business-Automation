# 🚀 Business Automation Workflow (n8n)

An end-to-end business automation workflow built using **n8n**, **Google Sheets**, **Groq AI**, **WhatsApp Cloud API**, and **Gmail** to automate lead management, customer communication, and CRM reporting.

---

## 📌 Project Overview

This project automates the complete lead management process:

- Capture leads using a Webhook
- Store lead information in Google Sheets
- Generate AI-powered follow-up messages using Groq AI
- Send WhatsApp messages automatically
- Update lead status in the CRM
- Generate and email weekly CRM reports

---

# 🏗 Workflow Architecture

```
Webhook
    │
    ▼
Append Row (Google Sheets)
    │
    ▼
Groq AI (HTTP Request)
    │
    ▼
WhatsApp Cloud API
    │
    ▼
Update Lead Status
```

---

# ⚙️ Technologies Used

- n8n
- Google Sheets API
- Groq AI API
- WhatsApp Cloud API
- Gmail API
- JavaScript

---

# 📁 Project Structure

```
business-automation/
│
├── assets/
│   └── logo.png
│
├── docs/
│   ├── architecture.png
│   └── workflow.png
│
├── screenshots/
│   ├── workflow-canvas.png
│   ├── webhook-test.png
│   ├── google-sheet.png
│   ├── whatsapp-message.png
│   ├── weekly-crm-report-email.png
│   └── output.png
│
├── Business-Automation.json
├── LICENSE
├── README.md
└── .gitignore
```

---

# 🚀 Features

## 1️⃣ Lead Capture Automation

- Receives new leads via Webhook
- Saves lead details in Google Sheets
- Stores:
  - Name
  - Email
  - Phone
  - Requirement
  - Status
  - Created At

---

## 2️⃣ AI WhatsApp Follow-up

- Sends lead details to Groq AI
- Generates personalized follow-up messages
- Sends the generated message using WhatsApp Cloud API

---

## 3️⃣ CRM Status Update

Automatically updates lead status after communication.

Example:

```
New → Contacted
```

---

## 4️⃣ Scheduled Lead Processing

Runs automatically using Schedule Trigger.

- Reads CRM data
- Updates lead status
- Maintains Google Sheets automatically

---

## 5️⃣ Weekly CRM Report

Every week:

- Reads all CRM records
- Counts:
  - Total Leads
  - New Leads
  - Contacted
  - Follow-up 1
  - Follow-up 2
  - Converted
- Sends an automated report via Gmail

---

# 📊 Sample CRM Sheet

| Name | Email | Phone | Requirement | Status |
|------|-------|-------|------------|--------|
| John Doe | john@gmail.com | 9876543210 | Kitchen Interior Design | New |

---

# 📸 Screenshots

### Workflow

![Workflow](docs/workflow.png)

### Architecture

![Architecture](docs/architecture.png)

### Google Sheet

![Google Sheet](screenshots/google-sheet.png)

### WhatsApp

![WhatsApp](screenshots/whatsapp-message.png)

### Gmail Report

![Gmail](screenshots/weekly-crm-report-email.png)

---

# ▶️ How to Run

1. Clone the repository

```
git clone https://github.com/yourusername/business-automation.git
```

2. Open n8n.

3. Import

```
Business-Automation.json
```

4. Configure:

- Google Sheets Credentials
- Groq API Key
- WhatsApp Cloud API
- Gmail Credentials

5. Execute the workflow.

---

# 📌 Future Improvements

- CRM Dashboard
- Slack Notifications
- SMS Integration
- AI Lead Scoring
- Multi-user Support

---

# 👨‍💻 Author

**Hemeen Parmar**

Computer Science & Engineering Student
DevOps & Automation Enthusiast

GitHub: https://github.com/parmarhemeen05

---

# 📄 License

This project is licensed under the MIT License.