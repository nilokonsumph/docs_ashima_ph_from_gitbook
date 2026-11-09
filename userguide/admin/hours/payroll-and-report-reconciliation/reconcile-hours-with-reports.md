# reconcile Hours with reports

## reconcile Hours with reports

use reports after the underlying timesheets have been recalculated. a report organizes or snapshots source data; deleting or regenerating it does not correct the shift, punch, leave, approval, or payroll record that produced the result.

### which Hours-related output should i use?

| question or purpose                                    | output                                                                     | what it shows                                                                                                                                                       | important limit                                                                                                                              |
| ------------------------------------------------------ | -------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| review the exact operational rows currently on screen  | **Hours → Timesheets → Download**                                          | filtered timesheet rows, punches, schedule, source, and interpreted attendance values included by the export                                                        | it follows the active filters and has a 4,000-row limit                                                                                      |
| find likely attendance exceptions                      | **Reports → Hours → Possible Errors**                                      | a saved snapshot of missing logs and configured tardiness or undertime conditions for the selected run                                                              | it identifies review candidates; it does not prove that the shift, leave, or timesheet is wrong                                              |
| summarize attendance for a selected scope              | **Reports → Hours → Attendance**                                           | a saved attendance report with employee and period detail available for review and download                                                                         | generate it again after correcting source records; an older saved report remains a historical snapshot                                       |
| compare timekeeping categories with payroll-paid hours | **Reports → Hours → Paid Hours**                                           | absences, tardiness, undertime, leave, holiday, rest-day, overtime, night-differential, scheduled, worked, and paid-hour categories for the selected pay-date scope | optional overtime, rest-day, and paid-leave inclusion changes the total; paid leave is disabled for a monthly-paid scope in the current form |
| trace administrator activity in a module               | **Reports → Others → Log Summary**                                         | dated administrator actions filtered by administrator and module                                                                                                    | this is an administrative activity report, not an employee punch report                                                                      |
| confirm the money produced from approved time          | employee pay details and the applicable payroll or payroll-register report | the calculated earnings, premiums, and attendance deductions included in payroll                                                                                    | recalculate the open pay run after an eligible Hours source changes                                                                          |

### generate and use a possible error report

1. confirm that the relevant employee dates are recalculated.
2. open **Reports → Hours → Possible Errors**.
3. set the report dates and filters.
4. generate the report.
5. open the saved report and review the grouped employee findings.
6. use the available leave-status lookup before treating an absence as an error.
7. open the employee's assigned shift, leave, and timesheet source records.
8. correct the governing source record.
9. recalculate the affected timesheet and any open pay run.
10. generate a fresh report when you need evidence of the corrected state.

the **Possible Errors Indicator (BETA)** setting controls whether Hours highlights employees with missing logs or tardiness or undertime at or above the configured per-workday threshold for the current pay period. **Missing Logs** remains included in the current setting. the saved possible-error report and the page indicator support review; neither one changes the underlying record.

### use the Attendance Report

use **Reports → Hours → Attendance** when you need a saved report for a selected employee or broader scope and date period. open the report detail to review the generated attendance result, then download it when required.

if the report shows an unexpected absence, tardiness, undertime, leave, holiday, rest-day, overtime, or paid-hours value, compare the report period with the employee's timesheet, assigned shift, approved leave and applications, and payroll state. correct the source record, recalculate Hours, and generate a new report. do not edit a report to mask a source discrepancy.

### use Paid Hours Reconciliation

use **Reports → Hours → Paid Hours** to compare timekeeping categories with the hours recognized for payroll. select one pay date or an allowed pay-date range and choose whether **Overtime**, **Rest Day**, or **Paid Leave** should be included in **Total Paid Hours**.

review the report at employee level or by date. the current detail can separate:

* absences, tardiness, and undertime;
* paid and unpaid leave;
* regular, special, double-holiday, and rest-day hours;
* ordinary and special-day overtime;
* night differential and night-differential overtime by day type;
* total paid hours, non-attendance hours, total hours worked, and total scheduled hours.

{% hint style="warning" %}
**important:** report options change the comparison. confirm the pay-date scope and optional categories before concluding that Hours and payroll disagree. for a monthly-paid scope, **Paid Leave** is disabled in the current report form because paid leave is normally handled through the applicable absence, leave, and payroll logic.
{% endhint %}

\## use Log Summary for administrative traceability

**Reports → Others → Log Summary** generates a dated record of administrator activity for selected administrators and modules. use it when you need to identify who performed a supported administrative action and in which module.

it is not the employee's clock-in history. use **Hours → Timesheets**, the punch-level **Source**, and timesheet history for employee punches. use Log Summary or the applicable audit trail to supplement that evidence when an administrator changed a record or setting.

### investigate a difference from source to report

1. confirm the employee, work dates, report period, and pay-date scope.
2. review the assigned shift and special-day classification.
3. inspect each punch and its **Source**.
4. review approved leave and pending or completed timesheet, overtime, rest-day, holiday, or mobile-clock-in requests.
5. compare the applicable time-entry, tardiness, overtime, holiday, rest-day, and workflow settings.
6. confirm that Hours is recalculated.
7. compare the relevant Attendance or Paid Hours report with employee pay details.
8. correct the earliest incorrect source or governing rule.
9. recalculate Hours and the open pay run.
10. regenerate the report and verify the corrected result.
