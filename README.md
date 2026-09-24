# Northstar Medical Group — Employee Offboarding & Access Management

## Project Overview

This project demonstrates a simulated IT Help Desk and Identity & Access Management (IAM) employee offboarding workflow using Windows Server 2022 and Active Directory Domain Services.

The scenario follows the offboarding of a fictional Northstar Medical Group employee and demonstrates how IT can securely remove an employee's access while preserving organizational business data.

The project was completed in a controlled VirtualBox lab environment.

---

## Scenario

**Organization:** Northstar Medical Group
**Employee:** Sandra Torres
**Employee ID:** NMG-0052
**Department:** Human Resources
**Position:** HR Specialist
**Username:** `storres`
**Offboarding Ticket:** NMG-0058
**Reason:** Voluntary separation

---

## Objectives

The objectives of this project were to:

* Investigate an employee's Active Directory account.
* Verify account and group membership information.
* Disable the employee's AD account.
* Remove department-specific access.
* Preserve simulated business data.
* Verify that access removal was successful.
* Document the complete offboarding workflow.
* Close the Help Desk offboarding ticket.

---

## Offboarding Workflow

```text
HR Offboarding Request
        ↓
Identify Employee
        ↓
Investigate AD Account
        ↓
Disable Account
        ↓
Review Group Membership
        ↓
Remove Department-Specific Access
        ↓
Preserve Business Data
        ↓
Verify Changes
        ↓
Document & Close Ticket
```

---

## Project Environment

* Windows Server 2022
* Active Directory Domain Services
* Active Directory Users and Computers
* VirtualBox
* Windows file system
* Simulated Help Desk ticketing workflow

---

## Project Tasks

### Day 1 — Offboarding Request

Created and documented Help Desk ticket `NMG-0058`.

Established the required offboarding workflow and identified the information required before making changes.

### Day 2 — Active Directory Investigation

Located Sandra Torres' Active Directory account and documented:

* Username
* Domain
* Organizational Unit
* Account status
* Group membership
* Password settings
* Account information

### Day 3 — Account Disablement

Disabled the `storres` Active Directory account.

The account object was retained rather than deleted to support continued documentation and offboarding activities.

### Day 4 — Access Removal

Reviewed Sandra's group memberships.

Removed Sandra from the department-specific `HR-Users` security group while leaving the standard `Domain Users` membership unchanged.

Verified that Sandra was no longer listed as a member of `HR-Users`.

### Day 5 — Business Data Preservation

Created a simulated HR employee-data location and preserved three fictional business documents in a simulated HR records archive.

The original files were intentionally retained.

### Day 6 — Final Verification

Verified:

* AD account remained disabled.
* Sandra was no longer a member of `HR-Users`.
* `Domain Users` membership remained unchanged.
* Archived business data was present.
* Original business data remained intact.

### Day 7 — Documentation & Closure

Completed the final resolution documentation and closed the simulated Help Desk offboarding ticket.

---

## Key Skills Demonstrated

### Active Directory

* User account administration
* Organizational Units
* Security groups
* Group membership management
* Account disablement
* Employee lifecycle management

### Help Desk

* Ticket creation
* Investigation
* Change management
* Verification
* Resolution documentation
* Ticket closure

### IAM & Security

* Identity lifecycle management
* Access removal
* Least-privilege concepts
* Security group administration
* Access verification
* Business-data preservation

### Documentation

* Investigation notes
* Change records
* Verification checklists
* Resolution documentation
* Security analysis

---

## Project Documentation

### Documentation

* [Offboarding Ticket](documentation/NMG-0058-offboarding-ticket.md)
* [AD Investigation Notes](documentation/NMG-0058-investigation-notes.md)
* [Account Disablement Record](documentation/NMG-0058-account-disablement.md)
* [Offboarding Checklist](documentation/offboarding-checklist.md)
* [Final Resolution](documentation/NMG-0058-resolution.md)

### Data Preservation

* [Data Preservation Notes](data-preservation/data-preservation-notes.md)

### Security

* [Security Analysis](security/security-analysis.md)

### Screenshots

Screenshots documenting the lab procedures are stored in the `screenshots/` directory.

---

## Security & Privacy

This project is a simulated lab environment.

Northstar Medical Group is a fictional organization, and Sandra Torres is a fictional employee created for this exercise.

No production systems, real employee accounts, passwords, confidential business information, or real organizational data were used.

All procedures were performed in a controlled personal VirtualBox environment.

---

## What This Project Demonstrates

This project demonstrates the complete simulated employee offboarding lifecycle:

**Investigate → Disable → Remove Access → Preserve Data → Verify → Document → Close**

The focus is on practical Active Directory administration, Help Desk workflow, identity and access management fundamentals, and security-conscious documentation.

