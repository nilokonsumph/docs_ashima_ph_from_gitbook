# configure leave settings

## configure leave settings

use leave settings to define leave types, eligibility, accrual, expiry, conversion, and related company rules before assigning leave to employees.

**Navigation:**\
go to **Settings → Leaves**.

### how does leave setup work?

leave setup has two separate steps:

1. **Create the reusable leave type and policy.** this defines who the program applies to, when credits become available, how they accrue, and what happens to unused credits.
2. **Assign the leave type to employees.** this makes the configured program available to a specific employee and records the employee's opening position and effective date.

changing an employee's opening balance does not change the leave policy. changing the leave policy can affect every employee using that type.

### what should i configure?

* leave type name and unit
* earning or accrual rule
* effective and eligibility behavior
* expiry or carryover rule
* conversion or monetization option where supported
* approval and documentation requirements
* CTO source, conversion, rate, and expiry settings when CTO is enabled

### what do the leave-type fields mean?

### identity and units

* **Leave Type Name** — the employee- and admin-facing name of the leave program.
* **Description** — explains the purpose or policy represented by the leave type.
* **Requires Leave Units** — determines whether the type maintains a numeric balance. turn this off only for a type that is tracked without accrued units.
* **Leave Units** — defines how the balance is expressed, such as credits or another supported unit.
* **Paid Leave** — identifies whether approved use is treated as paid leave under the configured payroll rules.

### eligibility

* **Applicable To** — limits the reusable leave policy to the selected employee population.
* **Employment Type**, **Rank**, and **Gender** — refine which employees are eligible when those restrictions apply to the policy.
* **Effective Start Date** — defines when a new employee becomes eligible. it may be based on date hired with a month or year waiting period, or a custom date where supported.

eligibility in the leave type does not by itself assign the type to an employee. the employee still needs an assignment before the balance can be used.

### credits and accrual

* **Accrual Frequency** — controls how often credits are generated. supported choices include anniversary, annual, monthly, and one time.
* **Credits to Accrue** — sets the credit amount for the selected accrual cycle.
* **Accrual Schedule** — controls when the accrual posts, such as the beginning or end of the accrual period, a date based on hire, or a specific date.
* **Earned Leaves / Leave Given Upfront** — establishes the default upfront credit where the policy grants credits in advance.
* **Maximum Accrual or Carry-Forward Limit** — limits how much can accumulate or remain available when the relevant option is enabled.

### negative balance behavior

* **Allow Negative Unpaid Leave** — permits qualifying leave use beyond available paid credits as unpaid leave.
* **Allow Borrowing Unearned Leave** — permits qualifying future credits to be borrowed.

in the current leave-type editor, enabling either choice turns the other off.

these options produce different results, and Ashima allows only one at a time. confirm the company policy before selecting either option.

### unused leave, expiry, and conversion

* **Monetize Unused Leave** — enables supported conversion of unused credits to cash.
* **What Happens to Unused Leave** — selects the configured year-end treatment, such as conversion, carryover, or another available outcome.
* **Carryover Schedule** — defines when carryover is processed.
* **Maximum Carryover** — limits the credits that can move into the next period.
* **Carry-Forward Expiry** — defines whether carried credits expire and, where applicable, after how many months.
* **Unused Leave Upon Termination** — defines the supported treatment of eligible unused credits during final pay.

conversion is not the same as manually reducing a balance. use the configured conversion workflow and its report so the employee movement remains traceable.

### applications and approval

* **Required Lead Time** — defines how early an employee must file the leave request when the rule is enabled.
* **Required Documents** — identifies supporting files required for the leave type. uploaded files are downloadable for approximately 30 days, then deleted for newer files.
* **Workflow Approval** — routes applications through the configured default or custom approver sequence. a custom workflow can also notify staff after approval or rejection.

### how do settings relate to employee assignment?

the leave setting defines the reusable policy. the employee assignment applies a configured leave type to one employee and records opening earned/used values and the effective start rule.

an **Opening Expiry Date** is conditional. it appears for credit-bearing assignments that require an expiry for opening earned credits. for CTO, it appears when the selected CTO type has expiry enabled and can use the configured CTO expiry or a custom date. it does not appear for every leave type, which explains why it can be absent during a valid assignment flow.

the current leave settings list shows the leave unit, whether units are required, paid status, monetization, accrual frequency/start, conversion treatment for unused leave and termination, conversion run, and required lead time. these module rules are not redefined by the employee's opening balance.

### which settings control this workflow?

