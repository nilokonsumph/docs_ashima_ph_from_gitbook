# Shift settings overview

Use Shift settings to define reusable work schedules before assigning them to payroll groups or employees. Choose the shift family that matches how work time is expected, recorded, and reviewed.

**Navigation:**\
go to **Settings → Shifts**.

> \[!WARNING] A shift is timekeeping and payroll source data. Changing a shift that is already assigned can change expected hours, tardiness, undertime, breaks, rest-day treatment, holiday treatment, and open-payroll results. Use **Save As New** when a new rule should coexist with the old one.

## which shift type should i use?

| shift family | use it when                                                                                            | main time rule                                                                                       |
| ------------ | ------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------- |
| Regular      | employees follow defined daily start, break, and end times                                             | each selected workday has a fixed schedule                                                           |
| Compressed   | employees work a defined schedule that concentrates required hours into fewer or longer workdays       | still uses fixed daily time ranges; the schedule itself defines the compressed arrangement           |
| Night        | the regular schedule starts or continues through nighttime hours                                       | fixed schedule plus the applicable night-shift differential settings                                 |
| Flexi Time   | employees may begin within configured limits but must satisfy the day's required hours and break rules | daily required hours, latest allowed start, and login/break settings replace one fixed start pattern |
| Open Shift   | work does not use the same fixed daily start/end schedule as the other shift families                  | recorded Open Shift time and its approval/adjustment workflow establish worked time                  |
| Rest Day     | a date should be identified as a non-working scheduled day                                             | no normal work requirement; recorded work is handled through rest-day and premium rules              |

Regular, Compressed, and Night are maintained through the same fixed-schedule framework. Their business meaning comes from the selected family and the actual daily schedule you configure.

## how do shift records connect?

1. **Shift settings** create a reusable schedule.
2. A **payroll-group default** can provide the normal schedule for employees in that group.
3. A dated **employee shift assignment** can apply another schedule for specific dates.
4. **Hours** uses the dated result to interpret logs, attendance, tardiness, undertime, breaks, rest days, and holidays.
5. **Paycheck** uses the resulting approved or calculated hours and premiums.

Do not assume that saving a shift automatically assigns it. Setup and assignment are separate actions.

## what should i decide before creating a shift?

* the shift family;
* covered workdays and rest days;
* daily start, end, and break rules where applicable;
* required daily hours for flexible work;
* threshold and grace-period behavior where available;
* whether normal timekeeping is allowed on rest days or holidays;
* premium behavior when one shift crosses a workday, rest day, or holiday boundary; and
* whether a payroll-group default or dated employee assignment will use the shift.

## how do i create or maintain a shift?

1. Open the correct shift-family tab.
2. Select the add action or open an existing schedule.
3. Enter a clear schedule name.
4. Complete the displayed schedule and rule fields.
5. Review the calculated daily and total hours.
6. Confirm the displayed rest days.
7. Review threshold, grace, break, rest-day, holiday, and premium options that appear for that family.
8. Save the shift or use **Save As New** when preserving the original is required.
9. Assign the saved shift through the payroll-group or employee assignment workflow.
10. Review affected employee calendars and recalculate affected open payroll.

## related articles

* [shift types and schedule rules](/broken/pages/88550025ccf662a1d76eb68f49b6e36d0e2f7e5c)
* [thresholds, grace periods, and breaks](/broken/pages/3505341c9bc5d3c4f930d73e7cdb39ad49842236)
* [open shift](/broken/pages/ddbe4589e870c34f5ea3ff238f61390ca97e69a3)
* [rest days and shift enforcement](/broken/pages/c790226a3e50e55d559f4bd4d7a5c082a79351f7)
* [company holiday calendar](/broken/pages/2525e1950b69a5b43e117a1b1800597460980396)
* [assign shifts](/broken/pages/08a1f7b44b69f79977984c87a38ba957b852e9be)
* [manage and archive shifts](/broken/pages/4c7eea4ab75758dad23a0601d8fee31035e2cf4b)
