# Review and recalculate a pay run

Use Pay Run Details to review employee payroll totals, open an employee calculation, and recalculate the draft after relevant source changes.

**Navigation:**\
go to **Paycheck → Pay Run → Payroll**, then select **View Details** for an open draft.

## before you begin

* verify the Pay Run ID, payroll group, pay date, period from/to, and **Open** status.
* complete or approve relevant time, leave, compensation, earning, deduction, contribution, tax, exclusion, and adjustment changes.
* confirm that payroll is not blocked by an applicable lock or approval state.

## which settings control this workflow?

| level            | setting or record                                                                  | effect                                                            |
| ---------------- | ---------------------------------------------------------------------------------- | ----------------------------------------------------------------- |
| company / global | pay rates, contribution/tax rules, earnings/deductions, and payroll settings       | provides calculation rules and reusable items                     |
| module           | hours, leave, shifts, workflow, payroll lock, and recalculation behavior           | determines eligible source inputs and whether changes can proceed |
| employee         | compensation, schedule, tax/contribution profile, assigned items, and entitlements | supplies employee-specific calculation inputs                     |
| pay run          | pay date, period, exclusions, adjustments, and recalculation state                 | determines the dated calculation being reviewed                   |

Recalculation regenerates payroll results from current eligible inputs. It should not be described as a simple screen refresh.

## what does the page show?

The current employee table shows:

* Employee Details and ID
* Base Pay
* Taxable Pay
* Non Taxable Pay
* Total Deductions
* Net Pay

Select an employee's Net Pay amount to open the employee calculation detail.

## how do you review the run?

1. confirm the summary dates and status.
2. use **select employee name** and **search** when you need one employee.
3. review the employee totals, including zero or negative values that require explanation.
4. open the employee Net Pay link to trace the calculation components.
5. use **recalc history** to review prior recalculation activity.
6. use **update open shift hrs** only when the open-shift workflow applies and its effect has been reviewed.
7. click **recalc** after eligible source inputs change.
8. verify the recalculation completed and review the affected employee totals again.
9. click **continue to masterlist** only after the run is ready for consolidated review.

## what happens after recalculation?

The system rebuilds generated payroll output for the draft from eligible current source records. Recheck employee details, exclusions, direct payroll adjustments, totals, and downstream readiness before submission.

> \[!WARNING] Recalculation can replace generated payroll breakdown rows. Do not rely on an earlier displayed total after changing a source record. Run-specific adjustments and protected records must be confirmed through the appropriate workflow.

## related articles

* [pay run workspace and history](/broken/pages/1aae811cf00a844c563a72b274efd3a4f11bcde1)
* [timesheet logs](file:///4659123/hours/timesheet_logs.md)
* [payroll groups and schedules](file:///4659123/settings/payroll_groups_and_schedules.md)
* [contribution settings](file:///4659123/settings/contribution_settings.md)
