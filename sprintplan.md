# Live Well Rx
## Single-Agent Sprint Plan (Windsurf AI Development)

Product: Live Well Rx  
Organization: Live Well Pharmacy  
Goal: Build a HIPAA-compliant mobile pharmacy application that allows patients to refill prescriptions, request additional refills, and choose pickup or delivery.

Development Method:  
Single AI agent in Windsurf executing sequential tasks.

Stack:
- React Native (Expo)
- Node.js (Express)
- PostgreSQL
- Firebase Cloud Messaging
- HIPAA-compliant cloud hosting (AWS)

Sprint Duration: 1 week  
Total Estimated Sprints: 10

---

# Development Principles for Single-Agent Workflow

The AI agent will follow this cycle for every sprint:

1. Plan the feature
2. Generate code
3. Generate database schema
4. Write API endpoints
5. Build frontend screens
6. Write tests
7. Fix errors
8. Commit code

---

# Sprint 0 — Project Initialization

## Objective
Prepare the development environment and repository.

## Tasks

### Create Repository Structure

/livewell-rx
  /mobile
  /backend
  /database
  /api
  /docs

---

### Initialize Mobile App

Use Expo:

npx create-expo-app mobile

Install dependencies:

expo install react-navigation
expo install axios
expo install firebase

---

### Initialize Backend

mkdir backend  
cd backend  

npm init -y  

Install dependencies:

npm install express cors body-parser jsonwebtoken bcrypt pg

---

### Database Setup

Create PostgreSQL database:

livewell_rx_db

---

### Deliverables

- Repository initialized
- Mobile app bootstrapped
- Backend server running
- Database connected

---

# Sprint 1 — Authentication System

## Objective
Allow patients to register and login securely.

---

## Database Tables

users

Fields:

- id
- phone
- email
- password_hash
- created_at

verification_codes

- id
- phone
- code
- expires_at

---

## Backend API

POST /auth/register

POST /auth/login

POST /auth/verify

POST /auth/reset-password

---

## Mobile Screens

- LoginScreen
- RegisterScreen
- VerificationScreen

---

## Windsurf Agent Task Prompt

Build a secure authentication system for a React Native pharmacy app using Node.js and PostgreSQL.

Features:
- user registration
- login
- SMS verification
- password reset

Create backend API endpoints and mobile screens.

---

## Deliverables

Users can create accounts and login.

---

# Sprint 2 — Patient Profile

## Objective
Allow patients to view and update their information.

---

## Database

patient_profiles

Fields:

- id
- user_id
- name
- date_of_birth
- address
- phone
- insurance_provider

---

## Backend API

GET /profile

PUT /profile

---

## Mobile Screens

ProfileScreen  
EditProfileScreen

---

## Agent Task

Generate backend endpoints and React Native screens for viewing and updating patient profile data.

---

## Deliverables

Patients can manage their profile.

---

# Sprint 3 — Prescription Data

## Objective
Allow patients to see their medications.

---

## Database

prescriptions

Fields:

- id
- patient_id
- drug_name
- dosage
- quantity
- refills_remaining
- last_fill_date
- prescribing_doctor

---

## Backend API

GET /prescriptions

GET /prescriptions/:id

---

## Mobile Screens

MedicationListScreen  
MedicationDetailScreen

---

## Deliverables

Patients can see medication list.

---

# Sprint 4 — Prescription Refill

## Objective
Allow patients to refill prescriptions.

---

## Database

refill_requests

Fields:

- id
- patient_id
- prescription_id
- status
- created_at

Statuses:

- pending
- approved
- denied

---

## Backend API

POST /refill-request

GET /refill-status

---

## Mobile

RefillButton  
RefillConfirmationScreen

---

## Deliverables

Patients can request refills.

---

# Sprint 5 — Doctor Refill Authorization

## Objective
Handle prescriptions with no refills remaining.

---

## Database

doctor_requests

Fields:

- id
- prescription_id
- doctor_contact
- status
- created_at

---

## Backend API

POST /refill-authorization

---

## Deliverables

System can request refill authorization from doctors.

---

# Sprint 6 — Delivery & Pickup

## Objective
Allow patients to select delivery or pickup.

---

## Database

delivery_orders

Fields:

- id
- patient_id
- delivery_type
- address
- delivery_status
- delivery_time

Delivery Types

- pickup
- delivery

---

## Backend API

POST /delivery-order

GET /delivery-status

---

## Mobile Screens

PickupSelectionScreen  
DeliverySelectionScreen

---

## Deliverables

Patients can choose pickup or delivery.

---

# Sprint 7 — Notifications

## Objective
Notify patients of updates.

---

## Technology

Firebase Cloud Messaging

---

## Events

- refill approved
- prescription ready
- delivery dispatched

---

## Agent Task

Integrate Firebase push notifications with backend triggers.

---

## Deliverables

Push notification system working.

---

# Sprint 8 — Secure Messaging

## Objective
Enable patient-pharmacist messaging.

---

## Database

messages

Fields

- id
- sender_id
- receiver_id
- message
- created_at

---

## Backend API

POST /messages

GET /messages

---

## Mobile

ChatScreen  
MessageThread

---

## Deliverables

Secure messaging implemented.

---

# Sprint 9 — Pharmacy Admin Dashboard

## Objective
Allow pharmacy staff to manage requests.

---

## Admin Features

- refill requests
- delivery orders
- patient messaging

---

## Admin API

GET /admin/refills

GET /admin/deliveries

GET /admin/messages

---

## Deliverables

Admin dashboard for pharmacy staff.

---

# Sprint 10 — Security & Deployment

## Objective
Prepare system for production.

---

## Security

- HIPAA compliant encryption
- Secure token authentication
- Audit logs

---

## Infrastructure

Deploy:

Backend → AWS  
Database → AWS RDS  
Mobile → iOS / Android builds

---

## Deliverables

Production-ready application.

---

# Post Launch Roadmap

Future Features:

- Telepharmacy video consultations
- Medication reminders
- Automatic refills
- Copay payments
- Family medication profiles
