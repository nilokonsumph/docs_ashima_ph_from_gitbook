# Leave settings

use leave settings to define leave types, eligibility, accrual, expiry, conversion, and related company rules before assigning leave to employees.

**Navigation:**\
go to **Settings → Leaves**.

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

The current Leave Settings list shows the leave unit, whether units are required, paid status, monetization, accrual frequency/start, conversion treatment for unused leave and termination, conversion run, and required lead time. These module rules are not redefined by the employee's opening balance.

## which settings control this workflow?

| level            | setting or record                                                       | effect                                                         |
| ---------------- | ----------------------------------------------------------------------- | -------------------------------------------------------------- |
| company / global | configured leave type                                                   | defines the reusable leave program and its unit                |
| module           | accrual, paid status, monetization, conversion, lead time, and workflow | controls how balances are earned, used, converted, or approved |
| employee         | assigned type, opening values, and effective start                      | establishes the employee's balance and eligibility timing      |
| transaction      | leave application, cancellation, conversion, or transfer                | changes or reserves balance under the configured rules         |

## how do i update a leave rule?

1. open the applicable leave setting.
2. review the employees and balances already using the type.
3. update the available rule.
4. review any effective or expiry consequence.
5. click **Save**.

> \[!WARNING] changing an active accrual or expiry rule can affect employee balances. Create a new leave type when the policy meaning changes and the old history must remain distinct.

## related articles

* [assign leave or cto](file:///4659123/leaves/assign_leave_or_cto.md)
* [leave balances](file:///4659123/leaves/leave_balances.md)
* [compensatory time off](file:///4659123/leaves/compensatory_time_off.md)
