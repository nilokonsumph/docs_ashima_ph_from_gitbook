# configure thresholds, grace periods, and breaks

## configure thresholds, grace periods, and breaks

use these controls to define how a scheduled shift interprets arrival time and break logs. availability depends on the selected shift family.

These controls appear in the applicable shift-definition form under **Shifts → Shifts Planning**. Choose a shift family and open a definition to see which controls that family offers.

### what is the shift threshold?

the shift threshold allows an employee to start within a configured number of minutes after the scheduled start without immediately being treated under the ordinary fixed-start rule.

example: for an 8:00 am shift with a 60-minute threshold, the threshold extends to 9:00 am.

the form displays guidance that the threshold should not exceed half of the minimum required work hours for the day.

### what is the grace period?

grace is the configured period after the applicable start reference before the employee is marked tardy under the selected tardiness rule.

when both threshold and grace are enabled, grace begins after the threshold—not directly after the original start time.

example: an 8:00 am shift with a 60-minute threshold and a 10-minute grace period uses 9:00 am as the start of grace. the employee becomes subject to the selected tardiness rule after that grace window.

grace does not change the scheduled hours or automatically excuse missing work. it changes the point at which tardiness treatment begins.

### which tardiness rule applies?

when grace is enabled, select one of the company tardiness rules displayed by the form. those rules are maintained separately from the shift itself.

if no tardiness rule is available, complete the required tardiness setup before relying on shift grace behavior.

### how do lunch and breaks work?

a supported fixed shift can define:

* whether lunch is enabled;
* paid or unpaid treatment;
* whether employees must log break out and break in;
* fixed or flexible break scheduling;
* break duration;
* up to the displayed number of additional breaks; and
* advanced enforcement of required break logs.

tracked breaks allow hours to identify late return or overbreak using the configured schedule. a break shown in the shift is not proof that the employee recorded the required break punches.

for **Flexi Time**, lunch duration is active only when login is required and break handling is **capture** or **assumed**. a hidden lunch-duration field is not an active schedule rule.

### what should i validate?

1. review the displayed daily schedule and calculated hours.
2. confirm the threshold is appropriate for the business rule.
3. confirm the selected tardiness rule matches the intended outcome.
4. confirm paid versus unpaid break treatment.
5. confirm whether break punches are required.
6. test a representative employee date before broad assignment.
7. review attendance and open payroll after assignment or change.

### common problems

* **Employee appears tardy sooner than expected:** check whether the threshold is enabled and whether grace begins after it.
* **No tardiness rule is available:** review the company tardiness settings.
* **Hours are lower than expected:** check unpaid break duration and required daily hours.
* **Overbreak is not shown:** confirm break tracking and the employee's break-out and break-in logs.
* **A schedule change does not appear:** confirm the dated employee assignment and recalculate the affected timesheet or open payroll.
