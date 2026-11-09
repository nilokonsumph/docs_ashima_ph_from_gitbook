# Leave settings

use leave settings to define leave types, eligibility, accrual, expiry, conversion, and related company rules before assigning leave to employees.

**Navigation:**\
go to **Settings → Leaves**.

## how does leave setup work?

Leave setup has two separate steps:

1. **Create the reusable leave type and policy.** This defines who the program applies to, when credits become available, how they accrue, and what happens to unused credits.
2. **Assign the leave type to employees.** This makes the configured program available to a specific employee and records the employee's opening position and effective date.

Changing an employee's opening balance does not change the leave policy. Changing the leave policy can affect every employee using that type.

## what should i configure?

* leave type name and unit
* earning or accrual rule
* effective and eligibility behavior
* expiry or carryover rule
* conversion or monetization option where supported
* approval and documentation requirements
* cto source, conversion, rate, and expiry settings when cto is enabled

## what do the leave-type fields mean?

### identity and units

* **Leave Type Name** — the employee- and admin-facing name of the leave program.
* **Description** — explains the purpose or policy represented by the leave type.
* **Requires Leave Units** — determines whether the type maintains a numeric balance. Turn this off only for a type that is tracked without accrued units.
* **Leave Units** — defines how the balance is expressed, such as credits or another supported unit.
* **Paid Leave** — identifies whether approved use is treated as paid leave under the configured payroll rules.

### eligibility

* **Applicable To** — limits the reusable leave policy to the selected employee population.
* **Employment Type**, **Rank**, and **Gender** — refine which employees are eligible when those restrictions apply to the policy.
* **Effective Start Date** — defines when a new employee becomes eligible. It may be based on date hired with a month or year waiting period, or a custom date where supported.

Eligibility in the leave type does not by itself assign the type to an employee. The employee still needs an assignment before the balance can be used.

### credits and accrual

* **Accrual Frequency** — controls how often credits are generated. Supported choices include anniversary, annual, monthly, and one time.
* **Credits to Accrue** — sets the credit amount for the selected accrual cycle.
* **Accrual Schedule** — controls when the accrual posts, such as the beginning or end of the accrual period, a date based on hire, or a specific date.
* **Earned Leaves / Leave Given Upfront** — establishes the default upfront credit where the policy grants credits in advance.
* **Maximum Accrual or Carry-Forward Limit** — limits how much can accumulate or remain available when the relevant option is enabled.

### negative balance behavior

* **Allow Negative Unpaid Leave** — permits qualifying leave use beyond available paid credits as unpaid leave.
* **Allow Borrowing Unearned Leave** — permits qualifying future credits to be borrowed.

These options represent different product behavior and are mutually constrained in the current form. Confirm the company policy before enabling either option.

### unused leave, expiry, and conversion

* **Monetize Unused Leave** — enables supported conversion of unused credits to cash.
* **What Happens to Unused Leave** — selects the configured year-end treatment, such as conversion, carryover, or another available outcome.
* **Carryover Schedule** — defines when carryover is processed.
* **Maximum Carryover** — limits the credits that can move into the next period.
* **Carry-Forward Expiry** — defines whether carried credits expire and, where applicable, after how many months.
* **Unused Leave Upon Termination** — defines the supported treatment of eligible unused credits during final pay.

Conversion is not the same as manually reducing a balance. Use the configured conversion workflow and its report so the employee movement remains traceable.

### applications and approval

* **Required Lead Time** — defines how early an employee must file the leave request when the rule is enabled.
* **Required Documents** — identifies supporting files required for the leave type.
* **Workflow Approval** — routes applications through the configured default or custom approver sequence. A custom workflow can also notify staff after approval or rejection.

## how do settings relate to employee assignment?

the leave setting defines the reusable policy. The employee assignment applies a configured leave type to one employee and records opening earned/used values and the effective start rule.

An **Opening Expiry Date** is conditional. It appears for credit-bearing assignments that require an expiry for opening earned credits. For CTO, it appears when the selected CTO type has expiry enabled and can use the configured CTO expiry or a custom date. It does not appear for every leave type, which explains why it can be absent during a valid assignment flow.

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

## what should i review after saving?

* confirm that the leave type appears with the intended paid, accrual, conversion, and lead-time values;
* review a representative employee assignment and effective date;
* confirm that the expected application fields and approval path are available;
* review opening, earned, used, pending, available, expired, and adjusted balances separately; and
* check the transaction ledger or conversion report when the rule changes an existing balance.

## related articles

* [assign leave or cto](/broken/pages/775b5570a1a5dc9270a73ef8160f41f7e5315cc8)
* [leave balances](/broken/pages/c91635aff7ed4863a292ef86e31e9ffc9f27050b)
* [leave expiry, carryover, and conversion](/broken/pages/b168e4f85d7d4baee68ae65642130a5d3d94f5c0)
* [compensatory time off](/broken/pages/c745ebbfd65fb85e023d427427543c48142481a7)
