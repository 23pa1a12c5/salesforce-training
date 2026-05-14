# Day 3 – Salesforce Data Modeling

## 1. Difference Between App, Object, Record, and Field

| Term | Meaning | Example |
|------|---------|---------|
| App | A collection of tools, tabs, and features built for a specific business process | College Management App |
| Object | A database table that stores similar types of data | Student Object |
| Record | A single row inside an object | Student: Rahul Kumar |
| Field | A column that stores specific information about a record | Student Name, Roll Number |

### Simple Understanding

- App → Complete system
- Object → Table
- Record → Single entry in the table
- Field → Information about the entry

---

# 2. Standard vs Custom Objects

| Standard Objects | Custom Objects |
|------------------|----------------|
| Already provided by Salesforce | Created by developers/users |
| Used for common business processes | Used for organization-specific needs |
| Examples: Account, Contact, Opportunity | Examples: Student__c, Course__c |
| Cannot be deleted | Can be modified or deleted |

### Example

A college management system may use:

- Standard Object → Contact
- Custom Objects → Student, Faculty, Course

---

# 3. College Data Model

## Objects Used

### Custom Objects

1. Student
2. Course
3. Faculty
4. Department
5. Enrollment

---

## Relationships

| Object 1 | Relationship | Object 2 |
|----------|-------------|-----------|
| Student | Enrolls In | Course |
| Faculty | Teaches | Course |
| Department | Contains | Faculty |
| Department | Contains | Course |
| Enrollment | Connects | Student and Course |

---

## Data Model Diagram

```text
Department
   |
   |---- Faculty
   |
   |---- Course
            |
            |
        Enrollment
         /      \
        /        \
   Student ---- Course
