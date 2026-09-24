# NMG-0058 — Active Directory Investigation Notes

## Ticket Information

* **Ticket:** NMG-0058
* **Employee:** Sandra Torres
* **Employee ID:** NMG-0052
* **Department:** Human Resources
* **Position:** HR Specialist
* **Offboarding Reason:** Voluntary separation

## Active Directory Account

The employee's Active Directory account was located and reviewed in the Northstar Medical Group lab environment.

| Attribute           | Finding                          |
| ------------------- | -------------------------------- |
| First Name          | Sandra                           |
| Last Name           | Torres                           |
| Display Name        | Sandra Torres                    |
| Username            | `storres`                        |
| Email               | `storres@NMG.com`                |
| Domain              | `NMG.com`                        |
| Organizational Unit | HR                               |
| Account Status      | Enabled at time of investigation |
| Password Setting    | Never Expires                    |
| Group Membership    | `HR-Users`, `Domain Users`       |

## Investigation Findings

The correct employee account was identified in the `HR` Organizational Unit.

The account was enabled at the time of investigation and had membership in both the department-specific `HR-Users` security group and the standard `Domain Users` group.

The account information was documented before making any changes.

## Security Considerations

The account required security action because the employee was being offboarded.

The investigation confirmed the account identity and existing access before changes were made.

The account was not deleted during the initial investigation because additional offboarding activities remained to be completed.

## Initial Account State

```text
Account:        Enabled
OU:             HR
Username:       storres
Groups:
    HR-Users
    Domain Users
```

## Next Action

Disable the Active Directory account and verify the account state before proceeding with additional access-removal activities.

## Environment

This investigation was completed in a simulated Windows Server 2022 Active Directory environment running in VirtualBox.

No production systems or real employee data were used.
