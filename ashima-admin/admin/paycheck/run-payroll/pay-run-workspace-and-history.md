# Pay run workspace and history

Use Pay Run to start payroll work, review payrolls still being prepared, and find payrolls that are waiting for approval or already closed.

**Navigation:**\
go to **Paycheck → Pay Run → Payroll**.

## before you begin

* confirm that payroll groups, pay schedules, pay dates, employee payroll assignments, and required payroll settings are complete.
* confirm that source changes to compensation, time, leave, earnings, deductions, contributions, or tax have been approved and recalculated where required.
* use an account with payroll access.

## which settings control this workflow?

| level            | setting or record                                                                                      | effect                                                                          |
| ---------------- | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------- |
| company / global | payroll groups, pay schedules, rates, contributions, tax, payment, and payslip settings                | supplies the reusable payroll configuration                                     |
| module           | payroll lock and approval workflow                                                                     | controls whether payroll-sensitive changes are allowed and who approves payroll |
| employee         | payroll group, compensation, pay type, tax, contribution, payment, entitlement, and assigned pay items | supplies employee-specific payroll inputs                                       |
| pay run          | payroll group, pay date, pay period, exclusions, adjustments, and current state                        | defines one payroll processing cycle                                            |

The pay run does not replace company or employee setup. It calculates a dated payroll from those settings and records, together with approved run-specific changes.

## what does the page show?

The current page contains two sections:

* **draft pay runs** — payrolls still being prepared.
* **pay run history** — payrolls waiting for approval or already closed.

Both tables show Pay Run ID, payroll group and schedule, pay date, pay period, payroll cost and included/excluded information, status, and available actions.

Draft rows currently provide **View Details**, **View Payroll Masterlist**, and **View Payroll Exclusion**. History rows can provide **View Recalc History** and **View Payroll Masterlist**.

## how do you find a pay run?

1. use **select employee** on draft pay runs when you need employee-specific context.
2. select the available payroll date after choosing an employee.
3. click **search**.
4. use **select pay run ids** and **search** in Pay Run History when you know the run identifier.
5. open the relevant action only after confirming the payroll group, pay date, pay period, and status.

## what happens next?

* **View Details** opens employee payroll totals and recalculation controls.
* **View Payroll Masterlist** opens consolidated payroll review and output actions.
* **View Payroll Exclusion** manages employees included in the selected draft.
* **View Recalc History** traces recalculation activity for the selected historical run.

> \[!WARNING] An **Open** status does not by itself prove every source record is current or every action is allowed. Check the payroll lock, approval state, readiness indicators, and recalculation status before continuing.

## related articles

* [create or delete a draft pay run](/broken/pages/5dc1f32924de589f21c8d71600259643edc68a5c)
* [review and recalculate a pay run](/broken/pages/4b2260817fafa8f67821e1a140643d4dd7a297ab)
* [payroll groups and schedules](file:///4659123/settings/payroll_groups_and_schedules.md)
* [workflow and manager access](file:///4659123/settings/workflow_and_manager_access.md)
