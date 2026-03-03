# GHL Configuration & Implementation Rules

## Single License / Two Clinics

### User Permissions
- **Location-restricted users** (Lexee, Nuhaa, Janine): Can only see leads tagged with their clinic location
- **Admin/Manager users** (Grant, Kyle, Amanda): Can see both pipelines for reporting

### Clinic Location Tagging
- Every lead must be tagged as **UK** or **SA** on entry
- This tag drives permission filtering and reporting

## Communication Policy
- **No automated emails/SMS** to patients at this stage
- Use **internal notifications** (mobile push / email) to prompt staff to send manual messages via existing tools
- All patient communication is manual and personal

## Key Integration Points
- **External Calendar:** Appointments are booked in the clinic's existing calendar system (not GHL calendar)
- **Medical History Form:** External link sent to patients (not a GHL form at this stage)
- **Pre-Consult Summary:** Document created by staff and linked via URL field in GHL

## Custom Fields Summary (All)

### Workflow 1 Fields
- Clinic Location (UK / SA)
- Lead Source (WhatsApp, Web, Referral)
- External Appt Date
- Pre-Consult Doc Link

### Workflow 2 Fields
- Internal Consult Notes
- Treatment Protocol Link
- Quote Status (Sent / Negotiating / Accepted)
- Escalation Reason (Pricing / Medical / Timing)
- Follow-up Consult Type (Free / Paid)
