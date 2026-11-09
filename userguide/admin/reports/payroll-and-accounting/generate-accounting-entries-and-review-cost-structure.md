# generate accounting entries and review cost structure

use Accounting Entries to prepare payroll journal information and Cost Structure to review or allocate payroll costs.

**navigation:** go to **Reports → Pay Run**, then select **Accounting Entries** or **Cost Structure**.

## what are accounting entries for?

Accounting Entries organize payroll amounts for journal review. The report is based on the selected payroll data and the company's payroll accounting setup.

## how do you generate accounting entries?

1. create a new **Accounting Entries** report with a report name, pay period, and the required payroll scope or filters.
2. select **Save**, then open the saved report. correct returned errors before retrying, or select **Cancel** to discard the unsaved form.
3. confirm the report period and filters, then review the journal accounts and totals.
4. choose **XLS** or **CSV** for accounting review.

if an account or amount is wrong, correct the payroll or accounting setup and generate fresh output. removing a saved report does not correct its source payroll.

## what is cost structure for?

Cost Structure helps you review how payroll costs are allocated to cost centers, including allocations for an individual employee's worked day. changing an allocation changes the report's cost distribution; it does not change the employee's pay or captured time logs.

## how do you review cost structure?

1. open **Cost Structure**, enter a report name, and choose the payroll scope and period.
2. select **Generate**. correct returned errors, or select **Cancel** to leave without creating the report.
3. open the saved report and search for the employee whose allocation you need to review.
4. open the employee's allocation detail and follow the steps below if it needs changing.
5. choose **XLS** or **CSV** to export the reviewed report.

to rename a report, open its name form and choose **Save** or **Cancel**. a name change does not alter source hours or pay.

## verify and correct the accounting output

compare total debits and credits, payroll totals, cost-center or department allocation, and representative employee detail with the approved payroll and saved mappings. correct the owning payroll, employee assignment, or mapping and regenerate the report. do not edit a downloaded file to conceal a source mismatch.

## how do i allocate an employee's worked hours?

1. open the employee's allocation for the intended day. the day must have worked hours; a day with no worked hours cannot be allocated.
2. choose **Percentage** or **Custom Hours**.
3. enter the values for the cost centers. use the totals below to check the allocation.
4. select **Update**, correct any validation errors, and verify the refreshed values. select **Cancel** to leave the allocation unchanged.

| method           | required total                                 | example for an eight-hour day                                                 |
| ---------------- | ---------------------------------------------- | ----------------------------------------------------------------------------- |
| **Percentage**   | allocations must total 100%.                   | 75% to one cost center and 25% to another represents six hours and two hours. |
| **Custom Hours** | allocations must total the day's worked hours. | enter six hours and two hours, totaling eight.                                |

{% hint style="info" %}
use the worked-hours total displayed for that day. this allocation distributes report costs; it is not a timesheet correction. if the worked hours themselves are wrong, correct the source timekeeping record and review the resulting payroll before regenerating the report.
{% endhint %}

## how do i remove an unneeded saved report?

in the Accounting Entries or Cost Structure report list, select the intended report rows, choose **Delete**, and confirm. this removes report records; it does not remove the source payroll or employee time logs.
