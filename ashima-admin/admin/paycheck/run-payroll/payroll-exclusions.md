# Payroll exclusions

Use Payroll Exclusion to keep an employee in the selected payroll group's context while preventing that employee's payroll from being processed in the current run.

**Navigation:**\
open **View Payroll Exclusion** from a draft pay run, or select **exclusion** from Pay Run Details or Payroll Masterlist.

## before you begin

* confirm the draft is **Open** and verify its pay date and period.
* confirm why the employee must not be processed in this run.
* review timesheet, employment status, leave, and payroll-group information before excluding the employee.

## which settings control this workflow?

| level            | setting or record                               | effect                                                                |
| ---------------- | ----------------------------------------------- | --------------------------------------------------------------------- |
| company / global | payroll group and pay schedule                  | establishes the employees normally eligible for the run               |
| module           | payroll recalculation, approval, and lock state | controls whether exclusion changes can be applied and regenerated     |
| employee         | payroll-group assignment and source readiness   | determines normal inclusion and the reason an exception may be needed |
| pay run          | Exclude Yes/No and optional reason              | changes processing only for the selected draft                        |

Exclusion is a run-specific decision. It does not terminate the employee or remove the employee from the payroll group.

## how do you exclude or include an employee?

1. select **exclude / include employees**.
2. choose the employee.
3. set **Exclude** to **Yes** to exclude the employee or **No** to include the employee again.
4. enter a clear **Reason** when excluding, such as missing timesheet submission or an absence-without-notice case that has been verified.
5. click **save**.
6. confirm the employee, reason, and updated date in the exclusion list.
7. recalculate and review Masterlist so the payroll result reflects the current inclusion state.

Use employee search to find an existing entry. The page also provides a download action for the exclusion list.

> \[!WARNING] The page states that an excluded employee's payroll will remain unprocessed. Do not use exclusion to correct compensation, time, leave, earnings, deductions, or employee status when the source record itself is wrong.

## related articles

* [pay run workspace and history](/broken/pages/1aae811cf00a844c563a72b274efd3a4f11bcde1)
* [review and recalculate a pay run](/broken/pages/4b2260817fafa8f67821e1a140643d4dd7a297ab)
* [payroll masterlist and readiness](/broken/pages/90993c9dd2e7045a5799c0b820706e27adc169e8)
