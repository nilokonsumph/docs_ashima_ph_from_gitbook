# understand which employees and actions you can access

your administrator can define your team using either or both of these scopes:

| scope              | who can be included                                       | important detail                                                                        |
| ------------------ | --------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| **Direct Reports** | employees whose **Reports To** relationship points to you | your administrator can include additional reporting levels, up to three levels in total |
| **Department**     | employees assigned to selected departments                | the administrator chooses the departments and the functions allowed for this scope      |

when both scopes are enabled, your visible team can include employees from either scope. the actions allowed for Direct Reports can differ from the actions allowed for Department employees.

## can i see the employees who report to my direct reports?

yes, when your administrator enables the additional reporting levels. the levels are counted from you:

| enabled depth | employees who can be included                                                   |
| ------------- | ------------------------------------------------------------------------------- |
| one level     | employees who report directly to you                                            |
| two levels    | your direct reports, plus the employees who report to them                      |
| three levels  | those first two levels, plus employees who report to people at the second level |

for example, if a supervisor reports to you and a team leader reports to that supervisor, the supervisor is at your first level and the team leader is at your second. employees reporting to that team leader are at your third level.

the employee's **Reports To** relationship connects these levels. adding a reporting level to the organization does not by itself expand your access; your administrator must enable the corresponding depth. if you need to review a team beyond the level available to you, ask the administrator to check your reporting depth and the employees' **Reports To** assignments.

## can my access differ between teams?

for example, you may be allowed to view timesheets for a department but edit timesheets only for **Direct Reports**. you may see an employee in the directory but have no access to that employee's leave balance or personal details.

managers cannot change their own scope or grant themselves functions. the administrator owns these controls under **Settings → Workflow → Manager Access Settings**. see [configure manager and Admin My Team access](../../../admin/settings/platform-controls/configure-manager-and-admin-my-team-access.md) for the administrator procedure.

## visibility and action are separate

seeing an employee does not grant every action for that employee. for example, **View - Timesheet**, **Add - Timesheet**, **Edit - Timesheet**, and **Delete - Timesheet** are separate controls. the same action can be enabled for **Direct Reports** but unavailable for **Department** scope.

this means you might be able to add a missing timesheet but not delete an existing one. use only the action enabled for the record you need to maintain. company rules and the record's current status can still prevent a change even when the action is part of your assigned access.

being able to view or file an employee's request is also different from being assigned to approve it. use **To Do** for requests waiting for your decision, and ask the workflow administrator to check the approval assignment when an expected request is missing. see [review requests in To Do](../approvals/review-requests-in-to-do.md).

when one action is missing, ask the administrator to review that exact function and scope rather than broadening every Manager portal permission.
