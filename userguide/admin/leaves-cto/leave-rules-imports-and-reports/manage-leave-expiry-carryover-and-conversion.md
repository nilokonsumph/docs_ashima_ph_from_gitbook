# manage leave expiry, carryover, and conversion

## manage leave expiry, carryover, and conversion

use the leave policy and employee transaction history together when reviewing unused credits. expiry, carryover, and cash conversion are different outcomes and should not be treated as a single balance adjustment.

**Navigation:**\
go to **Settings → Leaves** for the governing rule, **Leaves → Leave Balance** for employee records, or **Reports → Leaves** for supported conversion and forfeiture outputs.

### what is the difference?

* **Expiry** removes unused credits from availability when the configured expiry condition is reached.
* **Carryover** moves eligible unused credits into the next leave period, subject to the configured maximum and expiry rule.
* **Conversion** turns eligible unused credits into a supported cash result and report entry.
* **Adjustment** is an authorized correction to a specific employee balance. it does not replace the configured expiry, carryover, or conversion process.

### where is the rule defined?

go to **Settings → Leaves**, then open the applicable leave type. review:

* whether unused leave is monetized;
* what happens to unused leave;
* the carryover schedule;
* the maximum carryover;
* carry-forward expiry;
* conversion timing; and
* the treatment of unused leave upon termination.

the leave type is the reusable company rule. the employee assignment supplies the employee's opening position and effective date; it does not redefine the company policy.

### what is the opening expiry date?

an **Opening Expiry Date** applies to the opening earned credits entered when the leave type is assigned, when the selected type requires that date. it is not shown for every leave type.

do not use an opening expiry date to simulate a company-wide expiry rule. future accruals, carried credits, and CTO conversions follow their applicable policy and transaction dates.

### how should i review expiry?

1. confirm the leave type's expiry or carry-forward rule;
2. open the employee's leave details;
3. confirm which credits are opening, accrued, carried, converted, or manually added;
4. review the applicable credit or expiry date;
5. use **View Transaction** or the transaction ledger to trace the movement; and
6. confirm that expired credits are no longer included in available balance.

for CTO, use the dedicated CTO guide. CTO expiry is defined per source type and is applied to source-converted credit pools, not ordinary leave accrual.

### how should i review leave conversion?

1. confirm that the leave type allows monetization or the applicable conversion outcome;
2. confirm the conversion schedule and any maximum;
3. review the employee's available, pending, approved, used, and expired credits;
4. resolve or account for pending applications before the conversion run;
5. generate the leave conversion output for the intended period;
6. review converted, excluded, and forfeited results; and
7. retain the report as the supporting output for payroll and audit review.

{% hint style="warning" %}
**important:** do not manually deduct credits merely to imitate conversion. a manual balance change can leave the cash result and conversion reporting incomplete.
{% endhint %}

### what happens upon termination?

the leave type's termination rule determines the configured treatment of eligible unused credits. review the employee balance, pending applications, expiry state, and final-pay context before relying on a conversion value.

### troubleshooting

#### opening expiry date is not displayed

the selected leave or CTO type may not require an expiry for opening credits. review the leave-type or CTO settings before treating the missing field as an error.

#### available balance does not match earned minus used

pending applications, approved allocations, expired credits, carryover, conversion, cancellation returns, or adjustments may also affect the balance. open the transaction ledger.

#### conversion result is lower than expected

check the maximum conversion or carryover rule, pending or approved applications, expired credits, and whether the employee's leave type is eligible for monetization.
