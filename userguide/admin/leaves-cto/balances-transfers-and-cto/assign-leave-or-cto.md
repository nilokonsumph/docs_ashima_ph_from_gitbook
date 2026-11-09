# assign leave or CTO

## assign leave or CTO

use leave assignment to make an employee eligible for a specific leave or CTO type and record any opening balance and eligibility date.

**Navigation:**\
go to **Leaves → Leave Balance**, then select **Create**. you can also open an employee's leave details and select **Create** to assign a type to that employee.

### what should i know before assigning CTO?

CTO is not automatic. assign each eligible CTO type, such as CTO overtime, CTO rest day, or CTO holiday, before the employee receives or uses credits from that source.

### which settings control this workflow?

| level            | setting or record                                           | effect                                                    |
| ---------------- | ----------------------------------------------------------- | --------------------------------------------------------- |
| company / global | available leave types                                       | determines which reusable programs can be assigned        |
| module           | leave accrual, conversion, lead-time, and approval rules    | controls the assigned type's ongoing behavior             |
| employee         | assignment, opening earned/used values, and effective start | determines whether and when the employee can use the type |
| transaction      | application, cancellation, conversion, or transfer          | applies a dated change to the employee balance            |

assignment does not override the configured leave policy. it supplies the employee-specific eligibility and opening position within that policy.

### how do i assign a leave or CTO type?

1. select **Create**.
2. select the employee when you started from the main leave balance page. the employee is already selected when you started from employee leave details.
3. select the leave or CTO type.
4. enter the opening earned and used values, if any.
5. enter an adjustment description when the opening values need an explanation.
6. set the effective start date.
7. choose whether the effective start is based on date hired or a custom date. when based on date hired, enter the year or month offset.
8. click **Save**.

### fields

* **Employee Name** — selects the employee who will receive the assignment.
* **Leave Type** — selects the exact leave or CTO program assigned to the employee.
* **Earned Leaves** or **Opening Earned** — records opening credits already earned before this assignment.
* **Adjustment Description** — explains why an opening balance or adjustment was entered.
* **Used Leaves** or **Opening Used** — records credits already used before this assignment.
* **Available Leave Balance** — shows the opening earned amount less the opening used amount.
* **Effective Start Date** — sets when the employee becomes eligible to use the assigned type.
* **Effective Start Date basis** — uses either the employee's date hired or a custom date. the date-hired option supports a year or month offset; `0` allows immediate use from the applicable starting point.

### what happens after assignment?

the assigned type appears in the employee's leave balance. before the effective start date, the employee cannot use it and the application action should not appear. assignment alone does not create new CTO credits; CTO credits still come from an approved conversion or authorized adjustment.

verify the saved leave or CTO type, opening values, effective start date, and available action from the employee's leave details. if the assignment is missing or shows **No Entitlement**, review the type's applicability, effective-date rule, and employee eligibility before creating another assignment.

### related articles

* [leave balances](review-and-correct-leave-balances.md#page-057-pages-admin-leaves-review-and-maintain-leave-leave-balances-md)
* [file leave for an employee](../leave-requests-and-visibility/file-leave-for-an-employee.md#page-059-pages-admin-leaves-review-and-maintain-leave-file-leave-for-an-employee-md)
* [leave transaction ledger](../leave-requests-and-visibility/trace-leave-transactions.md#page-062-pages-admin-leaves-credits-and-related-workflows-leave-transaction-ledger-md)
* [compensatory time off](manage-compensatory-time-off-cto.md#page-053-pages-admin-leaves-compensatory-time-off-md)
