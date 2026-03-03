# Workflow 2: The "Clinical Conversion Cycle"

## Goal
Convert a consultation into a committed treatment plan.

## Pipeline Stages

### 1. Post-Consultation
- Doctor has seen the patient
- Staff saves internal notes
- Staff sends Take-Home Summary to the patient

### 2. Protocol & Quoting
- Staff generates the Treatment Protocol
- Staff creates multiple quote options

### 3. Awaiting Proposal Acceptance
- Quotes sent via Email/WhatsApp

### 4. Enquiry & Escalation
For patients with questions or price concerns:
- **Pricing concerns:** Escalate to Kyle (SA) or Amanda (UK)
- **Clinical concerns:** Escalate to Doctor/Nurse
- **Follow-up:** Schedule follow-up consult (marked as Free or Paid)

### 5. Treatment Booked
- Quote accepted
- Staff books the treatment block in the external calendar

### 6. Converted Patient (Closed Won)
- Opportunity closed

## GHL Configuration

### Custom Fields
| Field | Type | Purpose |
|-------|------|---------|
| Internal Consult Notes | Text Area | Doctor/staff notes from consultation |
| Treatment Protocol Link | URL | Link to treatment protocol document |
| Quote Status | Dropdown (Sent / Negotiating / Accepted) | Track quoting progress |
| Escalation Reason | Dropdown (Pricing / Medical / Timing) | Categorise escalation type |
| Follow-up Consult Type | Dropdown (Free / Paid) | Track follow-up consult billing |
