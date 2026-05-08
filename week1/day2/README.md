# Salesforce Summer Program – Day 2

---

# 1. What is Salesforce Platform?

The Salesforce Platform is a cloud-based platform that helps businesses build applications, manage customer data, automate workflows, and improve business processes.

It provides tools for:

- Customer Relationship Management (CRM)
- Application development
- Data management
- Automation
- Reporting and analytics
- Security and user management

Salesforce allows users to create customized business solutions using both configuration and coding.

---

# 2. How CRM Fits into Salesforce Platform

CRM concepts are managed in Salesforce using Objects and Apps.

| CRM Concept | Salesforce Representation |
|-------------|--------------------------|
| Company | Account Object |
| Customer | Contact Object |
| Sales Deal | Opportunity Object |

These objects are organized inside Salesforce Apps to help businesses manage customer relationships efficiently.

---

# 3. Important Salesforce Components

## App

An **App** in Salesforce is a collection of tabs, objects, and features designed for a specific business purpose.

### Example:
- Sales App
- Service App
- Recruitment App

---

## Object

An **Object** is a database table used to store data in Salesforce.

### Types of Objects:
- Standard Objects
- Custom Objects

### Examples:
- Account
- Contact
- Opportunity

---

## Tab

A **Tab** is a user interface element that helps users access objects, records, dashboards, and other features easily.

Tabs improve navigation inside Salesforce applications.

---

# 4. Difference Between Configuration and Coding

| Configuration | Coding |
|---------------|--------|
| Done using clicks and settings | Done using programming |
| No coding knowledge required | Requires coding knowledge |
| Faster to implement | Takes more development time |
| Uses Flow and Process Builder | Uses Apex and Lightning Web Components |
| Easier to maintain | More flexible and powerful |

---

## Examples of Configuration

1. Creating validation rules
2. Building workflows using Flow

---

## Examples of Coding

1. Writing Apex triggers
2. Developing Lightning Web Components (LWC)

---

# 5. My System Design

## App Name
**Sports Event Management App**

---

## Objects Used

| Object Name | Purpose |
|-------------|---------|
| Player | Stores player details |
| Organizer | Stores organizer information |
| Event | Stores sports event details |
| Registration | Stores participant registrations |

---

## User Interaction Flow

1. Organizer creates a sports event.
2. Players register for the event.
3. Registration details are stored in Salesforce.
4. Organizers track participants and event status.
5. Reports are generated for event analysis.
