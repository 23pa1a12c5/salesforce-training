# Day 6 – Triggers and SOQL

## 1. What is SOQL?

SOQL (Salesforce Object Query Language) is a query language used in Salesforce to retrieve data from objects.

It is similar to SQL, but SOQL is specially designed for Salesforce data and relationships.

Using SOQL, developers can:
- Fetch records from objects
- Filter specific data
- Retrieve related records
- Sort and organize results
- Support automation and business logic

---

# Example Understanding

Suppose a college system wants:
- All students from the CSE department
- Students with attendance below 75%
- Courses taught by a particular faculty member

SOQL is used to retrieve this information from Salesforce.

---

# 2. What is an Apex Trigger?

An Apex Trigger is a piece of Apex code that automatically executes when specific events occur on Salesforce records.

Triggers react to actions such as:
- Insert
- Update
- Delete
- Undelete

Triggers help enterprise systems respond automatically to data changes.

---

# Example

When a student record is created:
- Automatically generate student ID
- Create login credentials
- Send welcome email

This automation can be handled using triggers.

---

# 3. Difference Between Flow vs Trigger

| Flow | Trigger |
|------|---------|
| Declarative automation | Programmatic automation |
| Built using drag-and-drop | Written using Apex code |
| Easier for admins | Requires developers |
| Good for simple automation | Better for complex logic |
| Faster to develop | More flexible and powerful |
| Limited customization | Advanced customization possible |

---

# Difference Between Before Trigger vs After Trigger

| Before Trigger | After Trigger |
|----------------|---------------|
| Executes before record is saved | Executes after record is saved |
| Used for validation/modification | Used for related operations |
| Faster because record not committed yet | Used when record ID is required |
| Can change field values directly | Often used for notifications/integrations |

---

# Example

## Before Trigger
Automatically set:
- Student status = "Active"

before saving the student record.

---

## After Trigger
After saving:
- Send confirmation email
- Create related attendance record

---

# 4. My Trigger Use Cases

## 1. Student Admission Trigger

When a student record is inserted:
- Generate unique student ID
- Assign default department

---

## 2. Attendance Warning Trigger

When attendance percentage becomes less than 75%:
- Send warning notification

---

## 3. Fee Payment Trigger

When payment status changes to "Paid":
- Generate payment receipt
- Send confirmation email

---

## 4. Course Enrollment Trigger

When a student enrolls in a course:
- Increase enrolled student count
- Notify faculty

---

## 5. Faculty Assignment Trigger

When a faculty member is assigned:
- Update course ownership
- Notify department head

---

# 5. Query Examples (English Ideas)

## Example 1

Get all students whose attendance is below 75%.

---

## Example 2

Find all courses offered by the Computer Science department.

---

## Example 3

Retrieve students who have not paid fees.

---

## Example 4

Get all faculty members teaching more than 3 courses.

---

## Example 5

Find students enrolled in the "Database Systems" course.

---

# 6. Reflection – Why Enterprise Systems React Automatically to Data Changes

Enterprise systems manage thousands or millions of records daily. Manual monitoring is impossible at large scale.

Automatic reactions help organizations:
- Respond instantly to events
- Maintain data consistency
- Improve efficiency
- Reduce manual work
- Enable real-time operations

Triggers and automation allow systems to behave intelligently whenever data changes occur.

For example:
- Banks detect transactions instantly
- E-commerce systems update inventory automatically
- Colleges generate alerts automatically

Modern enterprise systems are heavily event-driven.

---

# Reflective Questions

## 1. Why do systems need triggers?

Systems need triggers to automatically respond to data changes without requiring human intervention.

---

## 2. Difference between polling and event-driven systems?

| Polling System | Event-Driven System |
|----------------|--------------------|
| Continuously checks for changes | Reacts immediately to events |
| Less efficient | More efficient |
| Slower response | Real-time response |

---

## 3. Why are database queries important?

Queries help retrieve useful information from large datasets quickly and accurately.

Without queries, finding business information would be extremely difficult.

---

## 4. When should Flows be preferred over Triggers?

Flows should be preferred when:
- Automation is simple
- No coding is needed
- Faster implementation is required
- Business users need maintainability

---

## 5. What problems happen if automation logic becomes too complex?

Complex automation may cause:
- Difficult maintenance
- Performance issues
- Unexpected behavior
- Debugging challenges
- Automation conflicts

---

## 6. Why should developers think carefully before automating actions?

Poor automation design can:
- Create incorrect updates
- Cause data corruption
- Trigger infinite loops
- Reduce system performance

Automation should always follow proper business logic and planning.

---

# End of Day Learning Outcome

After completing this activity, I understood:

- What SOQL is and why it is important
- How Apex Triggers work
- Difference between Flow and Trigger
- Difference between Before and After Triggers
- How enterprise systems react to events
- Why intelligent automation is important in business systems
