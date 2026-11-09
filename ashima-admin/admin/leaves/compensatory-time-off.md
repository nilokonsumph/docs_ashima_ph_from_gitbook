# compensatory time off

cto means compensatory time off. It is time-off credit created from approved source work, such as overtime, rest day work, or holiday work.

cto is not normally earned by schedule or yearly accrual. It is created when eligible approved work is converted into cto credits.

use **compensatory time off (cto)** to convert approved overtime, rest day work, or holiday work into time-off credits that employees can apply for later.

{% hint style="info" %}
changing cto settings affects which approved work can become cto, how credits are calculated, when credits expire, and how the same source work is treated in payroll. review the settings before saving.current CTO boundaries
{% endhint %}

**navigation:**\
go to **Leaves → cto settings**

### when should you use cto?

use cto when the company allows approved work to become time-off credits instead of paying that work only as overtime, rest day pay, or holiday pay.

example:

`approved overtime → converted into cto → cto credits added to the employee balance`\
\
some pages use **conversion**, **converted**, **wrapped**, or **earned**. in this guide, these terms refer to the same user-facing result: approved source work becomes cto credits.

### where does cto appear?

cto is managed through the leave module, but cto is not the same as ordinary leave.

ordinary leave is usually earned or accrued based on a policy. cto is a credit bank created from approved source work, such as overtime, rest day work, or holiday work.

because cto is managed inside the leave module, some screens may still use leave-related labels.

the leave module shows the employee's assigned cto leave type, available credits, pending credits, used credits, expiry date, and transaction history.

### what do cto balance terms mean?

| term      | simple meaning                                                                                                |
| --------- | ------------------------------------------------------------------------------------------------------------- |
| available | cto credits the employee can still use.                                                                       |
| pending   | cto credits reserved for a leave request that is waiting for approval. some screens may show this as applied. |
| approved  | cto credits attached to an approved cto leave request.                                                        |
| used      | cto credits already used for approved time off. some screens may show this as consumed.                       |
| expired   | cto credits that can no longer be used because the expiry rule has already applied.                           |

simple balance idea:

`available cto = credited cto - pending cto - used cto - expired cto +/- adjustments`

### what is a cto pool?

a cto pool is a group of cto credits that share the same employee, cto leave type, source type, and expiry date.

example:

`employee: ben aguilar`&#x20;

`cto leave type: cto - overtime`&#x20;

`source type: overtime`&#x20;

`expiry date: 2026-05-31`

if the same employee has multiple overtime conversions that create **cto - overtime** credits with the same expiry date, those credits may be grouped together in one pool.

a pool is not always equal to one overtime, rest day, or holiday record. one pool may include credits from more than one converted source record. use the ledger or more-info view when you need to trace the exact source records that created the credits.

### what does each cto page display?

| page                    | what you use it for                                                                                                        |
| ----------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| **cto settings**        | turn cto on or off, choose source types, set conversion rates, set expiry rules, and choose who can convert approved work. |
| **cto leave types**     | review cto leave types generated from cto settings.                                                                        |
| **leave balance**       | review employee cto balances, assignments, available credits, pending credits, and transaction history.                    |
| **cto conversions**     | review approved source rows that are ready to convert into cto.                                                            |
| **cto leave import**    | upload cto balances into the leave nil engine.                                                                             |
| **employee leave page** | let employees apply for assigned cto leave types.                                                                          |

### how do i set up cto?

1. go to **Leaves → cto settings**.
2. turn **enable compensatory time off (cto)** on.
3. select the cto source types in **cto time types**.
4. set the **cto minting rate** for each selected source type.
5. choose the **should cto expire** rule for each selected source type.
6. choose the **cto conversion access** setting.
7. click **save cto settings**.

### fields

* **enable compensatory time off (cto)** — turns cto on or off for the company.
* **cto time types** — selects which approved work types can become cto. the supported source types are overtime, rest day, and holiday.
* **cto minting rate** — sets how many cto minutes are created from source minutes.
* **should cto expire** — sets whether cto credits expire and how the expiry date is calculated.
* **cto conversion access** — sets who can convert approved work into cto.



### what happens after i save cto settings?

the system saves the cto rules and creates or reactivates generated cto leave types for the selected source types.

examples:

* **CTO - Overtime**
* **CTO - Rest Day**
* **CTO - Holiday**

if you remove a cto source type, the system deactivates the generated leave type for new use. existing balances and transaction history remain traceable.

### how do cto source types work?

cto supports these source types:

