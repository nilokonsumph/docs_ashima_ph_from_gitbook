# Rest day and holiday work

use the rest day and holiday records to check work captured on a scheduled rest day or holiday and determine whether an application is still required.

**Navigation:**\
go to **Hours → Restday** for rest-day records, or open the employee's timesheet for holiday work details.

## what should i know before reviewing these records?

Ashima captures valid time entries even when the date is a rest day or holiday. Captured work becomes payable only after the applicable settings, employee entitlement, and approval requirements are satisfied.

when a date is both a rest day and a holiday, the required action follows the enabled application rules. The page must not offer two competing applications for the same source work.

## how do i review rest day or holiday work?

1. select the date or date range.
2. search for the employee or apply the available work schedule, department, or position filters.
3. compare the captured time with the assigned shift and calendar classification.
4. check whether rest-day or holiday approval is required in settings.
5. review the related application and approval status.

## what action should appear on an overlapping date?

the current product rule is:

| rest day application required | holiday application required | action         |
| ----------------------------- | ---------------------------- | -------------- |
| no                            | yes                          | apply holiday  |
| yes                           | no                           | apply rest day |
| yes                           | yes                          | apply holiday  |
| no                            | no                           | change         |

use **Change** to correct the timesheet when neither premium requires an application. Exact button labels and all four live combinations remain part of the live-validation pass.

## what happens after approval?

approved work becomes available to payroll under the applicable rest-day or holiday rule. Recalculate an open pay run after a source time record or approval changes.

## how do i download rest-day records?

apply the needed filters, open the download control, and select **Excel** or **CSV**.

## related articles

* [timesheet logs](file:///pilot_revised_approach/client_articles/timesheet_logs.md)
* [overtime records](/broken/pages/6a162ae7c80129c83e06f3d02b2469778aedb7d1)
* [holiday and rest day settings](file:///4659123/settings/holiday_and_rest_day_settings.md)
* [review overtime, rest day, and holiday requests](file:///4659123/todo/review_premium_requests.md)
