# Business Process Management — BPMN Assignments

## Student Details

**Name:** Vinay Kartheek Bathala  
**Register No:** RA2411026010953 & AD2  
**Programme:** B.Tech – CSE (AI & ML)  
**Department:** Department of CSE  
**Institution:** SRMIST Kattankulathur  
**Course:** Workflow Automation Engineering  
**Faculty:** Dr. C. Muralidharan (102832)  
**Academic Year:** 2026–2027  

---

## Week 1 — BPMN Process Modeling

### Scenario 1 — Hotel Room Reservation
**File:** `hotel_room_reservation.bpmn`

Flow:
`Booking Request → Check Availability → Available? → Payment → Payment Successful? → Confirm Booking → Send Confirmation → End`

Alternative paths:
- Room unavailable → Notify Guest → End
- Payment failed → Notify Guest → End

### Scenario 2 — Loan Application Processing
**File:** `loan_application_processing.bpmn`

Flow:
`Loan Application → Verify Documents & Credit Score → Documents Valid? → Check Eligibility → Eligible? → Loan Officer Approval → Disburse Loan → Send Notification → End`

Alternative paths:
- Invalid documents → Reject → Notify Customer → End
- Not eligible → Reject → Notify Customer → End
- Loan rejected → Notify Customer → End

### Scenario 3 — Job Applicant Recruitment
**File:** `job_applicant_recruitment.bpmn`

Flow:
`Job Application → Eligibility Screening → Eligible? → Technical Interview → Pass? → HR/Managerial Round → Selected? → Generate Offer Letter → Send Offer → End`

Alternative paths:
- Not eligible → Reject → End
- Technical interview failed → Reject → End
- HR round rejected → Reject → End

---

## Week 2 — BPMN Process Modeling

### Scenario 1 — Employee Leave Approval
**File:** `scenario1_employee_leave_approval.bpmn`

Flow:
`Leave Request → Check Leave Balance → Sufficient? → Manager Approval → Approved? → Update Balance → Send Notification → End`

Alternative paths:
- Insufficient balance → Notify Employee → End
- Manager rejected → Notify Employee → End

### Scenario 2 — Online Purchase Order Processing
**File:** `scenario2_online_purchase_order.bpmn`

Flow:
`Place Order → Check Availability → Available? → Process Payment → Payment Successful? → Confirm Order → Prepare Shipment → Ship Order → Send Confirmation → End`

Alternative paths:
- Out of stock → Notify Customer → End
- Payment failed → Notify Customer → End

### Scenario 3 — IT Service Request Handling
**File:** `scenario3_it_service_request.bpmn`

Flow:
`Report Problem → Submit Request → Register Request → Check Severity → Severity Level → Assign Technician → Investigate Problem → Resolvable Internally?`

Alternative paths:
- Low severity → Support Technician
- High severity → Senior Technician
- Resolvable → Fix Problem
- Not resolvable → Escalate to External Provider

Final flow:
`Update Request Status → Send Resolution Notification → End`

---

## BPMN Elements Used

- **Start Event** — Beginning of the process
- **End Event** — End of the process
- **User Task** — Work performed by a user
- **Service Task** — Automated/system activity
- **Send Task** — Sends a notification/message
- **Exclusive Gateway (XOR)** — Selects one path based on a condition
- **Sequence Flow** — Shows the process flow

---

## Repository Structure

```text
bpmn-assignment/
├── README.md
├── hotel_room_reservation.bpmn
├── loan_application_processing.bpmn
├── job_applicant_recruitment.bpmn
├── scenario1_employee_leave_approval.bpmn
├── scenario2_online_purchase_order.bpmn
└── scenario3_it_service_request.bpmn
