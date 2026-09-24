# NMG-0058 — Security Analysis

## Overview

This document analyzes the security considerations involved in the simulated employee offboarding process for Sandra Torres.

The goal of the offboarding process was to prevent continued access after separation while preserving required business information and avoiding unnecessary changes to other users.

---

## 1. Risk of Leaving the Account Enabled

An enabled employee account can potentially be used to authenticate to organizational resources.

If a separated employee's credentials remained active, the organization could face risks such as:

* Unauthorized domain authentication
* Access to internal applications
* Access to shared resources
* Unauthorized use of existing permissions
* Potential misuse of organizational data

For this reason, disabling the Active Directory account was one of the first access-control actions performed.

---

## 2. Disable vs. Delete

The account was **disabled rather than deleted**.

Disabling the account prevents authentication while preserving the account object for administrative purposes.

Deleting the account immediately would remove the identity object and could make investigation, documentation, or recovery more difficult.

The simulated workflow therefore retained the account while preventing authentication.

---

## 3. Group Membership and Least Privilege

Sandra Torres was originally a member of:

* `HR-Users`
* `Domain Users`

The `HR-Users` group represented department-specific access in the simulated environment.

Sandra was removed from `HR-Users` while other authorized members remained in the group.

The `Domain Users` membership was reviewed and left unchanged as part of this simulated workflow.

This demonstrates the principle of **least privilege**: access should be limited to what is necessary and should be removed when it is no longer required.

---

## 4. Why Access Removal Requires Review

A group name alone does not necessarily explain every permission associated with that group.

Before removing access in a production environment, an administrator should understand what resources the group controls and determine whether additional access exists through:

* Other security groups
* File and folder permissions
* Application accounts
* VPN access
* Cloud services
* Email systems
* Remote access solutions
* Privileged roles

The simulated project focused on Active Directory and department-specific group membership rather than attempting to reproduce every enterprise system.

---

## 5. Business Data Preservation

Removing access does not mean deleting business data.

The employee's simulated business documents were copied to an HR records archive while the original files were retained.

This demonstrates two separate administrative responsibilities:

**Identity and Access:** Prevent unauthorized access.

**Data Management:** Preserve organizational information according to applicable retention and business requirements.

---

## 6. Verification

The offboarding process followed a:

**Change → Verify → Document**

approach.

Verification included:

* Confirming the AD account was disabled.
* Confirming Sandra was removed from `HR-Users`.
* Confirming other `HR-Users` members were not affected.
* Confirming the archived documents existed.
* Confirming the original documents remained intact.

---

## 7. Security Workflow

The simulated offboarding workflow can be summarized as:

**HR Request**
↓
**Identity Verification**
↓
**AD Investigation**
↓
**Account Disablement**
↓
**Access Review**
↓
**Department Access Removal**
↓
**Data Preservation**
↓
**Verification**
↓
**Documentation & Closure**

---

## 8. Security Lessons Learned

This project reinforced several practical IAM and Help Desk concepts:

* Employee lifecycle management
* Identity verification
* Active Directory account administration
* Security group management
* Least privilege
* Access removal
* Business data preservation
* Change verification
* Security-conscious documentation

The exercise also demonstrated that employee offboarding is a process rather than a single administrative action.

---

## Environment

This project was completed in a simulated Windows Server 2022 Active Directory environment running in VirtualBox.

Northstar Medical Group and Sandra Torres are fictional.

No production systems, real employee accounts, passwords, or confidential organizational data were used.
