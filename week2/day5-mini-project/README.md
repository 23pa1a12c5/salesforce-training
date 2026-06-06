# Day 5 – Mini Project

## System Overview

The project is a College Management CRM System built using Salesforce technologies. The system helps manage student admissions, course enrollments, attendance tracking, fee payments, and notifications in a centralized platform.

The system improves automation, data management, and communication between students, faculty, and administrators.

---

# CRM Concepts

The CRM system manages:
- Student information
- Faculty details
- Course management
- Admissions process
- Attendance monitoring
- Fee management
- Notifications and alerts

The system helps maintain accurate records and automate business processes efficiently.

---

# Data Model

## Objects Used

| Object | Purpose |
|--------|---------|
| Student | Stores student details |
| Faculty | Stores faculty details |
| Course | Stores course information |
| Department | Stores department data |
| Enrollment | Connects students and courses |
| Attendance | Tracks attendance |
| Fee Payment | Stores payment information |

---

# Relationships

| Parent Object | Child Object | Relationship |
|---------------|--------------|--------------|
| Department | Faculty | One-to-Many |
| Department | Course | One-to-Many |
| Student | Enrollment | One-to-Many |
| Course | Enrollment | One-to-Many |
| Student | Attendance | One-to-Many |

---

# Validation Rules

## Student Age Validation
- Student age must be greater than 17.

## Attendance Validation
- Attendance percentage cannot exceed 100%.

## Fee Validation
- Fee amount cannot be negative.

Validation rules help maintain accurate and valid data in the system.

---

# Flows

## Admission Flow
- Validate admission form
- Create student record
- Generate student ID
- Send confirmation email

---

## Attendance Alert Flow
- Check attendance percentage
- Send warning notification below 75%
- Notify faculty advisor

---

## Fee Reminder Flow
- Send reminders before due date
- Notify students for pending payments

---

# Apex Logic

## Fee Calculation Logic
Apex calculates:
- Scholarships
- Discounts
- Late fee penalties
- Tax calculations

---

## Payment Gateway Integration
Apex integrates Salesforce with external payment systems to process student fee payments.

---

## Batch Processing
Batch Apex processes:
- Large attendance uploads
- Bulk student updates
- Exam result imports

---

# UI Screens

## Student Admission Screen
- Add student details
- Submit admission form

---

## Course Enrollment Screen
- Register for courses
- View enrollment details

---

## Attendance Dashboard
- Track attendance percentage
- Display attendance alerts

---

## Fee Payment Screen
- View fee details
- Make payments
- Download receipts

---

# Complete Data Flow

```text
Student Admission Form
        |
        v
Flow Validation
        |
        v
Student Record Created
        |
        v
Trigger Generates Student ID
        |
        v
Course Enrollment
        |
        v
Attendance Tracking
        |
        v
Fee Payment Processing
        |
        v
Reports and Dashboards
```

---

# Frontend and Backend Flow

| Frontend | Backend |
|----------|---------|
| LWC Components | Apex Logic |
| User Interface | Business Processing |
| Form Submission | Database Operations |
| Dashboard Display | Automation and Validation |

---

# Reflection

This mini project helped me understand how multiple Salesforce technologies work together in a real CRM system.

I learned:
- CRM architecture
- Data modeling
- Validation rules
- Flow automation
- Apex logic
- LWC frontend development
- End-to-end system workflow

The most interesting part was understanding how automation, frontend components, and backend logic combine to build scalable enterprise applications.
