# configure pay-run warnings

use **Payroll Variance** to choose which conditions Ashima highlights while an administrator reviews a pay run. these settings add review signals. they do not correct the underlying employee, time, bank, earning, or deduction record.

**navigation:** go to **Settings → Paycheck → Payroll Variance**. the current page title is **Pay Run Settings** and the warning area is labelled **Pay Run Errors & Warning Notification (beta)**.

## choose the warnings

| warning                     | condition configured on the page                                                                               |
| --------------------------- | -------------------------------------------------------------------------------------------------------------- |
| payroll variance            | result is higher or lower than the same payroll period of the previous month by more than the saved percentage |
| negative net pay            | employee has negative net pay                                                                                  |
| negative earnings entry     | an earnings entry is negative                                                                                  |
| excessive absences          | total absence hours exceed the saved hour threshold                                                            |
| excessive tardiness         | total tardiness hours exceed the saved hour threshold                                                          |
| excessive undertime         | total undertime hours exceed the saved hour threshold                                                          |
| missing bank account number | required employee bank information is missing                                                                  |

## update and verify the warnings

1. turn **Warning Notification** on or off. the current page saves this master switch immediately.
2. when warnings are on, select **Edit**.
3. enable the checks the payroll reviewer needs.
4. enter the percentage or hour threshold for each enabled threshold-based check.
5. select **Update** and confirm the success message.
6. recalculate or reopen an appropriate test pay run and verify that a known condition is highlighted.
7. correct the owning source record, recalculate where required, and confirm that the warning clears when the condition no longer applies.

{% hint style="warning" %}
**important:** a warning is a review prompt, not an approval decision. A pay run can require investigation even when no configured warning appears.
{% endhint %}

\## continue in the affected module

* [review and recalculate a pay run](../../paycheck/)
