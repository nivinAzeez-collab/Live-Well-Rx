# Live Well Rx
## Product Backlog
### Pharmacy Prescription Refill Mobile Application

Owner: Live Well Pharmacy  
Product: Live Well Rx  
Location: Brooklyn, NY  

---

# Epic 1 — User Account & Authentication

## Goal
Allow patients to securely create and access their pharmacy accounts.

---

### User Story 1.1 — Create Account

**As a patient**  
I want to create an account  
So that I can manage my prescriptions digitally.

**Acceptance Criteria**

- User can sign up using:
  - Phone number
  - Email
  - Date of Birth
- User receives SMS verification code
- Account is created after verification
- Password must meet security requirements
- User must accept privacy policy

---

### User Story 1.2 — Login

**As a patient**  
I want to log in to my account  
So that I can access my prescriptions.

**Acceptance Criteria**

- User can log in with phone/email and password
- Incorrect credentials return error message
- Login session persists for authenticated users
- Two-factor authentication available

---

### User Story 1.3 — Password Reset

**As a patient**  
I want to reset my password  
So that I can recover access to my account.

**Acceptance Criteria**

- User can request password reset
- Reset link or code sent via email/SMS
- Password can be updated securely

---

# Epic 2 — Patient Profile Management

## Goal
Allow patients to manage personal information.

---

### User Story 2.1 — View Profile

**As a patient**  
I want to view my profile  
So that I can confirm my personal information.

**Acceptance Criteria**

- Display:
  - Name
  - Date of Birth
  - Address
  - Phone number
  - Insurance information

---

### User Story 2.2 — Update Profile

**As a patient**  
I want to update my contact details  
So the pharmacy can deliver medications correctly.

**Acceptance Criteria**

- Patient can update:
  - Address
  - Phone number
  - Email
- Changes saved securely
- Pharmacy system updated

---

# Epic 3 — Prescription Management

## Goal
Allow patients to view and manage prescriptions.

---

### User Story 3.1 — View Prescriptions

**As a patient**  
I want to see my prescriptions  
So I know what medications I take.

**Acceptance Criteria**

Display:

- Medication name
- Dosage
- Quantity
- Remaining refills
- Last filled date
- Prescribing doctor

---

### User Story 3.2 — View Medication Details

**As a patient**  
I want to see medication instructions  
So I can take the medication correctly.

**Acceptance Criteria**

Display:

- Dosage instructions
- Warnings
- Drug information
- Refill eligibility

---

# Epic 4 — Prescription Refills

## Goal
Allow patients to refill prescriptions digitally.

---

### User Story 4.1 — Refill Prescription

**As a patient**  
I want to refill my medication  
So that I do not run out of medication.

**Acceptance Criteria**

- Patient can select prescription
- Tap "Refill"
- Select pickup or delivery
- Order confirmation displayed

---

### User Story 4.2 — Refill Multiple Medications

**As a patient**  
I want to refill multiple prescriptions  
So I can receive them together.

**Acceptance Criteria**

- Patient can select multiple medications
- One order created
- Delivery grouped together

---

# Epic 5 — Refill Authorization

## Goal
Allow patients to request additional refills when no refills remain.

---

### User Story 5.1 — Request Refill Authorization

**As a patient**  
I want to request more refills  
So my doctor can approve additional medication.

**Acceptance Criteria**

- Button: "Request Refill Authorization"
- Request sent to pharmacy
- Pharmacy contacts doctor
- Status visible to patient

---

### User Story 5.2 — Refill Request Status

**As a patient**  
I want to track refill requests  
So I know when my medication is approved.

**Acceptance Criteria**

Statuses:

- Sent to pharmacy
- Sent to doctor
- Approved
- Denied

---

# Epic 6 — Pickup & Delivery

## Goal
Allow patients to choose medication delivery method.

---

### User Story 6.1 — Select Pickup

**As a patient**  
I want to pick up my medication  
So that I can collect it from the pharmacy.

**Acceptance Criteria**

- Select pickup
- Select pickup time
- Receive notification when ready

---

### User Story 6.2 — Select Delivery

**As a patient**  
I want medication delivered  
So I do not need to visit the pharmacy.

**Acceptance Criteria**

- Select delivery address
- Confirm delivery method
- Delivery scheduled

---

### User Story 6.3 — Delivery Tracking

**As a patient**  
I want to track my delivery  
So I know when it will arrive.

**Acceptance Criteria**

Display:

- Delivery status
- Estimated arrival time
- Delivery confirmation

---

# Epic 7 — Notifications

## Goal
Keep patients informed of medication status.

---

### User Story 7.1 — Push Notifications

**As a patient**  
I want notifications  
So I know when prescriptions are ready.

**Acceptance Criteria**

Notifications for:

- Prescription ready
- Refill approved
- Delivery on the way
- Refill reminder

---

### User Story 7.2 — Refill Reminders

**As a patient**  
I want refill reminders  
So I do not run out of medication.

**Acceptance Criteria**

- Reminder sent before medication runs out
- Patient can refill directly from notification

---

# Epic 8 — Secure Messaging

## Goal
Allow patients to communicate with pharmacists.

---

### User Story 8.1 — Send Message

**As a patient**  
I want to message the pharmacist  
So I can ask medication questions.

**Acceptance Criteria**

- Secure HIPAA compliant messaging
- Message history saved
- Pharmacy notified of new message

---

### User Story 8.2 — Receive Response

**As a patient**  
I want to receive pharmacist responses  
So I can get medication guidance.

**Acceptance Criteria**

- Notification when pharmacist replies
- Messages displayed in chat thread

---

# Epic 9 — Pharmacy Admin Dashboard

## Goal
Allow pharmacy staff to manage patient requests.

---

### User Story 9.1 — View Refill Requests

**As pharmacy staff**  
I want to see refill requests  
So I can process them quickly.

---

### User Story 9.2 — Send Refill Requests to Doctors

**As pharmacy staff**  
I want to send refill authorization requests  
So doctors can approve medications.

---

### User Story 9.3 — Manage Delivery Orders

**As pharmacy staff**  
I want to manage delivery schedules  
So medications arrive on time.

---

# Epic 10 — Compliance & Security

## Goal
Ensure the system complies with healthcare regulations.

---

### User Story 10.1 — HIPAA Compliance

**As a pharmacy owner**  
I want the app to follow HIPAA rules  
So patient data is protected.

**Acceptance Criteria**

- Encrypted patient data
- Secure authentication
- Role based access
- Audit logs

---

# Epic 11 — Integrations

## Goal
Integrate the app with pharmacy management systems.

---

### User Story 11.1 — Pharmacy Software Integration

**As a pharmacy owner**  
I want the app connected to PrimeRx  
So prescriptions update automatically.

**Acceptance Criteria**

- Prescription data synced
- Patient profiles synced
- Refill status updated

---

# Epic 12 — Future Enhancements

---

### Telepharmacy

Video calls with pharmacists.

---

### Auto Refills

Automatic refill enrollment.

---

### Copay Payment

Pay copays through the app.

---

### Family Accounts

Manage medications for children or parents.
