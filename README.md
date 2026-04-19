# AI Employee Onboarding & Offboarding Engine
### Built with n8n + Groq (Free AI) | Full employee lifecycle on autopilot

![workflow](screenshots/workflow.png)

## Project Summary
The AI Employee Onboarding & Offboarding Engine is an HR automation project built with n8n and Groq AI to streamline the full employee lifecycle. It reduces manual HR work by automating onboarding tasks such as welcome emails, role-based onboarding checklist generation, Notion page creation, manager notifications, and HR record updates. It also handles offboarding by sending exit surveys, alerting IT to revoke access, and updating employee records automatically.

This project demonstrates practical workflow automation, AI integration, multi-app orchestration, and business process design using free and accessible tools. It is designed as a portfolio-ready solution for real-world HR operations.

## The Problem
HR teams spend 2–4 hours per hire across multiple apps and manual processes. Many companies also fail to revoke access properly when employees leave, creating a major security and operations risk.

## What This Does

### Onboarding (triggers when Status = Hired)
- AI generates a personalized 30-day onboarding plan for the employee’s exact role
- Welcome email with checklist is sent automatically
- Notion onboarding page is created
- Manager is notified in Slack
- HR sheet is updated automatically

### Offboarding (triggers when Status = Offboarding)
- Exit survey is sent to the departing employee
- IT team is alerted to revoke all access within 24 hours
- Records are updated and archived automatically

## Workflow Overview
This project automates the employee lifecycle from onboarding to offboarding using n8n and Groq AI.

The onboarding workflow starts when HR updates an employee's status to **Hired** in Google Sheets. The workflow then generates a personalized onboarding checklist, sends a welcome email, creates a Notion onboarding page, notifies the manager in Slack, and updates the HR tracker.

The offboarding workflow starts when HR changes an employee's status to **Offboarding**. It sends an exit survey, alerts IT to revoke all access, and updates the employee record.

## Files Included
- `workflow-onboarding.json` — n8n onboarding workflow export
- `workflow-offboarding.json` — n8n offboarding workflow export
- `screenshots/workflow.png` — workflow screenshot
- `SETUP.md` — setup instructions

## Tech Stack

| Tool | Purpose | Cost |
|------|---------|------|
| n8n | Workflow automation | Free |
| Groq (Llama 3.3 70B) | Checklist generation | 100% Free |
| Google Sheets | HR trigger + tracking | Free |
| Gmail | Welcome/exit emails | Free |
| Slack | Manager alerts | Free |
| Notion | Onboarding pages | Free |

## Key Features
- Automated onboarding trigger from Google Sheets
- Role-based AI onboarding checklist generation
- Automated welcome and exit email workflows
- Slack notifications for managers and IT teams
- Notion page creation for onboarding records
- Offboarding automation with access revocation alerts
- Structured HR record tracking and status updates

## Use Case
This project is ideal for:
- HR teams
- startup founders
- operations teams
- internal workflow automation
- AI automation engineer portfolios

## Built By
**Ifeanyi Nwadike**  
Open to AI Automation Engineer, Python Developer, Backend Developer, and Workflow Automation roles.

- LinkedIn: https://www.linkedin.com/in/ifeanyi-nwadike-aab752356
- GitHub: https://github.com/Supreme-jay
