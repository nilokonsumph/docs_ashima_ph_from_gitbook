# configure pay rates for workdays, rest days, holidays, overtime, and night differential

use **Pay Rates (by Date Type)** to maintain the company's rate table for ordinary workdays, rest days, special holidays, regular holidays, double holidays, overtime, and night differential. the page also supports employee or payroll-group restrictions for the night-differential rate set shown in the restriction area.

**navigation:** go to **Settings → Paycheck → Pay Rate → Pay Rates (by Date Type)**.

## understand what the tables control

the default table stores numeric rate values against Ashima hour types. current rows distinguish date types such as **Workday**, **Rest Day**, **Special Holiday**, **Regular Holiday**, and **Double Holiday**, and expose the applicable working or not-working columns. overtime and night-differential additions are stored with the corresponding hour type.

the labels describe different payroll conditions. a value in one condition does not replace the rate for another condition.

## update the default table

1. review every visible date type and working-status column before editing.
2. select **Edit**.
3. enter numeric values only in the fields that apply to the company's rule.
4. review overtime and night-differential values in the same table.
5. save and confirm the success message.
6. recalculate a representative open pay run and compare the affected pay component before applying the change broadly.

## add a restricted rate set

1. enable the employee-level restriction option when the company needs an exception to the default night-differential rate set.
2. select **add employee restriction**.
3. choose whether the restriction applies through an employee or payroll group selector.
4. select the employee or payroll group.
5. enter numeric values for **Workday**, **Rest Day**, **Special Holiday**, **Regular Holiday**, and **Double Holiday**.
6. save and verify the resulting rows.

the current save rules require the selector and all five numeric date-type values. deleting a restriction makes its employee-specific rows inactive; it does not delete the company default table.

{% hint style="warning" %}
**warning:** the page stores rate values, but the final amount also depends on the employee's compensation, time record, shift, date classification, and other governing settings. use a test calculation to verify the combined result.
{% endhint %}

\## continue in the affected module

* [review payroll calculations](../../paycheck/)
* [review approved premium work](../../hours/)
