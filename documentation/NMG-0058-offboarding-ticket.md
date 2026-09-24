# NMG-0058 — Employee Offboarding Ticket

## Ticket Information

* **Organization:** Northstar Medical Group
* **Ticket:** NMG-0058
* **Request Type:** Employee Offboarding
* **Priority:** High
* **Requester:** Human Resources
* **Employee:** Sandra Torres
* **Employee ID:** NMG-0052
* **Department:** Human Resources
* **Position:** HR Specialist
* **Username:** `storres`
* **Domain:** `NMG.com`
* **Offboarding Reason:** Voluntary separation

---

## Request

Human Resources notified IT that Sandra Torres is leaving Northstar Medical Group and requested completion of the employee offboarding process.

The IT team is responsible for:

1. Investigating the employee's identity and access.
2. Disabling the Active Directory account.
3. Reviewing and removing appropriate access.
4. Preserving required business data.
5. Verifying the completed changes.
6. Documenting and closing the ticket.

---

## Initial Security Considerations

The employee's account should be secured promptly following the approved offboarding request to prevent continued authentication or unauthorized access.

The account should be **disabled rather than deleted** during the initial offboarding process so that the identity object and associated information remain available for investigation, documentation, auditing, and continued access-management activities.

Access should be reviewed based on actual group membership and authorization rather than removed blindly.

Business data should be preserved according to organizational requirements and should not be deleted simply because the employee has separated from the organization.

---

## Planned Actions

* [x] Identify employee account
* [x] Investigate Active Directory account
* [x] Disable Active Directory account
* [x] Review group membership
* [x] Remove department-specific access
* [x] Preserve simulated business data
* [x] Verify completed changes
* [x] Document resolution
* [x] Close ticket

---

## Initial Status

**Status:** Open

**Next Action:** Investigate Sandra Torres' Active Directory account and document the employee's current identity and access information.

---

## Environment

This ticket is part of a simulated Help Desk/IAM lab environment.

* Windows Server 2022
* Active Directory Domain Services
* Active Directory Users and Computers
* VirtualBox

No production systems or real employee data were used.

