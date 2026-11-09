# Thresholds, grace periods, and breaks

Use these controls to define how a scheduled shift interprets arrival time and break logs. Availability depends on the selected shift family.

**Navigation:**\
go to **Shifts → Thresholds, grace periods, and breaks**.

### what is the shift threshold?

The shift threshold allows an employee to start within a configured number of minutes after the scheduled start without immediately being treated under the ordinary fixed-start rule.

Example: for an 8:00 AM shift with a 60-minute threshold, the threshold extends to 9:00 AM.

The current form limits the threshold so it does not exceed half of the minimum required work hours for the day.

### what is the grace period?

Grace is the configured period after the applicable start reference before the employee is marked tardy under the selected tardiness rule.

When both threshold and grace are enabled, grace begins after the threshold—not directly after the original start time.

Example: an 8:00 AM shift with a 60-minute threshold and a 10-minute grace period uses 9:00 AM as the start of grace. The employee becomes subject to the selected tardiness rule after that grace window.

Grace does not change the scheduled hours or automatically excuse missing work. It changes the point at which tardiness treatment begins.

### which tardiness rule applies?

When grace is enabled, select one of the company tardiness rules displayed by the form. Those rules are maintained separately from the shift itself.

If no tardiness rule is available, complete the required tardiness setup before relying on shift grace behavior.

### how do lunch and breaks work?

A supported fixed shift can define:

* whether lunch is enabled;
* paid or unpaid treatment;
* whether employees must log break out and break in;
* fixed or flexible break scheduling;
* break duration;
* up to the displayed number of additional breaks; and
* advanced enforcement of required break logs.

Tracked breaks allow Hours to identify late return or overbreak using the configured schedule. A break shown in the shift is not proof that the employee recorded the required break punches.

### what should i validate?

1. Review the displayed daily schedule and calculated hours.
2. Confirm the threshold is appropriate for the business rule.
3. Confirm the selected tardiness rule matches the intended outcome.
4. Confirm paid versus unpaid break treatment.
5. Confirm whether break punches are required.
6. Test a representative employee date before broad assignment.
7. Review attendance and open payroll after assignment or change.

### common problems

* **Employee appears tardy sooner than expected:** check whether the threshold is enabled and whether grace begins after it.
* **No tardiness rule is available:** review the company tardiness settings.
* **Hours are lower than expected:** check unpaid break duration and required daily hours.
* **Overbreak is not shown:** confirm break tracking and the employee's break-out and break-in logs.
* **A schedule change does not appear:** confirm the dated employee assignment and recalculate the affected timesheet or open payroll.
