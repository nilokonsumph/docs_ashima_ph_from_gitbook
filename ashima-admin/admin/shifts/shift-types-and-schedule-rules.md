# Shift types and schedule rules

Use this guide to choose the appropriate shift family and understand which rules are meaningful for each type.

**Navigation:**\
go to **Shifts → Shift types and schedule rules**.

### regular shift

A Regular shift uses defined workdays and fixed daily time ranges. Configure start time, end time, lunch, optional additional breaks, rest days, and the displayed advanced rules.

Use it when employees are expected to follow a stable schedule such as Monday to Friday, 8:00 AM to 5:00 PM.

The scheduled start provides the reference for threshold, grace, tardiness, and expected time logs when those functions are enabled.

### compressed shift

A Compressed shift uses the same fixed-schedule framework but represents a work arrangement in which required hours are concentrated into the configured workdays.

The label does not calculate a compliant compressed schedule for you. The administrator must configure the correct workdays, daily times, breaks, and total hours under the approved company arrangement.

Review the calculated total hours before saving and confirm that the remaining days are intentionally shown as rest days.

### night shift

A Night shift is a fixed schedule intended for work during nighttime hours or across midnight. Configure the actual start, end, and break times; do not rely on the name alone.

Night-shift differential eligibility is also governed by the applicable **Night Shift Differential settings** and the actual worked hours. Creating a Night shift does not by itself prove that every recorded hour qualifies for NSD.

When a shift crosses midnight, review the advanced workday, rest-day, and holiday boundary rules because different portions of the shift can fall on different date types.

### flexi time shift

A Flexi Time shift uses configured rules for each covered day rather than one fixed daily start pattern. Its current schedule data can include:

* total required hours for the day;
* latest time-in allowed;
* whether login is required;
* lunch-break duration;
* applicable workdays and rest days; and
* holiday and premium behavior.

Flexi Time does not mean unlimited arrival and departure. The configured limits and required hours still control how Hours interprets the employee's logs.

### open shift

Open Shift does not use the same fixed start/end structure as Regular, Compressed, Night, or Flexi Time. It is intended for work whose actual time must be recorded through the Open Shift workflow.

Open Shift has its own employee logs, adjustments, and approval surfaces. It should not be used merely to avoid setting up an ordinary schedule.

See open shift for the full workflow.

### rest day schedule

A Rest Day identifies a date without a normal scheduled work requirement. It is not a standing instruction that any hours logged on that date are automatically payable.

Rest-day work remains subject to captured time, the applicable approval rule, employee entitlement, premium settings, and payroll calculation.

See rest days and shift enforcement.

### which options do not apply equally?

| option                                    | fixed shifts                     | flexi time                                  | open shift                                          | rest day                                              |
| ----------------------------------------- | -------------------------------- | ------------------------------------------- | --------------------------------------------------- | ----------------------------------------------------- |
| fixed daily start/end                     | yes                              | replaced by flexi rules                     | no ordinary fixed schedule                          | no normal work schedule                               |
| threshold and grace after scheduled start | available where displayed        | use the flexi limits shown for the schedule | not the ordinary basis                              | not the ordinary basis                                |
| lunch and additional breaks               | configurable                     | configurable flexi break rules              | limited to the Open Shift form                      | not a normal-day requirement                          |
| assigned rest days                        | yes                              | yes                                         | cannot use the ordinary Mark as Rest Day assignment | the date itself is the rest day                       |
| holiday timekeeping option                | available where displayed        | available                                   | available                                           | holiday/rest-day combination follows applicable rules |
| advanced cross-date premium rules         | available on supported schedules | supported options may appear                | separate Open Shift processing                      | governed by rest-day/holiday settings                 |

### review after saving

* confirm the shift appears under the correct family;
* confirm the workdays and rest days;
* confirm daily and total hours;
* confirm threshold, grace, and break rules;
* confirm holiday and rest-day timekeeping options;
* assign the shift to the intended payroll group or employees; and
* review employee calendars and affected open payroll.
