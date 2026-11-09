# Edit or delete timesheets

Use Edit to correct inaccurate punches or a shift date. Use Delete only when the entire timesheet should not exist.

> \[!WARNING] Editing or deleting a timesheet changes attendance results and can affect payroll. A timesheet included in a closed payroll cannot be deleted.

**Navigation:**\
go to **Hours → Timesheets**.

## when should i edit instead of delete?

* **Edit** when the employee worked but a punch, break, or shift date is wrong.
* **Delete** when the entire timesheet was created in error and should not exist.
* Correct the assigned shift first when the punches are accurate but Ashima interpreted them using the wrong schedule.
* Resolve a pending employee adjustment or application before making a separate direct correction.

## how do i edit a timesheet?

1. Find the employee and dates in **Timesheet Logs**.
2. Select one or more eligible records.
3. Select **Edit**.
4. Correct the shift date or available punch fields.
5. Review any lock or validation message.
6. Select **Save**.

## how do i delete a timesheet?

1. Find the employee and dates in **Timesheet Logs**.
2. Select one or more eligible records.
3. Select **Delete**.
4. Review the selected employee and dates in the confirmation window.
5. Select **Delete Log**.

## why is a timesheet locked?

| condition                                                          | result                                                                            |
| ------------------------------------------------------------------ | --------------------------------------------------------------------------------- |
| payroll is waiting for approval                                    | direct editing is blocked until payroll returns to an editable state              |
| payroll is closed                                                  | deletion is blocked; an eligible correction follows post-payroll adjustment rules |
| a timesheet application is pending                                 | direct editing is blocked while the request is unresolved                         |
| post-payroll adjustment was already used for the employee and date | another direct post-payroll correction is blocked                                 |
| required privilege is missing                                      | the action is hidden or unavailable                                               |

## what happens after editing or deleting?

The affected employee and dates are queued for attendance recalculation. A deleted record is removed from the active result; an edited record uses the corrected values.

After recalculation:

* verify the corrected row and its source;
* review hours, tardiness, undertime, absence, and schedule context;
* review related leave, overtime, rest-day, or holiday records; and
* review any affected open pay run and recalculate it when required.

## related articles

* [timesheet logs](/broken/pages/b36f1a9cae607a72a7a3b5140344b394b41cfa5a)
* [add a timesheet](/broken/pages/6715ba37022ecfd6728b92f36f8036bbe8ce8d7a)
* post-payroll adjustments
* payroll recalculation
