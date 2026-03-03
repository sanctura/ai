This document is designed to be handed directly to **Shift 1**. It outlines the two-stage conversion process for the UK and SA clinics within a single HighLevel license.

---

# **Project: Patient Conversion Engine**

**Objective:** Standardize lead management and clinical conversion across the UK and South African clinics.
**Key Personnel:** * **Global Lead:** Grant Merwitz

* **Practice Managers:** Kyle Bennet (SA) / Amanda Ross (UK)
* **Reception/Patient Facing:** Nuhaa Peterson (SA), Janine Nathan (SA), Lexee Duval (UK)

---

## **Workflow 1: The "Front Desk Launchpad"**

**Goal:** Convert an inquiry into a "Doctor-Ready" consultation.

### **1. Pipeline Stages**

1. **New Inquiry:** Lead enters (Email/Web/Phone). System tags by location (**UK** or **SA**).
2. **Outreach Phase:** Staff initiates contact via WhatsApp/Email.
* *Escalation Logic:* If no response, switch medium (e.g., Email → WhatsApp → Phone Call).


3. **Booking Requested:** Patient agrees to a consult. Staff provides upfront pricing.
4. **Awaiting Med History:** Staff sends the **External Link** for medical history.
5. **Pre-Consult Prep:** History received. Staff creates a **Pre-Consult Summary** for the Doctor.
6. **Ready for Doctor:** Summary is linked in GHL; appointment is set in the **External Calendar**.

### **2. Essential GHL Config**

* **Custom Fields:** * `Clinic Location` (UK / SA) — *Used for user-level permissions.*
* `Lead Source` (WhatsApp, Web, Referral)
* `External Appt Date` (Date Picker)
* `Pre-Consult Doc Link` (URL field for the summary document)


* **Tasks:** Automatic reminders every 24–48 hours if a lead stays in "Outreach" or "Awaiting Med History" too long.

---

## **Workflow 2: The "Clinical Conversion Cycle"**

**Goal:** Convert a consultation into a committed treatment plan.

### **1. Pipeline Stages**

1. **Post-Consultation:** Doctor has seen the patient. Staff saves internal notes and sends the **Take-Home Summary** to the patient.
2. **Protocol & Quoting:** Staff generates the Treatment Protocol and **Multiple Quote Options**.
3. **Awaiting Proposal Acceptance:** Quotes are sent via Email/WhatsApp.
4. **Enquiry & Escalation:** (For patients with questions/price concerns).
* *Action:* Escalate to **Kyle (SA)** or **Amanda (UK)**.
* *Action:* If clinical, escalate to **Doctor/Nurse**.
* *Action:* Schedule Follow-up Consult (Marked as **Free** or **Paid**).


5. **Treatment Booked:** Quote accepted. Staff books the treatment block in the **External Calendar**.
6. **Converted Patient (Closed Won):** Opportunity closed.

### **2. Essential GHL Config**

* **Custom Fields:**
* `Internal Consult Notes` (Text Area)
* `Treatment Protocol Link` (URL)
* `Quote Status` (Sent / Negotiating / Accepted)
* `Escalation Reason` (Pricing / Medical / Timing)
* `Follow-up Consult Type` (Dropdown: Free / Paid)



---

## **Implementation Rules for Shift 1**

### **A. Single License / Two Clinics**

* Use **User Permissions** to ensure Lexee (UK) only sees UK leads, and Nuhaa/Janine (SA) only see SA leads.
* Grant, Kyle, and Amanda must have "Admin" or "Manager" visibility to see both pipelines for reporting.

### **B. Manual Communication**

* **No automated emails/SMS** to patients at this stage.
* Use **Internal Notifications** (Mobile Push/Email) to prompt staff to send manual messages via their existing tools.

### **C. The "Pre-Consult Summary" Bridge**

* The transition between Workflow 1 and 2 is complete **only** when the `Pre-Consult Doc Link` is populated. This ensures the Doctor is never blind in a consultation.

---
