# NMG-0058 — Offboarding Resolution

## Ticket Information

* **Ticket:** NMG-0058
* **Employee:** Sandra Torres
* **Employee ID:** NMG-0052
* **Department:** Human Resources
* **Position:** HR Specialist
* **Username:** `storres`
* **Offboarding Reason:** Voluntary separation

---

## Resolution Summary

Completed the simulated employee offboarding process for Sandra Torres.

The employee's Active Directory account was disabled to prevent authentication. The account was retained rather than deleted to preserve the identity object for documentation and continued offboarding activities.

The employee was removed from the `HR-Users` security group after reviewing the account's group membership. Other users in the group were not affected.

Membership in the standard `Domain Users` group was reviewed and left unchanged as part of the simulated workflow.

Three fictional business documents were preserved by copying them from the employee's original HR data location to the simulated HR records archive.

---

## Verification

The following items were verified:

* AD account is disabled.
* Sandra Torres is no longer a member of `HR-Users`.
* `Domain Users` membership remains unchanged.
* Three business documents exist in the HR records archive.
* Original business documents remain intact.
* No other `HR-Users` members were affected.

<img width="921" height="892" alt="Sandra_Membership_After_Access_is_Removed" src="https://github.com/user-attachments/assets/ffe29655-f222-4ed9-a43c-74fe88ad9b4f" />

---

## Outcome

The simulated offboarding process was completed successfully.

**Ticket Status: Closed**

---

## Documentation

Supporting documentation includes:

* Offboarding ticket
* AD investigation notes
* Account disablement record
* Offboarding checklist
* Final verification record
* Simulated business-data preservation evidence
* Security analysis
* Screenshots of relevant AD and file-management steps

---

## Environment

This project was completed in a simulated Northstar Medical Group lab environment using Windows Server 2022 and Active Directory Domain Services.

No production systems or real employee data were used.
