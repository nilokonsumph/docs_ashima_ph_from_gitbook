# Payroll lock

Use Payroll Lock while payroll is being processed to pause employee submissions and manager approvals that could change payroll-sensitive source records.

**Navigation:**\
go to **Paycheck → Pay Run → Payroll Lock**.

## what does the lock cover?

The current page states that the lock prevents employees from submitting adjustments or filing requests for timesheets, leave, shift changes, and overtime. It also prevents managers from approving related To Do requests while payroll is being processed.

The page explicitly states that administrators are not blocked: administrators can still add or edit timesheets, file leave or overtime, and approve or reject requests during the locked period.

## which settings control this workflow?

| level            | setting or record                                    | effect                                                                                                          |
| ---------------- | ---------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| company / global | Payroll Lock state                                   | pauses the covered employee and manager actions for the account                                                 |
| module           | Hours, Leaves, Shifts, Overtime, and To Do workflows | enforce the lock on covered submissions and approvals                                                           |
| employee         | Not applicable as an override                        | the displayed lock is not configured per employee                                                               |
| pay run          | payroll processing timing                            | determines when an authorized admin chooses to lock or unlock; the page is not tied to one displayed Pay Run ID |

## how do you lock or unlock processing?

1. click **edit**.
2. change the **locked/unlocked** control to the required state.
3. review whether payroll processing is actually in progress and communicate the effect to employees and managers.
4. click **save**.
5. verify the displayed state and the **locked on** or **unlocked on** actor and timestamp.

Use **cancel** to leave edit mode without changing the state.

> \[!WARNING] This control does not prevent administrators from changing payroll-sensitive records. Administrators must still coordinate changes and recalculate affected open payroll before submission.

## related articles

* [pay run workspace and history](/broken/pages/1aae811cf00a844c563a72b274efd3a4f11bcde1)
* [review and recalculate a pay run](/broken/pages/4b2260817fafa8f67821e1a140643d4dd7a297ab)
* [workflow and manager access](file:///4659123/settings/workflow_and_manager_access.md)
