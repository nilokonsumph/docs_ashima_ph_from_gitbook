# understand shift types and schedule rules

## understand shift types and schedule rules

use this guide to choose the appropriate shift family and understand its purpose, timekeeping effect, and expected result. this is the authoritative shift-type comparison for the shifts module.

| shift family   | use it when                                                                   | effect on timekeeping and payroll inputs                                                                                               |
| -------------- | ----------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| **Regular**    | employees follow defined daily start, break, and end times                    | each selected workday has a fixed schedule used for expected logs, tardiness, undertime, and breaks                                    |
| **Compressed** | required hours are concentrated into fewer or longer configured workdays      | the fixed daily ranges and configured rest days establish the compressed pattern; Ashima does not design the arrangement automatically |
| **Night**      | the fixed schedule starts or continues through nighttime hours                | the actual worked time, schedule boundaries, and applicable NSD settings determine downstream night differential inputs                |
| **Flexi Time** | employees may start within configured limits but must complete required hours | required hours, latest allowed start, login, and break rules replace one fixed start pattern                                           |
| **Open Shift** | work cannot be represented by an ordinary fixed or flexi schedule             | recorded open shift time and its adjustment or approval workflow establish the hours input                                             |
| **Rest Day**   | a date has no normal scheduled work requirement                               | work recorded on the date follows rest-day capture, approval, entitlement, premium, and payroll rules                                  |

choose by the result you need in **Hours**. the shift family is not merely a label: it controls which fields are available and how attendance is interpreted. saving the template does not assign it; assignment is a separate dated action.

To inspect or create a definition, go to **Shifts → Shifts Planning** and choose its family. The comparison below explains those choices; it is not a separate Ashima settings page.

for **Regular**, **Compressed**, **Night**, and **Rest Day**, each configured workday must be unique. an overnight row may cross midnight but must not overlap the next configured workday. a boundary that ends exactly when the next row starts is allowed. equal start and end times represent a 24-hour schedule and can therefore overlap the following day.

### regular shift

a regular shift uses defined workdays and fixed daily time ranges. configure start time, end time, lunch, optional additional breaks, rest days, and the displayed advanced rules.

use it when employees are expected to follow a stable schedule such as monday to friday, 8:00 am to 5:00 pm.

the scheduled start provides the reference for threshold, grace, tardiness, and expected time logs when those functions are enabled.

### compressed shift

a compressed shift uses the same fixed-schedule framework but represents a work arrangement in which required hours are concentrated into the configured workdays.

the label does not calculate a compliant compressed schedule for you. the administrator must configure the correct workdays, daily times, breaks, and total hours under the approved company arrangement.

review the calculated total hours before saving and confirm that the remaining days are intentionally shown as rest days.

### night shift

a night shift is a fixed schedule intended for work during nighttime hours or across midnight. configure the actual start, end, and break times; do not rely on the name alone.

night-shift differential eligibility is also governed by the applicable **Night Shift Differential settings** and the actual worked hours. creating a night shift does not by itself prove that every recorded hour qualifies for NSD.

#### set up Night Differential separately

The **Night** shift family defines a schedule. **Settings → Shifts → Night Differential Settings** separately controls whether Night Differential is enabled and how its available calculation rules work. An employee's compensation details determine which enabled rule applies to that employee. Check all three before interpreting an NSD result.

On the Night Differential page, the main toggle shows whether the setting is on. Changing it requires password confirmation; the detail controls are unavailable while it is off. When the setting is on, select **Edit** to change the displayed hours or calculation-rule controls, then **Update** and complete the confirmation, or select **Cancel**. The NSD rate comes from the configured pay-rate choice; do not infer it from the name of a Night shift. Review an affected employee and open payroll after a change.

when a shift crosses midnight, review the advanced workday, rest-day, and holiday boundary rules because different portions of the shift can fall on different date types.

### flexi time shift

a flexi time shift uses configured rules for each covered day rather than one fixed daily start pattern. its current schedule data can include:

* total required hours for the day;
* latest time-in allowed;
* whether login is required;
* lunch-break duration;
* applicable workdays and rest days; and
* holiday and premium behavior.

flexi time does not mean unlimited arrival and departure. the configured limits and required hours still control how hours interprets the employee's logs.

### open shift

open shift does not use the same fixed start/end structure as regular, compressed, night, or flexi time. it is intended for work whose actual time must be recorded through the open shift workflow.

open shift has its own employee logs, adjustments, and approval surfaces. it should not be used merely to avoid setting up an ordinary schedule.

see [open shift](open-shift.md#page-041-pages-admin-shifts-open-shift-md) for the complete recording, approval, verification, and recovery workflow.

### rest day schedule

a rest day identifies a date without a normal scheduled work requirement. it is not a standing instruction that any hours logged on that date are automatically payable.

rest-day work remains subject to captured time, the applicable approval rule, employee entitlement, premium settings, and payroll calculation.

see [rest days and shift enforcement](rest-days-and-shift-enforcement.md#page-042-pages-admin-shifts-rest-days-and-shift-enforcement-md) for assignment, approval, premium, and verification guidance.

### which options do not apply equally?

| option                                    | fixed shifts                     | flexi time                                  | open shift                                          | rest day                                              |
| ----------------------------------------- | -------------------------------- | ------------------------------------------- | --------------------------------------------------- | ----------------------------------------------------- |
| fixed daily start/end                     | yes                              | replaced by flexi rules                     | no ordinary fixed schedule                          | no normal work schedule                               |
| threshold and grace after scheduled start | available where displayed        | use the flexi limits shown for the schedule | not the ordinary basis                              | not the ordinary basis                                |
| lunch and additional breaks               | configurable                     | configurable flexi break rules              | limited to the open shift form                      | not a normal-day requirement                          |
| assigned rest days                        | yes                              | yes                                         | cannot use the ordinary mark as rest day assignment | the date itself is the rest day                       |
| holiday timekeeping option                | available where displayed        | available                                   | available                                           | holiday/rest-day combination follows applicable rules |
| advanced cross-date premium rules         | available on supported schedules | supported options may appear                | separate open shift processing                      | governed by rest-day/holiday settings                 |

### review after saving

* confirm the shift appears under the correct family;
* confirm the workdays and rest days;
* confirm daily and total hours;
* confirm threshold, grace, and break rules;
* confirm holiday and rest-day timekeeping options;
* assign the shift to the intended payroll group or employees; and
* review employee calendars and affected open payroll.
