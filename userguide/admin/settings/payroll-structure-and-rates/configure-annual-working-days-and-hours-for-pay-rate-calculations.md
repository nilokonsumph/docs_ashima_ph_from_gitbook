# configure annual working days and hours for pay-rate calculations

use **Pay Rate Calculation** to define the annual working-day basis and average working hours per day used by salary-to-day and salary-to-hour calculations. use one company-wide basis when employees share the same working-day convention. enable advanced settings when a rank needs its own annual working-day value.

**navigation:** go to **Settings → Paycheck → Pay Rate → Pay Rate Calculation**.

## understand the two calculation modes

| mode             | what you maintain                                                | how Ashima uses it                                                                                                               |
| ---------------- | ---------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| company-wide     | **Working Days in a Year** and **Average Working Hours per Day** | supplies the common day and hour basis when a rank-specific override is not active                                               |
| advanced by rank | a rank and its **Total Working Days in a Year**                  | replaces the company-wide working-day basis for employees in that rank; the company average-hours value remains a separate input |

the working-day value is not only descriptive. current calculation paths read it when converting monthly amounts into day or hour values and when calculating affected payroll, leave, and termination components. a rank override therefore needs to match the employee's assigned rank.

## update the company-wide basis

1. review **Working Days in a Year** and **Average Working Hours per Day**.
2. select **Edit** when the page is in view mode.
3. enter the supported numeric values.
4. save the change and confirm that the updated values reload on the page.
5. recalculate an affected open payroll or other supported calculation before relying on its result.

when **Average Working Hours per Day** is left empty in the current save path, Ashima stores `8`. treat this as a product default, not a recommendation for every company.

## use advanced settings by rank

1. enable **Advanced Settings** and complete the password confirmation shown by Ashima.
2. select **add pay rate**.
3. choose the rank and enter **Total Working Days in a Year**.
4. save and verify that the rank appears in the list.
5. open a saved row to edit it, or select one or more rows and use the delete action when the override should no longer apply.

Ashima requires a rank and a numeric total-working-days value. deleted rows are made inactive rather than removed from the audit history.

{% hint style="warning" %}
**warning:** changing this basis can change results that convert monthly compensation into daily or hourly values. review the effective employee rank and recalculate affected open records. do not assume that previously approved or closed results are rewritten automatically.
{% endhint %}

\## continue in the affected module

* [review payroll calculations](../../paycheck/)
