# Mail to Tyler — Pilot Workflows

**To:** Tyler
**From:** Grant
**Subject:** HighLevel Pilot — Two Workflows to Get Started

---

Hi Tyler,

Great chatting today and thanks for walking me through HighLevel — it looks like a solid fit for what we need.

As promised, here are the two workflows I'd like us to pilot. We run clinics in both the UK and South Africa off a single license, so location tagging and permissions are important throughout.

---

## Workflow 1: "Front Desk Launchpad"

**Goal:** Take an inquiry from first contact through to a doctor-ready consultation.

**Pipeline stages:**

1. **New Inquiry** — Lead comes in via email, web, or phone. Tagged as UK or SA.
2. **Outreach Phase** — Staff reaches out via WhatsApp or email. If no response, we escalate the medium (e.g. email → WhatsApp → phone call).
3. **Booking Requested** — Patient agrees to a consult and receives upfront pricing.
4. **Awaiting Med History** — Staff sends the patient a link to complete their medical history.
5. **Pre-Consult Prep** — History received, staff prepares a Pre-Consult Summary for the doctor.
6. **Ready for Doctor** — Summary linked in GHL, appointment set in our external calendar.

**Custom fields we'll need:**
- Clinic Location (UK / SA)
- Lead Source (WhatsApp, Web, Referral)
- External Appointment Date (date picker)
- Pre-Consult Doc Link (URL)

**Automation:** Internal reminders (push/email to staff) if a lead sits in "Outreach" or "Awaiting Med History" for more than 24–48 hours. No automated messages go to patients — all patient communication is manual at this stage.

---

## Workflow 2: "Clinical Conversion Cycle"

**Goal:** Convert a completed consultation into a booked treatment plan.

**Pipeline stages:**

1. **Post-Consultation** — Doctor has seen the patient. Staff saves internal notes and sends the patient a take-home summary.
2. **Protocol & Quoting** — Staff generates the treatment protocol and multiple quote options.
3. **Awaiting Proposal Acceptance** — Quotes sent to the patient via email/WhatsApp.
4. **Enquiry & Escalation** — For patients with questions or pricing concerns:
   - Pricing → escalate to Kyle (SA) or Amanda (UK)
   - Clinical → escalate to doctor/nurse
   - Schedule a follow-up consult if needed (marked as free or paid)
5. **Treatment Booked** — Quote accepted, treatment block booked in external calendar.
6. **Converted Patient (Closed Won)** — Opportunity closed.

**Custom fields we'll need:**
- Internal Consult Notes (text area)
- Treatment Protocol Link (URL)
- Quote Status (Sent / Negotiating / Accepted)
- Escalation Reason (Pricing / Medical / Timing)
- Follow-up Consult Type (Free / Paid)

---

## A Few Important Notes

- **Single license, two clinics** — We need user permissions so UK staff only see UK leads and SA staff only see SA leads. Managers and I need visibility across both.
- **No automated patient comms** — Everything patient-facing is manual for now. Internal notifications to prompt staff are fine.
- **The bridge between the two workflows** is the Pre-Consult Doc Link — Workflow 1 isn't complete until that's populated, ensuring the doctor is never going in blind.

Happy to jump on a call to talk through any of this in more detail. Let me know what you need from our side to get these set up.

Cheers,
Grant