| level            | setting or record                                                       | effect                                                         |
| ---------------- | ----------------------------------------------------------------------- | -------------------------------------------------------------- |
| company / global | configured leave type                                                   | defines the reusable leave program and its unit                |
| module           | accrual, paid status, monetization, conversion, lead time, and workflow | controls how balances are earned, used, converted, or approved |
| employee         | assigned type, opening values, and effective start                      | establishes the employee's balance and eligibility timing      |
| transaction      | leave application, cancellation, conversion, or transfer                | changes or reserves balance under the configured rules         |

### understand which leave settings change the employee result

use the setting's business effect when reviewing a leave type. the field label alone is not enough.

| setting group                    | what it controls                                                                                               | what the administrator should verify                                                                          |
| -------------------------------- | -------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| type and unit                    | the program name and whether balances are held in credits or the supported time unit                           | the unit matches how employees request leave and how balances are displayed                                   |
| required credits and paid status | whether the type uses a balance and whether approved leave is treated as paid under the supported payroll rule | the employee has sufficient entitlement and payroll uses the intended paid or unpaid treatment                |
| applicability                    | which employees can receive the type, including supported gender, employment, or company criteria              | a representative eligible and ineligible employee behave differently as intended                              |
| accrual period and amount        | when credits are created and how many are added                                                                | the frequency, start boundary, and amount match the written policy                                            |
| accrual start and maximum        | whether credits are added at the beginning or end of a period and where accumulation stops                     | existing balances and the next scheduled allocation do not exceed the intended cap                            |
| negative balance                 | whether excess leave becomes unpaid or can borrow from unearned credits, including any limit                   | only one supported negative-credit treatment is active and the employee result matches it                     |
| advance notice                   | how many days before leave the employee must file                                                              | the request date meets the rule; an unavailable action is not mistaken for a balance problem                  |
| unused-credit treatment          | whether unused credits do nothing, carry forward, convert to cash, or forfeit under the saved rule             | the schedule, maximum, carry-forward expiry, pending applications, and report scope agree                     |
| termination treatment            | what happens to eligible unused leave when employment ends                                                     | the employee balance and final-pay context are reviewed before relying on a cash result                       |
| workflow                         | who reviews and approves the request                                                                           | the company uses the central leave workflow or the supported leave-type-specific route intended for that type |

{% hint style="warning" %}
**warning:** changing an active leave type can affect future accrual, application, expiry, conversion, forfeiture, or final-pay behavior. preserve the old type when its historical meaning must remain distinct, and validate a representative employee before a broad policy change.
{% endhint %}

### configure CTO separately

CTO uses source, rate, expiry, and conversion-access controls that differ from ordinary leave accrual. follow [manage compensatory time off](../balances-transfers-and-cto/manage-compensatory-time-off-cto.md#page-053-pages-admin-leaves-compensatory-time-off-md) for the authoritative setup, calculation, conversion, pool, expiry, correction, and payroll relationship.

### where do i create or find a leave type?

On **Leave Settings**, use **Create New** to open the add form. Complete the policy fields, then choose **Save** or **Cancel**. Open a saved row to inspect its rule; the list also offers the available delete and **XLS** or **CSV** actions. Check existing employee assignments and history before deleting a type.

**ACL Settings** is a separate list for ACL policies. Use **Add New ACL** to create one, then **Save** or **Cancel**. Open a saved ACL row to review it. Do not use the ordinary Leave Settings editor as a substitute for an ACL policy.

### how do i update a leave rule?

1. open the saved policy from **Leave Settings** or **ACL Settings**.
2. review the employees and balances already using the type.
3. choose **Edit** and change the applicable fields.
4. review any effective-date, accrual, or expiry consequence.
5. choose **Update** to save the existing policy, or **Cancel** to leave it unchanged.

{% hint style="warning" %}
**warning:** changing an active accrual or expiry rule can affect employee balances. create a new leave type when the policy meaning changes and the old history must remain distinct.
{% endhint %}

\## what should i review after saving?

* confirm that the leave type appears with the intended paid, accrual, conversion, and lead-time values;
* review a representative employee assignment and effective date;
* confirm that the expected application fields and approval path are available;
* review opening, earned, used, pending, available, expired, and adjusted balances separately; and
* check the transaction ledger or conversion report when the rule changes an existing balance.

### related articles

* [assign leave or CTO](../balances-transfers-and-cto/assign-leave-or-cto.md#page-058-pages-admin-leaves-review-and-maintain-leave-assign-leave-or-cto-md)
* [leave balances](../balances-transfers-and-cto/review-and-correct-leave-balances.md#page-057-pages-admin-leaves-review-and-maintain-leave-leave-balances-md)
* [leave expiry, carryover, and conversion](manage-leave-expiry-carryover-and-conversion.md#page-067-pages-admin-leaves-leave-expiry-carryover-and-conversion-md)
* [compensatory time off](../balances-transfers-and-cto/manage-compensatory-time-off-cto.md#page-053-pages-admin-leaves-compensatory-time-off-md)
