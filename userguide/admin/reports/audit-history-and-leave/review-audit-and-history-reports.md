# review audit and history reports

use Audit Trail and history reports to trace saved actions and record changes in Ashima.

Audit information supports investigation, but it should be read together with the affected employee, payroll, shift, or approval record.

**navigation:** go to **Reports → Others → Audit Trail** or **Log Summary**. Use **Reports → Pay Run → Compensation History** or **Reports → Shifts → Shift History** for those focused histories.

## what can you review?

Audit Trail lists date/time, user, module, category, change from, and change to. It provides date, module, employee, category, and user filters. Open the export menu to choose **XLS** or **CSV**. Separate reports exist for compensation and shift changes. For workflow changes, current audit details identify the affected employee and the resolved approver levels.

## how do you investigate a change?

1. choose the **From/To** dates and the module, employee, category, and user filters you need, then select **Search**. use **Clear** to reset the filters.
2. locate the affected record. **Employee Name** search includes employees with **End of Employment** status, so you can review a separated employee's status history.
3. compare the entry's user, date, module, and change-from/change-to values with the source record and approval history.
4. check whether a later correction or recalculation followed the action.
5. choose **XLS** or **CSV** from the export menu when you need a review copy.

## why might the audit trail not explain the payroll amount by itself?

the audit trail records activity. Payroll calculations can also depend on shifts, time logs, approvals, compensation, settings, and recalculation timing. Use the related report or detail page to understand the final amount.

## how do i generate a Compensation History report?

use **Reports → Pay Run → Compensation History** to review pay-rate changes, their effective dates, adjustment details, and who updated them.

1. choose **Generate** to open report setup.
2. enter **Report Name**, **Date From**, and **Date To**. the end date cannot precede the start date.
3. choose **All Employees** or **Selected Employees**. for **Selected Employees**, select between 1 and 10 employees. if your access offers **All Non-confidential** or **All Confidential**, choose the appropriate group.
4. select **Active Employees**, **Inactive Employees**, or both. leaving both clear uses active employees; it does not produce an intentionally empty report.
5. choose **Generate**, correct any form errors, and check the resulting report name, coverage, and employee inclusions. choose **Cancel** or **X** to leave setup without generating.
6. review each employee's **Pay Rate To/From**, effective date, adjustment date and details, and updated-by information. use pagination for additional results.
7. choose **XLS** or **CSV** to download the permitted results for that generated report.

{% hint style="info" %}
the download uses the report's last generated coverage and inclusions, across its result pages. to change the download, change the setup and select **Generate** again. unsaved setup edits do not change the current report.
{% endhint %}

for employee-specific records, see [review salary and compensation history](../../workforce/compensation-and-payroll-assignments/review-salary-and-compensation-history.md).

## how do i use Log Summary?

use **Reports → Others → Log Summary** to review administrator activity for selected dates and modules.

1. create a named report and enter **From/To** dates.
2. select the administrators and modules to include.
3. select **Save**, correct any validation errors, and open the saved detail. select **Cancel** to discard unsaved creation.
4. confirm the saved dates, **Admin User**, and **Modules**, then review the activity rows. use the offered sort and **XLS** or **CSV** output.
5. to remove an unneeded saved summary, select its report row and confirm **Delete**. this does not delete the underlying activity records.

for captured employee punches, use [timesheet guidance in Hours](../../hours/).
