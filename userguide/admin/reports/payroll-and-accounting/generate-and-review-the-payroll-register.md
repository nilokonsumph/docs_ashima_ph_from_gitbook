# generate and review the payroll register

use the Payroll Register to review the detailed payroll results for a selected pay run.

{% hint style="warning" %}
**important:** review and recalculate the pay run before generating a final register. A report created from outdated payroll results will also be outdated.
{% endhint %}

\*\*navigation:\*\* go to \*\*Reports → Pay Run → Payroll Register\*\*.

## what does the report contain?

the register presents employee payroll amounts from the selected run, including regular pay, earnings, deductions, contributions, withholding tax, and net pay according to the data available for that run.

## how do you generate the report?

1. open **Payroll Register** and create a report.
2. enter its name and select the pay run or period and employee/filter scope.
3. select **Save**. correct any returned validation errors, or select **Cancel** to discard the unsaved form.
4. open the saved report and confirm its period, employee count, payroll status, and pay-item totals.
5. compare those totals with the reviewed source payroll, then choose **XLS** or **CSV** for the output.

## why might columns vary?

Some payroll columns are created from pay items used by the company. A dynamic item may appear under its configured name rather than as a fixed universal column.

## can you delete a saved report?

select the saved report records you no longer need, choose **Delete**, and confirm the selection. keep reports required by your company's review process. removing the report does not correct or delete its source payroll.

## verify the register

confirm the pay run, employee count, payroll-group scope, gross pay, deductions, contributions, withholding tax, and net pay against the reviewed payroll. correct and recalculate the source pay run, then regenerate the register when a total or employee is wrong.

## what does Pay Run Status mean?

the status summarizes the eligible active pay runs matching the report's company, period, and filters. **Rejected** runs are excluded from that status.

| status                   | how to read it                                                                                   |
| ------------------------ | ------------------------------------------------------------------------------------------------ |
| **Open**                 | at least one matching eligible run is open; this takes precedence over the other statuses.       |
| **Waiting for approval** | no matching run is open, but at least one is awaiting approval.                                  |
| **Closed**               | all eligible matching runs are closed.                                                           |
| blank                    | the eligible runs do not produce one of those statuses. a blank is not confirmation of approval. |

for example, a report covering one open run and one closed run shows **Open**. saving the report does not approve or close either run.
