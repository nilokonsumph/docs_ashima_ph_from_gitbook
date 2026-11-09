# increase an employee's salary

## increase an employee's salary

{% hint style="warning" %}
use **salary increase** when changing basic pay. changing basic pay through another action does not create the same salary increase and retroactive-pay records.
{% endhint %}

**navigation:**\
go to **earnings → compensation**, open the employee, then select **salary increase**.

### how do I enter the salary increase?

1. open the employee's compensation page.
2. select **salary increase**.
3. enter the **new basic pay**.
4. select the **effective date**.
5. enter the **adjustment details**, when needed.
6. review the employee's entitlements shown on the form.
7. select **proceed**.
8. confirm the success message, then review the new record in compensation history.

### fields

* **current basic pay** — shows the employee's basic pay before the new change and cannot be edited in this form.
* **new basic pay (\*)** — enter the basic pay that should apply from the effective date.
* **effective date (\*)** — select the first date when the new basic pay applies. this date determines whether the change is current, future-dated, or retroactive.
* **adjustment details** — enter a short reason or reference for the change.
* **entitlements** — review the pay and statutory entitlements shown on the form, including applicable overtime, leave, De Minimis, holiday, and other pay entitlements. this form does not change the employee's tax entitlement; maintain that through the dedicated withholding-tax workflow.

(\*) required fields must be completed before you proceed.

### what warnings can appear?

* **the new basic pay is not greater than the current basic pay** — review the amount before proceeding because the form is intended for a salary increase.
* **retroactive pay is not enabled** — enable **Settings → Paycheck → Earnings → Retroactive Pay** if the effective date belongs to a payroll period already processed and retroactive pay must be calculated.
* **past-period notice** — Ashima identifies that the effective date belongs to a closed payroll period and prepares the resulting retroactive pay for a later payroll.
* **same-coverage notice** — another salary change already affects the same payroll coverage. review both records before creating another entry.
* **stacking rule notice** — the change conflicts with an existing retroactive-pay sequence and cannot proceed until the conflict is corrected.

### what happens after I proceed?

Ashima records the previous basic pay, new basic pay, effective date, adjustment details, entitlements, and change details in compensation history.

the effective date then controls the payroll treatment:

* a current-period change is included in salary increase handling after payroll recalculation.
* a future-dated change waits until its effective date applies.
* a past-period change generates retroactive pay when the setting is enabled and the salary history passes the applicable checks.

### where can I review the result?

open compensation history to confirm the saved salary record. after recalculating payroll, use salary increase details for a current-period change or retroactive pay for earlier payroll periods.

### related articles

* salary increase
* update salaries in bulk
* salary increase details
* retroactive pay