<figure><img src="../../.gitbook/assets/Screenshot 2026-06-11 at 15.55.57.png" alt=""><figcaption></figcaption></figure>

| source type | what it means                       |
| ----------- | ----------------------------------- |
| overtime    | approved overtime work becomes cto. |
| rest day    | approved rest day work becomes cto. |
| holiday     | approved holiday work becomes cto.  |

only approved source work should become cto. pending, rejected, cancelled, already converted, zero-minute, missing-assignment, or unrelated source work should not be converted.

### how does the cto minting rate work?

minting is the credit-creation step inside cto conversion.

plainly, conversion decides that approved source work will become cto. minting calculates how many cto minutes are added to the employee's balance.

the cto minting rate controls how many cto minutes are created from source minutes.

`source minutes × cto minting rate = cto minutes`

examples:

`3 hours overtime (180 minutes) at 1.00x = 3 hours cto (180 minutes)`&#x20;

`2 hours rest day work (120 minutes) at 1.50x = 3 hours cto (180 minutes)`&#x20;

`1 hour holiday work (60 minutes) at 2.00x = 2 hours cto (120 minutes)`

some pages show the saved rate as a ratio instead of an x value.

examples:

`1:1 = 1.00x` \
`135:100 = 1.35x` \
`178:100 = 1.78x`

### can converted cto be reverted?

converted cto should not be directly reverted back to ordinary overtime, rest day pay, or holiday pay once credits have been added to the employee balance.

if a correction is needed, use the proper correction process instead. this keeps the cto balance, payroll treatment, and transaction history clear.

common correction cases include:

* deducting cto through a manual adjustment when credits were added incorrectly
* reviewing payroll treatment if the original source work should be paid instead
* checking whether the cto credit was already applied, approved, cancelled, or expired before making a correction

### how are decimal cto minutes handled?

cto uses whole minutes. when a conversion creates a decimal minute, the system rounds half up per source row.

examples:

`15.49 minutes becomes 15 minutes`&#x20;

`15.50 minutes becomes 16 minutes`&#x20;

`15.51 minutes becomes 16 minutes`

the system finalizes the rounded cto minutes per source row. it does not combine several rows first and then round the total.

### how do cto expiry rules work?

expiry is set per cto source type.

| expiry rule      | what happens                                                                         |
| ---------------- | ------------------------------------------------------------------------------------ |
| does not expire  | cto credits stay available until used or adjusted.                                   |
| after x days     | cto credits expire after the configured number of days from the conversion run date. |
| end of the month | cto credits expire at the end of the conversion run month.                           |
| end of the year  | cto credits expire at the end of the conversion run year.                            |

if cto does not expire, the credits remain available until they are used, adjusted, or otherwise changed by an authorized action.

for **after x days**, **end of the month**, and **end of the year**, the expiry date is based on the cto conversion date. it is not based on the original overtime, rest day, or holiday work date.\
\
example:\
\
`overtime work date: 2026-04-20`

`conversion run date: 2026-05-07`&#x20;

`validity: 10 days`&#x20;

`expiry date: 2026-05-17`

{% hint style="info" %}
the expiry date is based on the cto conversion date. it is not based on the original overtime, rest day, or holiday work date.
{% endhint %}

### who can convert approved work into cto?

the **cto conversion access** setting controls who can initiate cto conversion.

| option                        | what it means                                                               |
| ----------------------------- | --------------------------------------------------------------------------- |
| **admin manual conversion**   | only users with admin access convert eligible work from the admin workflow. |
| **approvers during approval** | assigned approvers choose cto during approval when the workflow allows it.  |

### how do i review cto leave types?

open **cto leave settings** to review cto leave types generated by cto settings.

the page displays the cto leave type, cto source, conversion rate, expiry rule, assigned employee count, leave units, and availability.

if no cto source types are enabled, the page shows that no cto leave types were found and instructs you to enable cto time types from cto settings.

### how do i convert approved work into cto?



1. open **cto conversions**.
2. filter by employee, source, date range, or status.
3. review the source row details.
4. select rows with a ready status.
5. click the conversion action shown on the page.

depending on the page, the button may show **wrap selected** or **wrap selected and mint CTO**. both actions convert the selected source rows into cto.

### what happens after i convert selected rows?

the system converts the selected source rows into cto credits. the employee cto balance increases, the source row is marked converted, and the transaction is recorded in the ledger.

the same approved source work should not also be paid again as the same overtime, rest day, or holiday pay.

`converted into cto = not paid again as the same source work`

to check: before closing payroll, review open or draft pay runs when cto conversion affects overtime, rest day work, or holiday work. this helps confirm that the same source work is not counted both as paid work and as cto.

