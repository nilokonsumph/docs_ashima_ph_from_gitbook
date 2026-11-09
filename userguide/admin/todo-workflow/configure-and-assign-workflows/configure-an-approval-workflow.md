# configure an approval Workflow

## configure an approval Workflow

create a Workflow when the current approvers or approval order do not fit a supported process. the Workflow defines routing; the source module still defines what is being approved.

**Navigation:**\
go to **Settings → Workflow**, then select the process you need to configure.

### choose the Workflow model for the process

Workflows do not all use the same scope. first identify whether the process has one company-wide route, employee-specific routing, or the optional Leave-type routing.

| Workflow model      | processes and examples                                                                                                        | how it works                                                                                                | when to use it                                                                         |
| ------------------- | ----------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| company-wide        | **Payroll**, **Termination**, **Disbursement**, **13th Month**, **End of Year**, and **Document**                             | the company uses one current approval route for that process; employees are not assigned individually       | when every submitted batch or company-level record must follow the same approval chain |
| employee-scoped     | **Timesheet Adjustment**, **Overtime**, **Shifts**, **Leave**, **Maternity Benefits**, and other supported employee processes | administrators can create several Workflows for the same process and assign different employees to each one | when teams, locations, payroll groups, or operating units need different approvers     |
| Leave-type-specific | individual Leave types when advanced Leave Workflow is enabled                                                                | the approval route can be assigned at the Leave-type level instead of using one general Leave route         | when different Leave policies require different approvers or approval levels           |

for a company-wide process, creating another active Workflow changes the current company-wide route; it does not create employee-level routing. review requests already pending under the previous route before making the new route operational.

for an employee-scoped process, creating a Workflow is only the first step. assign the intended employees to it, then verify their active assignment. employees not moved to the new Workflow continue to use their applicable existing or default route.

advanced Leave-type routing appears only when the company option is enabled. when it is not enabled, Leave uses the standard employee-scoped Leave Workflow.

### understand the default Workflow

Ashima provides a default Workflow for a supported process so requests always have a starting approval route. it begins with one approval level and the account's root owner as the approver.

the default Workflow cannot be deleted, and its **Approval Levels** value is fixed at one. it is not completely read-only: an administrator with Workflow edit privilege can update its name, the approver or approvers at level one, and **Notify Staff**. keep a valid level-one approver because the default route is the fallback when no applicable custom assignment is available.

{% hint style="warning" %}
**important:** do not use the default Workflow as an unreviewed catch-all. confirm its current approver and notification setting whenever administrators, employee assignments, or approval responsibilities change.
{% endhint %}

### choose the approval structure

| choice                            | effect                                                                               |
| --------------------------------- | ------------------------------------------------------------------------------------ |
| Workflow name                     | identifies the approval group in lists and employee assignments                      |
| **Approval Levels**               | sets one to five sequential decision stages for a custom Workflow                    |
| approvers at a level              | places one or more alternate authorized approvers at the same stage                  |
| **Send Notifications via: Email** | shows the supported notification channel for the Workflow                            |
| **Notify Staff**                  | sends the supported email notification after the application is approved or rejected |

one level is suitable when one decision stage is enough. use multiple levels when the request must pass through distinct stages in order—for example, a team review at level one followed by payroll authorization at level two.

add multiple approvers to the same level when more than one person should be able to act at that stage. this provides operational cover when an approver is unavailable. any authorized approver at the current level can complete that level; Ashima does not wait for every same-level approver. after one approver completes the level, the request moves to the next configured level or reaches final approval.

each active level requires at least one approver, and the same approver cannot be selected more than once in one Workflow. levels beyond the current level cannot decide the request early.

notifications communicate the result; they do not replace the saved approval record. verify the decision and source-module status in Ashima even when an email was sent.

### create a Workflow

1. select the process under **Settings → Workflow**.
2. select **Create new**.
3. enter a clear Workflow name that identifies its scope or approver group.
4. choose the number of **Approval Levels**, from one to five.
5. add at least one approver to each required level.
6. enable **Notify Staff** when staff should receive the supported notification after the application is approved or rejected.
7. review the level order and approvers.
8. select **Create workflow**.
9. reopen the saved Workflow and verify its name, levels, approvers, and notification setting.

the list identifies the default Workflow, approval-level count, approvers, notification state, creator, dates, and last update. the default Workflow is protected from deletion.

{% hint style="warning" %}
**important:** create or update routing before users submit the requests that should follow it. changing the current configuration does not prove that pending requests were safely moved to the new routing.
{% endhint %}

### update or delete a Workflow

open a custom Workflow to change its name, approval levels, approvers, or notification setting. the default Workflow keeps one approval level but permits the supported name, level-one approver, and notification changes when you have edit privilege. before reducing levels or deleting a non-default Workflow, review employee assignments and pending requests. Ashima blocks or limits changes where the active assignment or pending-request state would become invalid.

do not delete a Workflow merely to fix one employee's routing. reassign the employee to the correct compatible Workflow and verify the saved assignment.

### replace an approver who leaves the company

if an approver resigns or is terminated, review their Workflow assignments as part of the employee-status change. Changing the person's status to **Inactive** or **End of Employment** does not move their approval levels to the default Workflow or its approver. Requests already waiting for approval do not automatically restart under the default route.

when Ashima shows the Workflows affected by the status change, choose an active replacement for each listed approval level and submit the reassignment. Then reopen **Settings → Workflow** to check the saved approvers, and check pending **Todo** requests to make sure the replacement can act on them. If the status was changed without completing reassignment, update those Workflow levels immediately.

{% hint style="warning" %}
**important:** do not assume that adding a replacement has cleared every pending request. Check the requests that were already waiting for the departing approver.
{% endhint %}

For the status-change steps and pending-work checks, see [handle locked and changed approval work](../review-approval-work/handle-locked-and-changed-approval-work.md#what-happens-if-an-approver-resigns-or-becomes-inactive).
