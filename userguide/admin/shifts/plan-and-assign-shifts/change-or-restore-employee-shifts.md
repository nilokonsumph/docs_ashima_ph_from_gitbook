# change or restore employee shifts

## change or restore employee shifts

every employee has a default work schedule through the applicable payroll group. a dated assignment overrides that default for selected dates. administrators can replace a dated shift for one employee or make the same change for multiple employees. when an employee should use the default again, clear only the dated override.

{% hint style="warning" %}
**important:** the **Delete** control on a dated custom assignment does not leave the employee without a shift. it deletes the dated override, after which the employee's default work schedule applies. it does not delete the reusable shift template or the payroll-group default.
{% endhint %}

**Navigation:**\
go to **Shifts → Shifts Overview**.

### choose the intended result and scope

| intended result                                              | action                                                                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------- |
| change one employee's shift                                  | open the employee's dated cell and use the edit action                                                  |
| change several employees or a whole payroll group            | use **Assign Shifts**, choose the date range, and select employees by **Payroll Group** or **Employee** |
| return selected dates to the default work schedule           | clear the dated override with **Delete**                                                                |
| change the normal schedule for everyone in the payroll group | update the payroll-group default through the applicable setup workflow                                  |
| stop a reusable shift from appearing in future setup         | use the separate archive workflow in **Manage Shifts**                                                  |

### change one employee's shift

1. display the affected week in **Shifts Overview**.
2. find the employee and date.
3. point to the dated cell and select the edit action.
4. choose the intended **Work Schedule**.
5. review the **From** and **To** dates. the selected date is loaded first; change the range only when the replacement should cover additional dates.
6. save the assignment.
7. verify the replacement schedule in the employee calendar.

### change shifts in bulk

1. select **Assign Shifts** from **Shifts Overview**.
2. choose the intended **Work Schedule** and enter the **From** and **To** dates.
3. under **Select Employees**, choose **Payroll Group** to load employees from one group, or **Employee** to select one or more employees directly.
4. review the generated **Employee list** and remove anyone who should not be included.
5. save the assignment.
6. review validation messages. when Ashima allows valid employees to continue, confirm that excluded employees and dates are handled separately.
7. verify representative employee calendars and affected timesheets.

the bulk action applies the chosen shift to every valid employee-date in the reviewed scope. it replaces a dated assignment for those dates; it does not change dates outside the selected range or modify the reusable shift definition.

### return selected dates to the default shift

1. display the affected week in **Shifts Overview**.
2. confirm that the date currently has a custom dated assignment.
3. select the dated assignment and choose **Delete**. use the bulk **Delete** action only when the reviewed employees and displayed date range should all return to their defaults.
4. review the warning, employees, and affected dates.
5. confirm the action.
6. verify that each employee calendar now shows the applicable default work schedule for those dates.

### understand when a shift assignment cannot be changed

these rules apply when assigning, replacing, or clearing a dated employee shift assignment. they are different from editing the reusable shift template.

| condition                                                  | what Ashima does                                                          | what the administrator should do                                                                                                                  |
| ---------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| the employee's shift is ongoing                            | blocks the dated shift change                                             | wait for the employee to clock out, then wait **60 minutes after clock-out** before changing the assignment                                       |
| the date has a pending timesheet                           | blocks the dated shift change                                             | have the timesheet approved or rejected, then retry the change                                                                                    |
| the employee has an overlapping pending shift request      | blocks the affected shift change                                          | approve, reject, or otherwise resolve the pending shift request before retrying                                                                   |
| the date belongs to a closed pay run                       | blocks assignment, replacement, and dated-override deletion for that date | remove the closed-payroll dates from the requested range; use the supported payroll correction process when a historical result must be addressed |
| the date has approved or pending leave                     | displays a warning                                                        | review the leave dates, status, and schedule used by the leave before deciding whether to continue                                                |
| a bulk selection contains valid and invalid employee-dates | can offer to continue with only the valid records                         | review every excluded employee and date before continuing, then resolve the excluded records separately                                           |

{% hint style="warning" %}
**important:** do not try to correct an ongoing shift by overwriting its assignment. wait until the employee has clocked out and the 60-minute protection period has passed. then change the dated assignment and review the recalculated timesheet.
{% endhint %}

\## understand additional assignment and import messages

| message or condition                                                      | meaning and recovery                                                                                                                                                    |
| ------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| the requested range is longer than the supported action                   | standard bulk assignment is capped at 90 days from the start date; calendar assignment is capped at nine months. use a shorter range and confirm the displayed end date |
| **There are no rest days on the shift period specified**                  | the selected rest-day-work schedule applies only to qualifying rest-day dates, but none exist in the requested range. correct the dates or schedule                     |
| imported shift overlaps the previous shift                                | the two calculated time ranges overlap. correct the shift, date, or adjacent-day assignment before importing again                                                      |
| **Can't assign rest day on an open shift**                                | the ordinary rest-day assignment does not apply to an employee using an open shift. use the open-shift workflow and its applicable rules                                |
| invalid or blank shift name                                               | the import name does not match an available reusable shift. use the exact current shift name or **Mark as Rest Day** where supported                                    |
| employee is missing or outside the administrator's shift visibility scope | correct the employee ID or use an authorized administrator whose scope includes the employee                                                                            |
| invalid **Valid From** or **Valid Until**                                 | correct the date format and ensure **Valid From** is not later than **Valid Until**                                                                                     |
| import exceeds 18,250 expanded employee-date records                      | reduce the employee count or date range; the limit counts each employee-date produced by the file, not only CSV rows                                                    |

errors block the affected record. warnings require review and can allow the supported valid records to continue. after any partial bulk action or import, verify the saved employees and dates instead of assuming the entire request succeeded.

### what happens after the change?

Ashima recalculates affected timesheets after a successful individual change, bulk change, or dated-override deletion. each employee continues to have schedule context: either the newly assigned shift or the applicable default work schedule.

review the employee calendars, affected timesheets, attendance results, approvals, and any open payroll covering the changed dates. recalculate the open payroll when required.

### what should i check before changing shifts?

* the employee or payroll-group scope;
* the default work schedule that will apply when no dated override exists;
* the intended dates and replacement schedule;
* the generated employee list for a bulk change;
* existing time logs and pending timesheets;
* approved or pending overtime, rest-day, holiday, leave, or shift-change requests;
* an open or closed payroll covering the dates; and
* validation messages that exclude an employee or date from the change.

### what if the wrong change was saved?

assign the correct shift again for the affected employees and dates. if an employee should use the default, clear only the dated override and verify the default schedule appears. then review the recalculated timesheets and any affected open payroll.

### related articles

* [shift calendar and overview](shift-calendar-and-overview.md#page-033-pages-admin-shifts-shift-calendar-and-overview-md)
* [assign shifts](assign-shifts.md#page-034-pages-admin-shifts-assign-shifts-md)
* [import shift assignments](import-shift-assignments.md#page-035-pages-admin-shifts-import-shift-assignments-md)
* [manage and archive shifts](manage-and-archive-shifts.md#page-037-pages-admin-shifts-manage-and-archive-shifts-md)
