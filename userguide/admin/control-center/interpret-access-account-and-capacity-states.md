# interpret access, account, and capacity states

use this reference when a person appears in Control Center but still cannot complete a task.

## read the access layers in order

use this table to identify the access layer that controls the missing company, page, employee, or action.

| layer                       | what it controls                                                                                                                     | it does not replace                                                     |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------- |
| account state               | whether the administrator account is enabled and usable                                                                              | invitation completion or permissions                                    |
| invitation state            | whether the invited person has completed account setup                                                                               | enabled state or assigned permissions                                   |
| company selection           | which businesses are included in an ordinary administrator's access arrangement                                                      | owner or designated-admin access rules                                  |
| role label                  | a short label for identifying the administrator's responsibilities                                                                   | page access or detailed permissions                                     |
| page and action permissions | **Available Roles** and **Selected Roles** control the pages and actions assigned to the administrator, regardless of the role label | company access, confidentiality, employee scope, or approval assignment |
| confidentiality rule        | confidential, non-confidential, or both employee populations                                                                         | company assignment or my team scope                                     |
| Admin My Team Access        | whether an eligible administrator can use the my team path                                                                           | which employees and actions are available                               |
| Manager Privileges          | employee populations and manager-facing actions                                                                                      | Admin-portal role privileges                                            |
| Workflow                    | who approves a request and in what order                                                                                             | visibility or module permission                                         |
| support access              | temporary Ashima support access and its level                                                                                        | an ordinary administrator role                                          |

check the narrow missing layer rather than assigning a broader role.

## interpret invitation and enabled states

assigning a role does not itself prove that an administrator has received or completed an invitation. resending an invitation does not enable a disabled account. after any change, confirm the person's invitation status, enabled state, named role, companies, and required access layers separately.

## interpret available slots

**available slots** shows the remaining account capacity after counted employee and administrator records are deducted from the plan limit. a positive number means capacity remains; zero means the account has reached the displayed limit.

## interpret audit records

where an **Audit Trail** is available, use it to confirm who changed a setting and when. then verify the affected function using the intended account and company.

***
