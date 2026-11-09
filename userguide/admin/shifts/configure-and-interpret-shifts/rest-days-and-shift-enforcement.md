# understand rest days and shift enforcement

## understand rest days and shift enforcement

a rest day is a scheduled date without the employee's normal work requirement. it does not mean that any time entered on that date is automatically paid, and it does not always mean that Ashima will ignore the employee's logs.

**Navigation:**\
go to **Shifts → Shifts Overview** for dated **Mark as Rest Day** assignments, or **Shifts → Shifts Planning → Rest Day** for reusable and enforcement rules.

### how is a rest day established?

a date can become a rest day through:

* the reusable shift's configured rest days;
* a dated **Mark as Rest Day** employee assignment; or
* a dedicated rest-day schedule where the current setup uses one.

the employee calendar should display the resulting date as a rest day.

### can an employee work on a rest day?

yes, when the company permits rest-day work and the required time and approval conditions are met. rest-day work is not the same as ordinary scheduled work.

the employee cannot simply arrive at any time and assume that every recorded hour is payable. review:

* the applicable shift and date;
* whether normal timekeeping on rest days is enabled for the schedule;
* captured start, end, and break logs;
* the rest-day work or premium approval setting;
* employee entitlement; and
* the calculated hours and payroll result.

### can a shift be enforced on a rest day?

supported fixed and flexible schedules expose a **Timekeep normally on Rest Days** option. when enabled, the configured schedule rules can be used to interpret rest-day timekeeping rather than treating the date as completely unscheduled.

this does not convert the date into an ordinary workday or remove premium rules. it provides schedule context for the captured time. review the resulting rest-day classification and pay treatment.

open shift does not support the ordinary **Mark as Rest Day** assignment. handle open shift dates through the open shift and applicable premium workflow.

### how do i mark selected dates as rest days?

1. go to **Shifts → Shifts Overview**.
2. select the employee or employees.
3. open **Assign Shifts**.
4. enter the covered from and to dates.
5. select **Mark as Rest Day**.
6. review validation messages, existing logs, pending timesheets, pending shifts, leave, and closed-payroll restrictions.
7. confirm the assignment.
8. review the employee calendar.

bulk imports can also use `Mark as Rest Day` as the schedule name. the import rejects duplicate employee dates and can exclude dates in closed pay runs.

if the wrong dates were marked as rest days, assign the intended working schedule for those dates. if the payroll-group default should apply, clear only the dated rest-day override with **Delete**. then verify the default schedule in the employee calendar, recalculate affected time, and review open payroll.

### what happens when a rest day is also a holiday?

the company holiday calendar first determines whether the holiday applies to the employee's location. hours and payroll then use the holiday type, rest-day status, schedule rules, application requirements, and configured rates.

do not add a duplicate holiday or remove the rest day simply to force a rate. correct the calendar, shift, or premium settings that govern the date.

### review checklist

* employee calendar shows the intended rest day;
* no conflicting dated shift exists;
* recorded work has the correct approval state;
* holiday scope is correct when applicable;
* rest-day and holiday premiums are not duplicated;
* affected timesheets have been recalculated; and
* open payroll reflects the intended result.
