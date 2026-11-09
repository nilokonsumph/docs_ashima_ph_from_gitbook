# configure holidays and the holiday calendar

these are three related decisions. **Holiday Pay Settings** controls the holiday-pay options displayed by Ashima. **Rest Day Settings** controls whether qualifying rest-day work needs approval. **Holiday Schedule** defines the dates and classifications to which holiday rules may apply. Check the relevant setting and calendar date before interpreting a time record or an open pay run.

## change Holiday Pay Settings

**Navigation:** **Settings → Shifts → Holiday Pay Settings**.

1. Review the current options and choose **Edit** for the setting you need to change.
2. Change the applicable toggle or conditional field and review the confirmation. A toggle can require a password confirmation before its new state takes effect.
3. Confirm the saved state on the page. Select **Cancel** to leave an edit unchanged.

The holiday-pay controls are independent of the Night Differential settings and the holiday calendar. Each applicable toggle has its own confirmation; do not look for a single page-level **Update** that saves every toggle. Review an affected timesheet and open payroll after a consequential change.

## set rest-day approval

**Navigation:** **Settings → Shifts → Rest Day Settings**.

Open **Enable approval for rest day pay**, select **Edit**, choose whether approval is required, then select **Update**. Select **Cancel** if you do not want to save the change. When approval is required, a captured rest-day time entry alone does not complete the pay decision; review the related application and its status in [Hours](../../hours/premium-work/rest-day-and-holiday-work.md).

This setting does not turn an ordinary workday into a rest day or change the holiday calendar. The assigned shift and date still determine the work context.

## choose the holiday calendar

Choose the calendar source that matches your company's approved holiday list:

1. **Use the default holiday calendar** provided by ashima.
2. **Upload a custom holiday list** using a CSV template.

## how do i use the default holiday calendar?

1. Open **Shifts → Holiday Schedule**.
2. Review the offered default schedule for the selected year and confirm it when it matches your company's policy.
3. Verify the dates, classifications, and locations before payroll uses them.

for a custom schedule, follow [the holiday-calendar import and confirmation steps](../../shifts/configure-and-interpret-shifts/company-holiday-calendar.md#can-i-import-holidays). **Upload File** stages the CSV; **Continue** saves valid rows. choosing the custom-calendar option in the setup prompt only closes that prompt. calendar setup is separate from changing a holiday-pay toggle.

## verify the calendar result

open the holiday calendar and confirm the date, classification, location or scope, and year. then review a representative shift or timesheet for that date. if the classification is wrong, correct the holiday record before payroll uses it and recalculate the affected open time or payroll result where supported.

## continue in the affected module

* [use holiday classifications in Shifts](../../shifts/)
* [review holiday work in Hours](../../hours/)
