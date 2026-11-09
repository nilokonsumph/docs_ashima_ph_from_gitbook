# configure shift rules

shift definitions establish the workdays, rest days, expected hours, break rules, and—where offered—threshold, grace, and cross-date premium choices that Hours uses to interpret an employee's logs. A saved definition becomes available for payroll-group defaults or dated employee assignments; saving it does not assign it.

**Navigation:** go to **Shifts → Shifts Planning** for shift definitions. Separate **Settings → Shifts** pages control Night Differential, holiday pay, rest-day approval, and schedule-request lead time.

## what shift types are available?

* **Regular, Compressed, and Night** use fixed daily time ranges.
* **Flexi Time** uses its configured required-hours, arrival, and break rules.
* **Open Shift** has a separate actual-work entry and review flow.
* **Rest Day** represents a date without a normal work requirement.

For the full comparison and the fields that differ by family, see [shift types and schedule rules](../../shifts/configure-and-interpret-shifts/shift-types-and-schedule-rules.md).

## how do i create or change a definition?

Use [configure shift definitions and premium transitions](../../shifts/configure-and-interpret-shifts/shift-settings-overview.md#how-do-i-create-a-shift-definition) for the complete, current task. From **Shifts Planning**, select the family and **Create New** to add a definition; the new form uses **Save**. To change an existing definition, open its row, select **Edit**, then **Update** or **Cancel**. Where available for a non-default definition, **Save as New** creates a separate schedule instead of changing the original.

The system checks weekly time ranges, including overnight overlaps with the following workday. Review any validation message before changing the schedule. A boundary that ends exactly when the next scheduled range starts is allowed; an overlapping interval is not.

## what happens after saving?

The definition becomes available for payroll-group defaults and employee assignments. Changing a definition used by employees can change their schedule interpretation and affected open payroll. Review the employee calendar, Hours result, and open pay run after a consequential change.

## verify the resulting shift behavior

create or open a representative shift using the saved rule, assign it to a test employee for a future date, and verify the expected schedule and timesheet context. if the result is wrong, correct the shift definition or future assignment; do not attempt to repair an ongoing shift by deleting its schedule context.

## continue in the affected module

* [create, assign, and maintain shifts](../../shifts/)
* [review time against assigned shifts](../../hours/)
