# Day 5 – Apex Introduction

## 1. What is Apex?

Apex is Salesforce’s programming language used to add custom business logic to applications running on the Salesforce platform.

It is similar to Java and is used when declarative tools like Flow Builder are not enough to handle complex requirements.

Using Apex, developers can:
- Automate advanced business processes
- Perform complex calculations
- Integrate Salesforce with external systems
- Create custom APIs and services
- Execute operations on large amounts of data

Apex runs securely on Salesforce servers and follows Salesforce platform rules and limits.

---

# 2. Difference Between Flow vs Apex

| Flow | Apex |
|------|------|
| No-code/low-code automation | Full programming language |
| Built using drag-and-drop | Written using code |
| Easier for admins/business users | Requires programming knowledge |
| Best for simple to medium automation | Best for complex logic |
| Faster development | More flexible and powerful |
| Limited customization | High customization possible |

---

# Difference Between Configuration vs Coding

| Configuration | Coding |
|---------------|--------|
| Uses clicks instead of code | Uses programming logic |
| Faster to implement | Takes more development time |
| Easier maintenance | Requires developer support |
| Limited flexibility | Highly flexible |
| Used for standard business processes | Used for advanced/custom requirements |

---

# 3. Real Examples Where Apex Is Needed

## 1. Complex Fee Calculation System

A university wants:
- Scholarship calculations
- Category-based discounts
- Late fee penalties
- Dynamic tax calculations

This logic becomes too complex for Flows alone, so Apex is used.

---

## 2. Integration with External Payment Gateway

When students pay fees online:
- Salesforce must connect with external banking APIs
- Validate transactions
- Store payment responses

Such integrations usually require Apex callouts.

---

## 3. Bulk Student Data Processing

Suppose the college imports:
- 50,000 student records
- Attendance updates
- Exam results

Apex batch processing is needed for handling large-scale operations efficiently.

---

# 4. Integrated System Design – College Management System

## CRM Purpose

The College Management CRM helps manage:
- Student records
- Faculty records
- Courses
- Admissions
- Attendance
- Fee management
- Notifications

---

# Objects Used

| Object | Purpose |
|--------|---------|
| Student | Stores student details |
| Faculty | Stores faculty details |
| Course | Stores course information |
| Department | Stores department data |
| Enrollment | Connects students and courses |
| Attendance | Tracks attendance |
| Fee Payment | Stores payment details |

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

# Validation Rules Used

## Example 1 – Student Age Validation

- Student age must be greater than 17.

Purpose:
- Prevent invalid admissions.

---

## Example 2 – Attendance Validation

- Attendance percentage cannot exceed 100%.

Purpose:
- Maintain accurate data.

---

# Flow Automation Used

## Admission Flow

When a student submits admission details:
- Create student record
- Generate ID
- Send confirmation email
- Assign department automatically

---

## Attendance Alert Flow

If attendance falls below 75%:
- Notify student
- Notify faculty advisor

---

# Apex Usage in System

## Fee Calculation Apex Logic

Apex calculates:
- Scholarships
- Late fees
- Discounts
- Taxes

because the logic is dynamic and complex.

---

## API Integration Apex

Apex integrates Salesforce with:
- Payment gateways
- SMS services
- Email systems

---

## Batch Processing Apex

Apex batches process:
- Large attendance uploads
- Result imports
- Mass student updates

---

# 5. Pseudocode Examples

## Example 1 – Attendance Alert

```text
IF attendance < 75%
    SEND warning email
    NOTIFY faculty advisor
END IF
