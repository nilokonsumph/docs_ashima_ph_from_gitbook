# review payroll variance

use Payroll Variance to compare payroll results and identify material changes between runs or periods.

**navigation:** go to **Reports**, then select **Payroll Variance**.

## when should you use this report?

use it during payroll review to find employees whose pay changed because of salary updates, attendance, earnings, deductions, contributions, tax, or other payroll inputs.

## how do you review payroll variance?

1. open **Payroll Variance** and enter the report name.
2. choose **Previous Pay Date** and review the automatically filled **Date From** and **Date To**. open payroll dates are not offered in that selection.
3. enter the **Variance** percentage for your review threshold. choose **Filter By → All**, **Pay Group**, or **Employee Name**, then complete the group or employee selection when needed.
4. select **Generate**. correct any validation errors; choose **Cancel** to leave the form without generating.
5. compare the current and comparison periods and review the employee amount differences.
6. trace an unexpected amount to Employee Pay Details or the owning source record. correct that record and recalculate payroll before generating another comparison.
7. use **XLS** or **CSV** to download the generated result when your access permits it.

use the same employee and payroll scope for a meaningful comparison. a difference caused by comparing different populations is not necessarily a payroll error.

## what does a variance mean?

a variance identifies a difference; it does not automatically mean an error. confirm whether the difference is expected before changing payroll.

common valid causes include a changed employee population, salary or payroll-group change, approved time or leave, added earnings or deductions, statutory recalculation, tax adjustment, and a different pay-run period. compare like-for-like runs before treating the variance as exceptional.

## what should i record during review?

for each material difference, record whether it is expected, needs correction, or requires another reviewer. trace the amount to Employee Pay Details or the owning source page. after a correction, recalculate the affected payroll and regenerate the variance report so the review does not rely on a stale comparison.

## can a saved variance report be removed?

Payroll Variance generates a comparison for review and download. it does not provide a saved-report list to reopen or delete. select **Generate** to return to the comparison form and prepare a fresh result. keep the downloaded comparison if your review process requires a record.

## how is the variance percentage calculated?

when both compared amounts are positive:

{% hint style="info" %}
**variance (%) = (current amount − previous amount) ÷ previous amount × 100**

the result is rounded to two decimal places.
{% endhint %}

for example, an increase from 10,000 to 11,000 produces a 10% variance. a decrease from 10,000 to 9,000 produces −10%. the report displays a negative variance in parentheses.

| amounts being compared                                          | result |
| --------------------------------------------------------------- | ------ |
| previous amount is zero or negative; current amount is positive | 100%   |
| previous amount is positive; current amount is zero or negative | −100%  |
| both amounts are zero or negative                               | 0%     |

the **Variance** threshold identifies increases at or above the entered percentage. decreases are classified separately as negative; the threshold is not an absolute-value rule that treats an equal-sized increase and decrease the same way. review the amounts as well as the percentage, especially when the previous amount is zero.
