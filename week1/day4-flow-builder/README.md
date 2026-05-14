# Day 4 – Salesforce Flow Builder

## 1. What is Flow Builder?

Flow Builder is a no-code/low-code automation tool in Salesforce used to automate business processes. It helps organizations reduce manual work by creating workflows using drag-and-drop elements instead of writing code.

Using Flow Builder, businesses can:

- Automate repetitive tasks
- Update records automatically
- Send notifications and emails
- Guide users through screens
- Improve productivity and consistency

Flow Builder is widely used in enterprise systems because it allows automation without requiring advanced programming knowledge.

---

# 2. Types of Flows

Salesforce provides different types of flows for different business needs.

## Screen Flow

A Screen Flow interacts directly with users by displaying screens where users can enter or view information.

### Features

- User interaction required
- Contains forms, buttons, and screens
- Used for guided business processes

### Example

Student Admission Form:
- User enters student details
- Flow validates information
- Record gets created automatically

### Real-World Use Cases

- Customer feedback forms
- Loan application forms
- Employee onboarding forms

---

## Record Triggered Flow

A Record Triggered Flow runs automatically when a record is created, updated, or deleted.

### Features

- Fully automated
- No user interaction needed
- Executes in the background

### Example

When a student’s fee payment status changes to "Paid":
- Automatically send confirmation email
- Update payment status
- Notify the accounts department

### Real-World Use Cases

- Automatic approval processes
- Auto email notifications
- Updating related records

---

# 3. My Automation Ideas

## 1. Student Admission Automation

When a new student record is created:
- Generate student ID automatically
- Send welcome email
- Assign department

---

## 2. Attendance Alert System

If attendance drops below 75%:
- Send warning email to student
- Notify faculty advisor

---

## 3. Fee Payment Reminder

Automatically send reminders:
- 7 days before due date
- On due date
- After overdue

---

## 4. Leave Approval Process

When a leave request is submitted:
- Notify manager/faculty
- Update leave status automatically
- Send approval/rejection notification

---

## 5. Course Enrollment Automation

When a student enrolls in a course:
- Update seat count
- Generate enrollment confirmation
- Notify faculty

---

# 4. Flow Diagram

## Example Flow: Student Admission Process

```text
Start
  |
  v
Student submits admission form
  |
  v
Validate student details
  |
  v
Create Student Record
  |
  v
Generate Student ID
  |
  v
Send Welcome Email
  |
  v
Assign Department
  |
  v
End
