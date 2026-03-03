# Workflow 1: The "Front Desk Launchpad"

## Goal
Convert an inquiry into a "Doctor-Ready" consultation.

## Pipeline Stages

### 1. New Inquiry
- Lead enters via Email, Web, or Phone
- System tags by location (UK or SA)

### 2. Outreach Phase
- Staff initiates contact via WhatsApp/Email
- **Escalation Logic:** If no response, switch medium (Email -> WhatsApp -> Phone Call)

### 3. Booking Requested
- Patient agrees to a consult
- Staff provides upfront pricing

### 4. Awaiting Med History
- Staff sends external link for medical history form

### 5. Pre-Consult Prep
- Medical history received
- Staff creates a Pre-Consult Summary for the Doctor

### 6. Ready for Doctor
- Summary is linked in GHL
- Appointment is set in the external calendar

## GHL Configuration

### Custom Fields
| Field | Type | Purpose |
|-------|------|---------|
| Clinic Location | Dropdown (UK / SA) | User-level permissions filtering |
| Lead Source | Dropdown (WhatsApp, Web, Referral) | Tracking lead origin |
| External Appt Date | Date Picker | Consultation date |
| Pre-Consult Doc Link | URL | Link to summary document for Doctor |

### Automation / Tasks
- Automatic reminders every 24-48 hours if a lead stays in "Outreach" or "Awaiting Med History" too long
- These are **internal staff reminders only** (no patient-facing automation)

## Transition to Workflow 2
- Workflow 1 is complete **only** when the `Pre-Consult Doc Link` is populated
- This ensures the Doctor is never blind in a consultation
