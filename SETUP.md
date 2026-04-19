# Setup Guide

## 1. Google Sheets Setup
Create a Google Sheet named **HR New Hires** with these columns:

- Name
- Email
- Role
- Department
- StartDate
- Manager
- Status
- EndDate

### Status values
Use:
- Hired
- Onboarded
- Offboarding
- Offboarded

## 2. Gmail
Connect Gmail in n8n using OAuth2.

Used for:
- welcome emails
- onboarding emails
- exit survey emails

## 3. Slack
Connect Slack in n8n.

Used for:
- manager alerts
- IT offboarding alerts

Recommended channel:
- `hr-onboarding`

## 4. Notion
Create a Notion database for onboarding records.

Suggested fields:
- Name
- Role
- Department
- Start Date
- Status

Connect your Notion integration to the database and use the database ID in n8n.

## 5. Groq
Create a Groq API key and connect it in n8n using HTTP Request.

Used for:
- generating role-based onboarding checklists

Recommended model:
- `llama-3.3-70b-versatile`

## 6. n8n Workflows
Import:
- `workflow-onboarding.json`
- `workflow-offboarding.json`

Then reconnect credentials for:
- Gmail
- Slack
- Google Sheets
- Notion
- Groq API

## 7. Test the workflows

### Onboarding test
Add a new employee row and set:

- Status = Hired

Expected result:
- onboarding plan generated
- welcome email sent
- Slack manager alert sent
- Notion page created
- HR sheet updated

### Offboarding test
Update an employee row and set:

- Status = Offboarding
- EndDate = any valid date

Expected result:
- exit survey email sent
- IT alert sent in Slack
- HR records updated

## 8. Notes
This project is designed as a portfolio-ready automation project and may require reconnecting credentials before use in another n8n environment.
