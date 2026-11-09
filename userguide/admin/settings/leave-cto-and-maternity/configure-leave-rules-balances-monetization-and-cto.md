# configure leave rules, balances, monetization, and CTO

use leave settings to define leave types, eligibility, accrual, expiry, conversion, and related company rules before assigning leave to employees.

**navigation:** go to **Settings → Leaves**.

## what should i configure?

* leave type name and unit
* earning or accrual rule
* effective and eligibility behavior
* expiry or carryover rule
* conversion or monetization option where supported
* approval and documentation requirements
* cto source, conversion, rate, and expiry settings when cto is enabled

## how do settings relate to employee assignment?

the leave setting defines the reusable policy. The employee assignment applies a configured leave type to one employee and records opening earned/used values and the effective start rule. The validated assignment form did not expose a separate opening-expiry field.

the **Leave Settings** list shows the leave unit, whether units are required, paid status, monetization, accrual frequency/start, conversion treatment for unused leave and termination, conversion run, and required lead time. These module rules are not redefined by the employee's opening balance.

## which settings control this workflow?

| level            | setting or record                                                       | effect                                                         |
| ---------------- | ----------------------------------------------------------------------- | -------------------------------------------------------------- |
| company / global | configured leave type                                                   | defines the reusable leave program and its unit                |
| module           | accrual, paid status, monetization, conversion, lead time, and workflow | controls how balances are earned, used, converted, or approved |
| employee         | assigned type, opening values, and effective start                      | establishes the employee's balance and eligibility timing      |
| transaction      | leave application, cancellation, conversion, or transfer                | changes or reserves balance under the configured rules         |

## how do i update a leave rule?

when configuring a paid leave type that requires credits and uses one-time accrual, leave **earned leaves / leave given upfront** blank or enter zero or a positive number. Negative or nonnumeric values fail validation. This condition does not change the requirements for unpaid leave or recurring accrual. Use the save steps below after reviewing the rule.

1. open the applicable leave setting.
2. review the employees and balances already using the type.
3. update the available rule.
4. review any effective or expiry consequence.
5. click **Save**.

{% hint style="warning" %}
**warning:** changing an active accrual or expiry rule can affect employee balances. Create a new leave type when the policy meaning changes and the old history must remain distinct.
{% endhint %}

\## verify the change and recover safely

review one affected employee's assigned leave type, balance, effective dates, and a representative request before relying on the setting. if the result is incorrect, restore the supported setting, correct the employee assignment or balance through its owning workflow, and verify again. do not assume that changing a rule rewrites approved or historical leave.

## continue in the affected module

* [use leave, balance, monetization, and CTO settings](../../leaves-cto/)
