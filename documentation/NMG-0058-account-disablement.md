# NMG-0058 — Account Disablement Record

## Employee Information

* **Employee:** Sandra Torres
* **Employee ID:** NMG-0052
* **Department:** Human Resources
* **Position:** HR Specialist
* **Username:** `storres`
* **Domain:** `NMG.com`
* **Organizational Unit:** `HR`

## Previous Account State

Before the change, Sandra Torres' Active Directory account was enabled.

| Attribute           | Before Change              |
| ------------------- | -------------------------- |
| Account Status      | Enabled                    |
| Organizational Unit | HR                         |
| Group Membership    | `HR-Users`, `Domain Users` |

## Action Performed

The Active Directory account for `storres` was disabled using Active Directory Users and Computers.

The account was disabled from:

```text
NMG.com → HR → Sandra Torres
```
<img width="944" height="848" alt="Sandra_Torres_Account_is_Disable" src="https://github.com/user-attachments/assets/d198f006-40a0-44fe-a750-a0d7633c1ea0" />

The account object was retained and was not deleted.

## Reason for Change

The account was disabled to prevent the former employee from authenticating to the domain following the approved offboarding request.

The account was not deleted because additional offboarding activities, including access review, data preservation, verification, and documentation, remained to be completed.

## Verification

The account status was verified after the change.

The ADUC context menu displayed **Enable Account**, confirming that the account was disabled.

The employee's group memberships were not removed during this step because access review and group cleanup were handled separately.

## Resulting Account State

```text
Account:        Disabled
Username:       storres
OU:             HR

Groups:
    HR-Users
    Domain Users
```

## Next Action

Review the employee's group memberships and remove appropriate department-specific access as part of the offboarding process.

## Environment

This change was performed in a simulated Windows Server 2022 Active Directory environment running in VirtualBox.

No production systems or real employee data were used.