### what do cto conversion statuses mean?

| status             | what it means                                                              |
| ------------------ | -------------------------------------------------------------------------- |
| all                | shows all source rows in the selected filters.                             |
| ready              | the source row is eligible for cto conversion.                             |
| converted          | the source row was already converted into cto.                             |
| missing assignment | the employee does not have the matching generated cto leave type assigned. |
| zero minutes       | the source row has no convertible minutes.                                 |

rows should only be selectable when they are ready for conversion.

### can the same source work be converted twice?

no. each source row should be converted only once.

the system checks whether the source work was already converted before allowing another conversion.

### how does an employee apply for cto?

the employee applies through the employee leave page and selects the assigned cto leave type.

the employee should review the cto leave type, requested date, requested duration, and available cto balance before submitting.

### can an employee apply for more cto than available?

no. generated cto leave types do not allow negative balance or borrowed cto.

if the requested cto is more than the available cto, the system should block the request with an insufficient balance message.

### what happens while a cto application is pending?

the requested cto is reserved while the application waits for approval.

this means the available cto balance decreases and the pending cto balance increases. pending cto should not expire while it is reserved.

### what happens when cto is approved?

the system releases the pending reservation and records the approved cto usage.

for forward usage, the system uses earliest-expiry-first allocation. credits that expire sooner are used before credits that expire later.

### what happens when cto is rejected?

the system returns the reserved cto using the refund rule.

returned credits go back to an eligible available balance for the same cto leave type.

### what happens when cto is cancelled?

the system reverses the pending or approved cto application, depending on the application status and permissions.

if cancellation returns credits, the system returns them to an eligible available balance for the same cto leave type. if no eligible balance is available, cancellation should be blocked.

when an application used credits from more than one expiry date, cancellation returns the later-expiring credits first. this keeps earlier-expiring credits used first and helps preserve credits with more time left.

example:

`cto used from credits expiring 2026-05-30`&#x20;

`cto used from credits expiring 2026-08-30`&#x20;

`cancelled cto returns first to the 2026-08-30 credits`\
<br>

### what happens when cto expires?

expiry removes unused available cto that has reached its expiry date.

expiry should not remove pending cto, approved cto, consumed cto, or historical ledger records.

if a pending cto application is later rejected or cancelled, the returned credits follow the refund rule.

### what does the leave balance page show?

open **leave balance** to review employee cto balances from the leave module.

the page displays employee details, leave type, leave units, credits added, available balance, pending balance, credit date, and transaction links.

### how do i import cto balances?

use **cto leave import** to upload cto balances into the leave module.

the import file must contain:

`Employee Number | Leave Type | Classification | Description | Transaction | Effective Start Date`

**Effective Start Date** accepts:

* 1|month
* 2|year
* MM/DD/YYYY
* YYYY-MM-DD

relative dates require a valid employee hire date.

### what does the cto ledger show?

use the ledger to trace cto transactions.

the ledger should help you review credits created from source work, cto applications, approvals, rejections, cancellations, expiries, and manual adjustments.

for deeper tracing, open the transaction detail or more-info view.

### what should i review in more info?

use more info to trace where a cto movement came from and what it affected.

useful details include source type, source date, source minutes, minting rate, credited cto minutes, expiry date, application reference, action taken, person who performed the action, and action date.

the more-info view should show only details that help you understand the cto movement.

use more info when you need to answer questions such as:

* which approved overtime, rest day work, or holiday work created this cto?
* how many minutes were converted into cto?
* what expiry date was assigned?
* was the cto later applied, approved, rejected, cancelled, expired, or adjusted?

### can i add manual cto adjustments?

use manual cto adjustments only for corrections.

manual credits and deductions should have a clear reason and should remain separate from source-converted cto so the audit trail stays clear.

### troubleshooting

| issue                                                        | what to check                                                                                                                    |
| ------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------- |
| cto source rows do not appear                                | check that cto is enabled, the source type is selected, and the source work is approved.                                         |
| a row shows missing assignment                               | assign the employee to the matching generated cto leave type.                                                                    |
| a row is not selectable                                      | check the row status. converted, zero-minute, missing-assignment, pending, rejected, or cancelled rows should not be selectable. |
| cto leave types are missing                                  | enable at least one cto time type and save cto settings.                                                                         |
| the converted minutes look different from the decimal result | cto uses whole minutes and rounds half up per source row.                                                                        |
| an employee cannot apply for cto                             | check that the cto leave type is assigned and that the employee has enough available balance.                                    |





<br>
