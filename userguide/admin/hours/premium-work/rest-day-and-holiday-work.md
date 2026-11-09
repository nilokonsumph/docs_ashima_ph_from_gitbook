# review rest-day and holiday work

## review rest-day and holiday work

use the rest day and holiday records to check work captured on a scheduled rest day or holiday and determine whether an application is still required.

**Navigation:**\
go to **Hours → Restday** for rest-day records, or open the employee's timesheet for holiday work details.

### what should i know before reviewing these records?

Ashima captures valid time entries even when the date is a rest day or holiday. captured work becomes payable only after the applicable settings, employee entitlement, and approval requirements are satisfied.

when a date is both a rest day and a holiday, the required action follows the enabled application rules. the page must not offer two competing applications for the same source work.

### how do i review rest day or holiday work?

1. select the date or date range.
2. search for the employee or apply the available work schedule, department, or position filters.
3. compare the captured time with the assigned shift and calendar classification.
4. check whether rest-day or holiday approval is required in settings.
5. review the related application and approval status.

### what action should appear on an overlapping date?

the current Restday page provides actions to filter, review, and download eligible records. privileged users can delete eligible logs; pending rows cannot be selected, and rows in closed payroll cannot be deleted.

when a date is both a rest day and a holiday, check the assigned shift, holiday calendar, and available application before deciding which approval is needed. Recalculation does not bypass an approval the company requires. For consecutive rest days, review the intended shift date; an overnight shift is associated with its start date.

### what happens after approval?

approved work becomes available to payroll under the applicable rest-day or holiday rule. Recalculate an open pay run after a source time record or approval changes.

### how do i download rest-day records?

apply the needed filters, open the download control, and select **Excel** or **CSV**.

### interpret rest-day and holiday work

a valid time log may have both rest-day and holiday context. Its pay treatment depends on the applicable shift, calendar, settings, and approved application. When rest-day approval is enabled, a pending recalculated row remains excluded until approval. When approval is disabled, an otherwise eligible recalculated rest-day row can be included without a pending approval. Review the employee's calculated pay before treating either case as complete.

if the same work is converted to CTO, Ashima records the conversion against the source row and excludes the successfully minted source from payroll. failed or rejected CTO conversion does not exclude the source work merely because conversion was attempted.

### related articles

* [timesheet logs](../timesheets-and-attendance/timesheet-logs.md#page-045-pages-admin-hours-timesheet-logs-md)
* [overtime records](overtime-history.md#page-050-pages-admin-hours-overtime-history-md)
* [holiday and rest day settings](../../settings/time-entry-hours-shifts-and-holidays/configure-holidays-and-the-holiday-calendar.md)
* [review overtime, rest day, and holiday requests](../../todo-workflow/request-specific-approvals/review-premium-work-requests.md)
