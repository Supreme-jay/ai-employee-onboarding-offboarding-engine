# AI Employee Onboarding & Offboarding Engine
### Built with n8n + Groq (Free AI) | Full employee lifecycle on autopilot

![workflow](screenshots/workflow.png)

## The Problem
HR teams spend 2–4 hours per hire across 5 apps. 1 in 4 companies fail to
revoke access when employees leave — a major security risk.

## What This Does
### Onboarding (triggers when Status = Hired)
- AI generates personalized 30-day plan for their exact role
- Welcome email with checklist sent automatically
- Notion onboarding page created
- Manager notified in Slack
- HR sheet updated

### Offboarding (triggers when Status = Offboarding)
- Exit survey sent to departing employee
- IT team alerted to revoke ALL access within 24hrs
- Records updated and archived

## Tech Stack
| Tool | Purpose | Cost |
|------|---------|------|
| n8n | Workflow automation | Free |
| Groq (Llama 3.3 70B) | Checklist generation | 100% Free |
| Google Sheets | HR trigger + tracking | Free |
| Gmail | Welcome/exit emails | Free |
| Slack | Manager alerts | Free |
| Notion | Onboarding pages | Free |

---
Built by Ifeanyi Nwadike | Open to AI Automation Engineer roles
