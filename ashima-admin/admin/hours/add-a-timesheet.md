# Add a timesheet

Use Add Timesheet to create one or more missing time records for an employee from the Admin Portal.

> \[!WARNING] Adding a timesheet changes attendance results and can affect an open payroll. Confirm the employee, shift date, and punches before saving.

**Navigation:**\
go to **Hours → Timesheets**, then select **Add Timesheet**.

## what must be set up first?

The employee needs a valid work schedule for the shift date. The schedule determines which lunch and additional-break fields are available.

Time-entry settings, access privileges, pending applications, and payroll state can also determine whether the date is open for direct entry or requires another correction process.

## fields

| field                  | use                                              |
| ---------------------- | ------------------------------------------------ |
| choose employee        | selects the employee who owns every queued row   |
| shift date             | identifies the work date and assigned schedule   |
| time in                | records the start of work                        |
| lunch out and lunch in | records lunch when the assigned shift tracks it  |
| 1st break out and in   | records the first additional break when enabled  |
| 2nd break out and in   | records the second additional break when enabled |
| time out               | records the end of work                          |

Enter dates in `MM/DD/YYYY` format. Only fields supported by the employee's assigned shift are available.

## how do i add a timesheet?

1. Open **Hours → Timesheets**.
2. Select **Add Timesheet**.
3. Search for and select the employee.
4. Enter the **Shift Date**.
5. Enter **Time In** and **Time Out**.
6. Enter lunch and break punches when the assigned shift requires them.
7. Select **Add Row** to queue another timesheet for the same employee.
8. Review every row and select **Save**.

Use **Remove** to discard a queued row before saving, or **Cancel** to return without saving.

## what happens after saving?

The records appear in Timesheet Logs and are queued for attendance recalculation. After recalculation:

* confirm the employee, shift date, and source;
* review scheduled and actual hours;
* review tardiness, undertime, absence, and break results;
* confirm any overtime, rest-day, holiday, or leave relationship; and
* recalculate an affected open pay run when required.

## why is a break field unavailable?

The employee's assigned shift does not use that break field for the selected date. Review the shift before changing the timesheet. Do not add a punch merely to fill a blank field.

## when should i not add a direct timesheet?

Do not create a second direct correction when a related employee adjustment or approval request is pending. A closed-payroll date also cannot be treated like an ordinary open attendance record; use the eligible post-payroll process when applicable.

## related articles

* [timesheet logs](/broken/pages/b36f1a9cae607a72a7a3b5140344b394b41cfa5a)
* [edit or delete timesheets](/broken/pages/742330828f2bd6407478cd319321ca70eadc72b6)
* time entry settings
* shift assignments
* post-payroll adjustments
