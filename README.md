# 🤖 n8n Placement Workflow — WIC Automation

> **Automated end-to-end WIC placement coordination using n8n workflow automation**

![n8n](https://img.shields.io/badge/Built%20with-n8n-EA4B71?style=for-the-badge&logo=n8n)
![Automation](https://img.shields.io/badge/Type-Workflow%20Automation-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Live%20Demo-brightgreen?style=for-the-badge)
![Healthcare](https://img.shields.io/badge/Domain-Healthcare-orange?style=for-the-badge)

---

## 📋 Overview

This project demonstrates a fully automated **WIC (Women, Infants, and Children) placement workflow** built using [n8n](https://n8n.io) — an open-source, low-code workflow automation platform.

The workflow eliminates manual coordination steps in WIC placement processes, reducing administrative burden, minimizing human error, and accelerating participant onboarding through intelligent automation.

---

## 🎯 Problem Statement

WIC placement coordination traditionally involves:
- Manual data entry across multiple systems
- Back-and-forth email/phone communication between coordinators
- Delayed notifications and missed follow-ups
- Inconsistent tracking of placement status

This automation solves all of the above by connecting all touchpoints into a single, self-running workflow.

---

## ⚙️ How It Works

```
Trigger (Form / Webhook / Schedule)
        │
        ▼
  Data Validation & Enrichment
        │
        ▼
  Eligibility Check (Logic Node)
        │
  ┌─────┴──────┐
  ▼            ▼
Eligible   Not Eligible
  │            │
  ▼            ▼
Placement   Notification
Assignment   + Follow-up
  │
  ▼
Confirmation & Record Update
  │
  ▼
Automated Notification to Participant
```

---

## 🚀 Key Features

| Feature | Description |
|---|---|
| 🔄 **Trigger-based Automation** | Initiates on form submission, webhook, or scheduled interval |
| ✅ **Eligibility Screening** | Automated logic checks for WIC qualification criteria |
| 📋 **Smart Placement Assignment** | Routes participants to available WIC locations/coordinators |
| 📧 **Automated Notifications** | Sends confirmation emails/SMS to participants and staff |
| 🗃️ **Record Management** | Auto-updates spreadsheet/database with placement status |
| 📊 **Error Handling** | Built-in retry logic and failure notifications |
| 🔒 **Secure Data Handling** | Credentials managed via n8n encrypted credential store |

---

## 🛠️ Tech Stack

- **[n8n](https://n8n.io)** — Core workflow automation engine (self-hosted)
- **Webhooks** — Real-time trigger events
- **HTTP Request Nodes** — API integrations with external services
- **Conditional Logic** — If/Switch nodes for eligibility routing
- **Email / SMS Nodes** — Automated participant communication
- **Google Sheets / Airtable** — Record keeping and status tracking
- **JSON Transform Nodes** — Data normalization and enrichment

---

## 📸 Demo

> 🎬 Live workflow demonstration available — showcasing the full automation pipeline from intake trigger to placement confirmation.

### Workflow Highlights:
- Intake form submission triggers the workflow in real-time
- Participant data is validated and eligibility is assessed automatically
- Placement is assigned and both participant and coordinator are notified instantly
- All records are updated without any manual intervention

---

## 📁 Repository Structure

```
n8n-placement-workflow/
├── workflows/
│   └── wic-placement-main.json    # Exportable n8n workflow file
├── docs/
│   ├── setup-guide.md             # How to import and configure
│   └── architecture-diagram.png   # Workflow architecture visual
├── sample-data/
│   └── test-payload.json          # Sample trigger payload for testing
└── README.md
```

---

## 🔧 Getting Started

### Prerequisites
- n8n instance (self-hosted or n8n Cloud)
- Access credentials for connected services (email, spreadsheet, etc.)

### Import the Workflow
1. Clone this repository
2. Open your n8n instance
3. Go to **Workflows → Import from File**
4. Select `workflows/wic-placement-main.json`
5. Configure credentials in the **Credentials** panel
6. Activate the workflow

---

## 💡 Use Cases & Applications

This automation pattern can be adapted for:
- Healthcare patient intake & coordination
- Social services case management
- Benefits enrollment processing
- Appointment scheduling & follow-up automation
- Any multi-step placement or referral workflow

---

## 🧠 Skills Demonstrated

- ✅ No-code / Low-code workflow design
- ✅ API integration and webhook handling
- ✅ Conditional logic and data routing
- ✅ Process automation for healthcare/social services
- ✅ Error handling and resilience patterns
- ✅ Documentation and workflow architecture

---

## 📬 Contact

**machamaniac** — open to automation consulting, n8n workflow design, and process optimization projects.

- 🐙 GitHub: [@machamaniac](https://github.com/machamaniac)

---

*Built as part of a portfolio demonstrating real-world workflow automation capabilities using n8n.*
