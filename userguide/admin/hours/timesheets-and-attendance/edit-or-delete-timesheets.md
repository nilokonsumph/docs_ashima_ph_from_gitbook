# edit or delete timesheets

## edit or delete timesheets

use Edit to correct inaccurate punches or a shift date. use Delete only when the entire timesheet should not exist.

{% hint style="warning" %}
**warning:** editing or deleting a timesheet changes attendance results and can affect payroll. a timesheet included in a closed payroll cannot be deleted.
{% endhint %}

**Navigation:**\
go to **Hours → Timesheets**.

### when should i edit instead of delete?

* **Edit** when the employee worked but a punch, break, or shift date is wrong.
* **Delete** when the entire timesheet was created in error and should not exist.
* correct the assigned shift first when the punches are accurate but Ashima interpreted them using the wrong schedule.
* resolve a pending employee adjustment or application before making a separate direct correction.

### how do i edit a timesheet?

1. find the employee and dates in **Timesheet Logs**.
2. select one or more eligible records.
3. select **Edit**.
4. correct the shift date or available punch fields.
5. review any lock or validation message.
6. select **Save**.

### how do i delete a timesheet?

1. find the employee and dates in **Timesheet Logs**.
2. select one or more eligible records.
3. select **Delete**.
4. review the selected employee and dates in the confirmation window.
5. select **Delete Log**.

### why is a timesheet locked?

| condition                                                          | result                                                                            |
| ------------------------------------------------------------------ | --------------------------------------------------------------------------------- |
| payroll is waiting for approval                                    | direct editing is blocked until payroll returns to an editable state              |
| payroll is closed                                                  | deletion is blocked; an eligible correction follows post-payroll adjustment rules |
| a timesheet application is pending                                 | direct editing is blocked while the request is unresolved                         |
| post-payroll adjustment was already used for the employee and date | another direct post-payroll correction is blocked                                 |
| required privilege is missing                                      | the action is hidden or unavailable                                               |

### what happens after editing or deleting?

successful edits and deletions automatically invoke timesheet recalculation for the affected employee dates. a deleted record is removed from the active result; an edited record uses the corrected values.

after recalculation:

* verify the corrected row and its source;
* review hours, tardiness, undertime, absence, and schedule context;
* review related leave, overtime, rest-day, or holiday records; and
* review any affected open pay run and recalculate it when required.

### edit or delete several timesheet rows

use batch edit when selected rows need the same review session but still require row-specific times and break values. Ashima validates employee, company, schedule, payroll state, and the submitted time sequence before saving. deleting a timesheet is a soft deletion: the active time row is inactivated and flagged as deleted from Hours rather than physically erased.

{% hint style="warning" %}
**warning:** a time record connected to closed payroll can be blocked from ordinary deletion or correction. use the supported post-payroll-adjustment path when the page identifies the record as eligible. a PPA correction is a new controlled adjustment; it does not rewrite the closed payroll.
{% endhint %}

after a successful add, edit, batch edit, deletion, or import, review the recalculated row. if the page shows pending recalculation, run **Recalculate** and wait for **In Sync** before exporting or using the results in payroll.

### related articles

* [timesheet logs](timesheet-logs.md#page-045-pages-admin-hours-timesheet-logs-md)
* [add a timesheet](add-a-timesheet.md#page-046-pages-admin-hours-add-a-timesheet-md)
* [post-payroll adjustments](../../paycheck/corrections-controls-and-ingestion/use-post-payroll-adjustments.md)
* [payroll recalculation](../../paycheck/run-payroll/review-and-recalculate-a-pay-run.md)
