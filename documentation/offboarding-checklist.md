# NMG-0058 — Employee Offboarding Checklist

## Ticket Information

* **Ticket:** NMG-0058
* **Employee:** Sandra Torres
* **Employee ID:** NMG-0052
* **Department:** Human Resources
* **Position:** HR Specialist
* **Username:** `storres`
* **Offboarding Reason:** Voluntary separation

---

## Offboarding Checklist

| Task                                 | Status    | Verification                               |
| ------------------------------------ | --------- | ------------------------------------------ |
| Receive approved offboarding request | Completed | HR request documented                      |
| Identify employee account            | Completed | `storres` located in Active Directory      |
| Review account information           | Completed | Account, OU, groups, and status documented |
| Disable Active Directory account     | Completed | Account confirmed disabled                 |
| Review group memberships             | Completed | `HR-Users` and `Domain Users` reviewed     |
| Remove department-specific access    | Completed | Sandra removed from `HR-Users`             |
| Preserve business data               | Completed | Three fictional documents archived         |
| Verify original business data        | Completed | Original files remain intact               |
| Verify account and access changes    | Completed | AD and group membership verified           |
| Document actions                     | Completed | Supporting records created                 |
| Close offboarding ticket             | Completed | Final resolution documented                |

---

## Security Considerations

The offboarding process was performed in a controlled sequence to reduce the risk of unauthorized access.

The Active Directory account was disabled before access cleanup was completed. Department-specific access was then reviewed and removed while the account object and business data were retained for documentation and records purposes.

Only the employee's access was modified. Other authorized members of the `HR-Users` group were not affected.

---

## Verification Standard

Each major change followed the:

**Change → Verify → Document**

process.

This ensured that administrative changes were confirmed before the ticket was considered complete.

---

## Final Status

**Offboarding Process: Completed**

**Ticket NMG-0058: Closed**

**Environment:** Simulated Windows Server 2022 Active Directory lab

No production systems or real employee data were used.
