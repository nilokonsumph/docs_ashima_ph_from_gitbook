# start here: manage employee schedules

## start here: manage employee schedules

use the shifts module to create reusable schedules, assign them to employees for specific dates, maintain the holiday calendar, and confirm how the resulting schedule is interpreted in hours and paycheck.

### why are shifts crucial to accurate timekeeping?

a shift provides the expected schedule for an employee and date. time logs record what the employee actually did. Ashima matches the captured logs with the applicable shift so the employee and administrator can quickly interpret the day.

| shift provides                    | captured time logs provide    | the timesheet can show                                             |
| --------------------------------- | ----------------------------- | ------------------------------------------------------------------ |
| expected start and end            | actual clock in and clock out | tardiness, undertime, or a missing clock out                       |
| scheduled lunch and breaks        | actual break out and break in | missing break logs or overbreak under the configured rule          |
| workday or rest-day context       | actual recorded work          | ordinary work, rest-day work, or another applicable classification |
| required hours and schedule rules | actual hours worked           | a difference that may require review or adjustment                 |

this is why correct shift assignment is essential. a time log without the intended shift context can be interpreted against the wrong start, end, break, required-hours, rest-day, or holiday rule.

{% hint style="success" %}
**tip:** plan, plot, and assign shifts before the work period starts. advance assignment gives employees the correct schedule to follow and allows timesheets to identify issues as logs are captured. correcting an incorrectly assigned shift later is a recovery action and can require timesheet recalculation, approval review, and open-payroll review.
{% endhint %}

### how do shifts help employees correct time logs promptly?

employees can use their timesheet to compare captured logs with the assigned shift and identify a late clock in, missing or accidental clock out, missing break log, tardiness, or undertime. after the shift ends and the completed timesheet is available, the employee can promptly file the supported **Timesheet Adjustment** when a log must be corrected.

the adjustment remains subject to the company's workflow, permitted filing period, payroll-lock state, and other applicable controls. after approval, review the recalculated timesheet and any affected open payroll.

### follow the schedule lifecycle

1. create or review the reusable schedule in **Shifts → Shifts Planning**.
2. confirm its workdays, times, breaks, tardiness treatment, rest-day behavior, holiday behavior, and supported premium options.
3. assign the schedule to a payroll group or to employees for specific dates.
4. verify the saved result in **Shifts Overview** or the employee calendar.
5. review affected time entries, approvals, and open payroll when the schedule or holiday context changes.

{% hint style="warning" %}
**warning:** editing a shift definition and assigning a shift are different actions. editing changes the reusable definition; assignment applies a schedule to employee dates. after either change, check affected time entries and recalculate an affected open payroll before relying on its result.
{% endhint %}

\## choose the article for your goal

| administrator goal                                                            | authoritative article                                                                                                                                                             |
| ----------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| review employee schedules or download the current view                        | [shift calendar and overview](plan-and-assign-shifts/shift-calendar-and-overview.md#page-033-pages-admin-shifts-shift-calendar-and-overview-md)                                   |
| assign a schedule to employees or a payroll group                             | [assign shifts](plan-and-assign-shifts/assign-shifts.md#page-034-pages-admin-shifts-assign-shifts-md)                                                                             |
| upload dated employee assignments                                             | [import shift assignments](plan-and-assign-shifts/import-shift-assignments.md#page-035-pages-admin-shifts-import-shift-assignments-md)                                            |
| change a dated shift or return it to the default                              | [change or restore employee shifts](plan-and-assign-shifts/change-or-restore-employee-shifts.md#page-036-pages-admin-shifts-remove-shift-assignments-md)                          |
| archive or restore a reusable schedule                                        | [manage and archive shifts](plan-and-assign-shifts/manage-and-archive-shifts.md#page-037-pages-admin-shifts-manage-and-archive-shifts-md)                                         |
| create, edit, or import reusable shift templates                              | [shift settings overview](configure-and-interpret-shifts/shift-settings-overview.md#page-038-pages-admin-shifts-shift-settings-overview-md)                                       |
| choose among regular, compressed, night, flexi time, open shift, and rest day | [shift types and schedule rules](configure-and-interpret-shifts/shift-types-and-schedule-rules.md#page-039-pages-admin-shifts-shift-types-and-schedule-rules-md)                  |
| configure threshold, grace, tardiness, lunch, or additional breaks            | [thresholds, grace periods, and breaks](configure-and-interpret-shifts/thresholds-grace-periods-and-breaks.md#page-040-pages-admin-shifts-thresholds-grace-periods-and-breaks-md) |
| configure and review work without a fixed daily pattern                       | [open shift](configure-and-interpret-shifts/open-shift.md#page-041-pages-admin-shifts-open-shift-md)                                                                              |
| mark dates as rest days or interpret rest-day work                            | [rest days and shift enforcement](configure-and-interpret-shifts/rest-days-and-shift-enforcement.md#page-042-pages-admin-shifts-rest-days-and-shift-enforcement-md)               |
| set up, import, edit, or review holidays and their rates                      | [company holiday calendar](configure-and-interpret-shifts/company-holiday-calendar.md#page-043-pages-admin-shifts-company-holiday-calendar-md)                                    |

### understand which record you are changing

a **shift template** is the reusable schedule definition. every employee has a default work schedule through the applicable payroll group. a dated **shift assignment** temporarily overrides that default for selected dates. changing the dated assignment replaces the override; using **Delete** on the dated override returns those dates to the employee's default work schedule.

### review dependent settings and outputs

| dependency                           | why it matters                                                                                                     |
| ------------------------------------ | ------------------------------------------------------------------------------------------------------------------ |
| **Night Differential Settings**      | controls the applicable NSD calculation context; a night shift name alone does not establish payable NSD           |
| **Holiday Pay Settings**             | controls approval and related holiday-pay behavior                                                                 |
| **Rest Day Settings**                | controls whether qualifying rest-day work requires approval before payment                                         |
| **Schedule Request Settings**        | controls employee schedule-change lead time                                                                        |
| **Hours → Timesheets**               | shows how the saved schedule and holiday context were interpreted for employee time                                |
| **Todo**                             | holds applicable employee schedule-change, open shift, rest-day, or holiday approvals                              |
| **Reports → Shifts → Shift History** | provides the audit-oriented schedule-change history                                                                |
| **Paycheck**                         | uses the resulting eligible hours and premiums; recalculate affected open payroll after a material schedule change |

### before changing a schedule

confirm the employee or payroll-group scope, covered dates, existing assignments, recorded time, pending requests, approved leave, holiday context, and any open or closed payroll covering the dates. closed-payroll dates and other protected records can block a change.
