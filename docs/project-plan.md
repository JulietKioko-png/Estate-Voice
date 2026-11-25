# Project Plan: Estate Voice

## 1. Project title
Estate Voice: an AI-assisted resident complaints and feedback system for apartments and affordable housing estates.

## 2. Problem statement
Residents of apartment estates usually share complaints in WhatsApp groups. These groups have hundreds of messages, so one property manager or admin cannot read them all. Urgent problems (no water, security issues) get lost, complaints are repeated, and residents do not know whether anything is being done.

## 3. Project goal
Build a web system where residents submit complaints and feedback in one place, and where AI sorts each message so the admin can see what needs attention first.

## 4. Objectives
1. Let residents register, log in, and submit complaints or feedback.
2. Automatically classify each message by type (complaint, positive feedback, suggestion), category (water, security, electricity, etc.), and urgency.
3. Give the admin a dashboard to view, filter, and update messages.
4. Let residents track the status of their complaints.
5. Generate simple reports for the admin.

## 5. Scope

### In scope (Version 1)
- Responsive web application (works on phones and laptops)
- Resident and admin roles with secure login
- Complaint submission and status tracking
- AI classification of messages
- Admin dashboard, filters, and a basic report
- Support for English and Kiswahili messages (Sheng as a stretch goal)

### Out of scope (future versions)
- Android app for residents
- Direct WhatsApp integration
- SMS and email alerts
- Payments (rent or service charge)

## 6. Users

| User | Description |
|---|---|
| Resident | Lives in the estate; submits and tracks complaints |
| Admin | Property manager or estate office; reviews and resolves complaints |

## 7. Proposed technology

| Layer | Tool |
|---|---|
| Frontend | HTML, CSS, JavaScript, Bootstrap |
| Backend | Python (FastAPI or Django) |
| Database | MySQL or PostgreSQL |
| AI | Language model API returning category, type, and urgency |
| Version control | Git and GitHub |

## 8. Development approach
Iterative (Agile-style): build and test one small piece at a time, following the SDLC phases.

## 9. Timeline (about 6 weeks)

| Week | Work |
|---|---|
| 1 | Requirements, database design, ER diagram, project setup |
| 2 | Registration, login, and roles |
| 3 | Resident complaint form and "My complaints" page |
| 4 | Admin dashboard, filters, and status updates |
| 5 | AI classification and admin correction of labels |
| 6 | Testing, deployment, demo video, README |

## 10. Risks and how to handle them

| Risk | Plan |
|---|---|
| Scope grows too big | Keep to the Version 1 list above |
| AI labels incorrectly | Admin can correct labels; report accuracy in testing |
| Privacy of resident data | Use fake data, hash passwords, keep keys in .env |
| Running out of time | Build the core first, leave AI polish for last |

## 11. Success criteria
- A resident can submit a complaint and see its status change.
- The admin sees messages automatically labelled and sorted by urgency.
- The AI labels at least about 80% of the sample messages correctly (to be measured).
- The system is deployed with a live link, README, and demo video.
