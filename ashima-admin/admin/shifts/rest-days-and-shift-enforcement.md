# Rest days and shift enforcement

A rest day is a scheduled date without the employee's normal work requirement. It does not mean that any time entered on that date is automatically paid, and it does not always mean that Ashima will ignore the employee's logs.

**Navigation:**\
go to **Shifts → Rest days and shift enforcement**.

### how is a rest day established?

A date can become a rest day through:

* the reusable shift's configured rest days;
* a dated **Mark as Rest Day** employee assignment; or
* a dedicated rest-day schedule where the current setup uses one.

The employee calendar should display the resulting date as a rest day.

### can an employee work on a rest day?

Yes, when the company permits rest-day work and the required time and approval conditions are met. Rest-day work is not the same as ordinary scheduled work.

The employee cannot simply arrive at any time and assume that every recorded hour is payable. Review:

* the applicable shift and date;
* whether normal timekeeping on rest days is enabled for the schedule;
* captured start, end, and break logs;
* the rest-day work or premium approval setting;
* employee entitlement; and
* the calculated Hours and payroll result.

### can a shift be enforced on a rest day?

Supported fixed and flexible schedules expose a **Timekeep normally on Rest Days** option. When enabled, the configured schedule rules can be used to interpret rest-day timekeeping rather than treating the date as completely unscheduled.

This does not convert the date into an ordinary workday or remove premium rules. It provides schedule context for the captured time. Review the resulting rest-day classification and pay treatment.

Open Shift does not support the ordinary **Mark as Rest Day** assignment. Handle Open Shift dates through the Open Shift and applicable premium workflow.

### how do i mark selected dates as rest days?

1. Go to **Shifts → Shifts Overview**.
2. Select the employee or employees.
3. Open **Assign Shifts**.
4. Enter the covered From and To dates.
5. Select **Mark as Rest Day**.
6. Review validation messages, existing logs, pending timesheets, pending shifts, leave, and closed-payroll restrictions.
7. Confirm the assignment.
8. Review the employee calendar.

Bulk imports can also use `Mark as Rest Day` as the schedule name. The import rejects duplicate employee dates and can exclude dates in closed pay runs.

### what happens when a rest day is also a holiday?

The company holiday calendar first determines whether the holiday applies to the employee's location. Hours and payroll then use the holiday type, rest-day status, schedule rules, application requirements, and configured rates.

Do not add a duplicate holiday or remove the rest day simply to force a rate. Correct the calendar, shift, or premium settings that govern the date.

### review checklist

* employee calendar shows the intended rest day;
* no conflicting dated shift exists;
* recorded work has the correct approval state;
* holiday scope is correct when applicable;
* rest-day and holiday premiums are not duplicated;
* affected timesheets have been recalculated; and
* open payroll reflects the intended result.
