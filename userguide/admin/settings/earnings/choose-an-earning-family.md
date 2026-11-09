# choose an earning family

use Earnings settings to define the earning items that administrators can later assign to employees. This page is a guide to the earning families; it is not a substitute for the detailed setup and assignment instructions for each family.

**navigation:** go to **Settings → Paycheck → Earnings**, then select the required earning family.

## which earning family should i use?

| family          | use it for                                                                                       | important distinction                                                                         |
| --------------- | ------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------- |
| allowance       | a named allowance with its own rate, payout schedule, applicability, and tax rule                | can be flat-rate or rate-based and may be affected by absence or worked-time rules            |
| other earnings  | a one-time or recurring earning that does not belong to a more specific earning family           | uses an explicit pay date or a recurring interval/occurrence schedule                         |
| de minimis      | a supported de minimis benefit with a prescribed non-taxable ceiling and taxable excess handling | is not the same as an ordinary non-taxable allowance or other earning                         |
| compensation    | the employee's base pay and salary history                                                       | use the salary-increase workflow for effective-dated basic-pay changes                        |
| retroactive pay | the result of an effective-dated salary correction                                               | review the affected periods and generated retro result; do not create it as a generic earning |

choose the family that matches the business, tax, payroll, and reporting meaning. A field that accepts an amount does not make the families interchangeable.

## common setup-to-payroll flow

1. create the reusable item under **Settings → Paycheck**.
2. Define its applicability, calculation, schedule, and tax treatment.
3. save the item.
4. open the matching Earnings or employee page.
5. Assign the item to the eligible employee or employees.
6. review the assignment amount, dates, and schedule.
7. Recalculate any affected open payroll.
8. confirm the item on the employee pay details, payslip, and applicable payroll reports.

creating an item does not automatically pay every eligible employee. The employee assignment is a separate step.

## tax and reporting reminder

allowance and Other Earnings screens can classify an earning as **Taxable** or **Non Taxable**. Their current user interface states that non-taxable classification participates in the ₱90,000 tax-exemption ceiling. Do not describe a non-taxable item as permanently tax-free without reviewing the employee's cumulative treatment.

De Minimis uses its own configured ceiling and records an excess amount for taxable treatment. Use the De Minimis family when the benefit is intended to follow that workflow.

## changing an item already in use

before editing, deleting, or repurposing an item, review:

* current employee assignments;
* open payroll using the item;
* completed payroll and reports that identify the item;
* effective dates and remaining occurrences; and
* whether a replacement item would preserve historical meaning more safely.

{% hint style="warning" %}
**warning:** when the business or tax meaning changes materially, create a replacement item instead of reusing an established item for a new purpose.
{% endhint %}

\## detailed instructions

* [allowances](configure-and-assign-allowances.md)
* [other earnings](configure-and-assign-other-earnings.md)
* [de minimis settings](configure-de-minimis-item-types-and-limits.md)
* [employee de minimis assignments](assign-and-manage-de-minimis.md)
* [compensation details](../../workforce/)
* [employee pay details](../../paycheck/)
