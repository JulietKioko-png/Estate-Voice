# Requirements: Estate Voice

## 1. Functional requirements (what the system does)

### Accounts and access
- FR1: A resident can register with name, email or phone, password, and estate/block.
- FR2: Users log in on one login page; the system sends them to the right page based on their role.
- FR3: There is no public admin sign-up. The first admin is created directly in the database, and admins can add other admins.
- FR4: Passwords are stored hashed.

### Resident features
- FR5: A resident can submit a complaint or feedback message (and optionally a photo).
- FR6: A resident can view their own submitted messages.
- FR7: A resident can see the status of each message (received, assigned, in progress, resolved).

### AI features
- FR8: The system classifies each new message by type (complaint, positive feedback, suggestion).
- FR9: The system assigns a category (water, security, electricity, garbage, lifts, noise, rent or service charge, other).
- FR10: The system assigns an urgency level (high, medium, low).
- FR11: The system works with English and Kiswahili messages.
- FR12: The admin can correct a wrong label.

### Admin features
- FR13: The admin can view all messages in a dashboard.
- FR14: The admin can filter by category, type, urgency, status, block, and date.
- FR15: The admin can update the status and add a comment visible to the resident.
- FR16: The admin can see summary counts (for example, complaints per category).
- FR17: The admin can export a simple report (CSV or printable page).

## 2. Non-functional requirements (how well it works)

| Area | Requirement |
|---|---|
| Security | Hashed passwords, input validation, role checks on every page, API keys in .env |
| Privacy | Residents see only their own messages; fake data used in the demo; Data Protection Act noted in README |
| Usability | Simple, works on small phone screens |
| Performance | Pages load in a few seconds; AI result shown shortly after submission |
| Reliability | Messages are saved even if the AI service fails (labelled "unclassified") |
| Maintainability | Clean folder structure, comments, and regular Git commits |

## 3. User stories
- As a resident, I want to submit a complaint in one place so that it is not lost in a WhatsApp group.
- As a resident, I want to see the status of my complaint so that I know it is being handled.
- As an admin, I want messages sorted by urgency so that I deal with serious problems first.
- As an admin, I want to correct a wrong AI label so that my reports stay accurate.
- As an admin, I want a summary report so that I can show the estate committee what is happening.

## 4. Assumptions and constraints
- Residents have a smartphone or computer with internet access.
- The demo uses fake data only.
- One developer, about 6 weeks, free-tier hosting.
