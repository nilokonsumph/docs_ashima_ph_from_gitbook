# Create or delete a draft pay run

Create a draft pay run to begin payroll for one configured payroll group and pay date. Delete a draft only when it must be discarded rather than corrected.

**Navigation:**\
go to **Paycheck → Pay Run → Payroll**, then select **+ New**.

## before you begin

* configure the payroll group and pay schedule.
* assign eligible employees to the payroll group.
* confirm compensation, work schedules, pay rates, cost centers, payment settings, and applicable payroll rules.
* confirm that the intended pay date has not already been processed for the same group.

## which settings control this workflow?

| level            | setting or record                                              | effect                                                                   |
| ---------------- | -------------------------------------------------------------- | ------------------------------------------------------------------------ |
| company / global | payroll groups, schedules, rates, payment and payroll settings | supplies the selectable payroll setup                                    |
| module           | payroll lock and workflow rules                                | can restrict creation or later payroll-sensitive actions                 |
| employee         | payroll-group membership and payroll profile                   | determines which employees and payroll inputs are brought into the draft |
| pay run          | selected group and pay date                                    | determines the covered period and creates the dated draft                |

## how do you create a draft?

1. select the payroll group on **select payroll group**.
2. review the employees, employee IDs, work schedules, pay schedule, pay rate, and cost center loaded for that group.
3. select the available payroll date when the page presents it.
4. verify the resulting pay period.
5. click **done**.
6. confirm the draft appears under **draft pay runs** before making exclusions, adjustments, or recalculating.

The workflow displays three stages: **Payroll Input**, **Preview & Approve**, and **Process Payment**. Creating the draft begins the first stage; it does not approve or close payroll.

## how do you delete a draft?

1. return to the Pay Run workspace.
2. select only the open draft that must be discarded.
3. click **delete**.
4. review and confirm the warning when the selected Pay Run ID, group, pay date, and period are correct.
5. verify the draft no longer appears.

> \[!WARNING] Draft deletion removes generated payroll output for the selected draft and inactivates the run. Use recalculation or correction workflows when the payroll should continue. Controlled create/delete validation is still required before this article is publication ready.

## related articles

* [pay run workspace and history](/broken/pages/1aae811cf00a844c563a72b274efd3a4f11bcde1)
* [review and recalculate a pay run](/broken/pages/4b2260817fafa8f67821e1a140643d4dd7a297ab)
* [payroll groups and schedules](file:///4659123/settings/payroll_groups_and_schedules.md)
