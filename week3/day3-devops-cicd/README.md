# Day 3 – DevOps and CI/CD

## What is CI/CD?

CI/CD stands for Continuous Integration and Continuous Deployment.

It is a modern software development process where:
- Developers continuously integrate code changes
- Automated testing is performed
- Applications are deployed efficiently and reliably

CI/CD helps teams deliver updates faster with fewer errors.

---

# Continuous Integration (CI)

Continuous Integration means developers regularly merge code changes into a shared repository.

CI helps:
- Detect errors early
- Improve code quality
- Reduce integration issues
- Support team collaboration

---

# Continuous Deployment (CD)

Continuous Deployment automates the deployment process after testing is completed successfully.

CD helps:
- Deliver updates quickly
- Reduce manual deployment work
- Improve release reliability
- Support faster development cycles

---

# Why Deployment Workflow Matters

A proper deployment workflow is important because enterprise systems are large and complex.

Deployment workflows help:
- Prevent production errors
- Improve testing reliability
- Maintain system stability
- Reduce deployment failures
- Ensure smooth releases

Without structured workflows, deployments can become risky and difficult to manage.

---

# Problems Without Version Control

Without version control systems like GitHub, teams may face:
- Code conflicts
- Lost code changes
- Duplicate work
- Difficult rollback processes
- Poor collaboration
- Unstable deployments

Version control helps teams manage project history and collaborate efficiently.

---

# GitHub + DX + DevOps Explanation

## GitHub
GitHub stores and manages source code using version control.

---

## Salesforce DX
Salesforce DX supports source-driven Salesforce development using CLI tools and scratch orgs.

---

## DevOps
DevOps combines development and operations practices to improve software delivery and automation.

---

# How They Work Together

1. Developers write code in scratch orgs
2. Code is pushed to GitHub
3. Automated testing is performed
4. CI/CD pipeline validates changes
5. Deployment is done to higher environments
6. Final deployment reaches production

This workflow improves:
- Collaboration
- Automation
- Deployment reliability
- Code quality

---

# Enterprise Deployment Risks

Enterprise deployments may face risks such as:
- Failed deployments
- Data corruption
- Performance issues
- Automation conflicts
- Security vulnerabilities
- Downtime

Proper testing, governance, and CI/CD pipelines help reduce these risks.

---

# Enterprise Workflow Diagram

```text
Developer
    |
    v
Scratch Org
    |
    v
GitHub Repository
    |
    v
CI/CD Pipeline
    |
    v
Testing
    |
    v
Deployment
    |
    v
Production Environment
```

---

# Benefits of DevOps and CI/CD

- Faster releases
- Better collaboration
- Reliable deployments
- Improved testing
- Better version management
- Reduced deployment risks

---

# Reflection

Today I learned how CI/CD, DevOps, GitHub, and Salesforce DX work together in enterprise Salesforce development.

I understood:
- Importance of deployment workflows
- Why version control matters
- How CI/CD automates deployments
- Enterprise deployment risks
- How DevOps improves software delivery

The most interesting topic was understanding how modern enterprise systems use automated pipelines for reliable deployments.
