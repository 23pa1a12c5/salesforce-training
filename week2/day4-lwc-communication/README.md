# Day 4 – LWC Communication

## 1. Component Communication

Component communication in LWC is used to share data between components.

There are mainly three types of communication:

- Parent to Child
- Child to Parent
- Unrelated Components Communication

This helps components work together and exchange information efficiently.

---

# Parent to Child Communication

Parent components send data to child components using properties.

### Example
- Parent component sends student details
- Child component displays student information

---

# Child to Parent Communication

Child components communicate with parent components using events.

### Example
- Child component sends button click event
- Parent component updates dashboard

---

# Unrelated Components Communication

Components without direct relationship communicate using:
- Pub/Sub
- Lightning Message Service (LMS)

### Example
- Attendance component updates dashboard component

---

# 2. Dashboard Design

## College Management Dashboard

The dashboard contains:
- Student Details Section
- Attendance Tracker
- Course Enrollment Summary
- Fee Payment Status
- Notifications Panel

---

# Dashboard Features

- Real-time updates
- Interactive UI
- Quick navigation
- Data visualization
- Automated alerts

---

# Example Dashboard Layout

```text
-----------------------------------
| Student Dashboard              |
-----------------------------------
| Attendance | Courses | Fees    |
-----------------------------------
| Notifications and Alerts       |
-----------------------------------
```

---

# 3. Data Flow Explanation

The system data flow works as follows:

1. User enters data through LWC forms
2. LWC sends data to Apex controller
3. Apex processes business logic
4. Salesforce database stores records
5. Updated data is returned to LWC
6. Dashboard displays latest information

---

# Simple Data Flow Diagram

```text
User Interface (LWC)
        |
        v
Apex Controller
        |
        v
Salesforce Database
        |
        v
Updated Dashboard
```

---

# 4. Aura vs LWC

| Aura Components | Lightning Web Components (LWC) |
|-----------------|-------------------------------|
| Older framework | Modern framework |
| Less performance | Faster performance |
| Uses Aura syntax | Uses standard web technologies |
| More complex | Simpler and lightweight |
| Event-based architecture | Modern JavaScript architecture |
| Slower rendering | Faster rendering |

---

# Why LWC is Preferred

Salesforce prefers LWC because it:
- Improves performance
- Uses modern web standards
- Simplifies development
- Creates reusable components
- Provides better user experience

---

# 5. Reflection

Today I learned how Lightning Web Components communicate with each other and how dashboards are designed in Salesforce applications.

I understood:
- Parent-child communication
- Event handling
- Data flow between frontend and backend
- Difference between Aura and LWC

The most interesting topic was learning how components interact dynamically to create responsive applications.
